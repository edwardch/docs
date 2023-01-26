# Connections and Transactions

Serenity uses the basic data access objects in .NET, like IDbConnection, DbCommand, etc.

It provides some basic helpers to create a connection, add parameters, execute queries, etc.

## ISqlConnections Interface

The [ISqlConnections](../../api/dotnet/Serenity.Net.Data/Serenity.Data/ISqlConnections.md) is a factory interface to create a connection in a database-agnostic way.

```cs
public interface ISqlConnections : IConnectionStrings
{
    IDbConnection New(string connectionString, string providerName, ISqlDialect dialect);
    IDbConnection NewByKey(string connectionKey);
}
```

The `New` method in `ISqlConnections` creates a method by specifying the full connection string, the provider name, and the dialect instance that should be used.

The `NewByKey` method is for creating a connection by its key:

```cs
public class SomeClass
{
    private ISqlConnections sqlConnections;

    // assuming ISqlConnections is injected via dependency injection
    public SomeClass(ISqlConnections sqlConnections)
    {
        this.sqlConnections = sqlConnections ??
            throw new ArgumentNullException(nameof(sqlConnections));
    }

    public void SomeOperation()
    {
        using (var connection = sqlConnections.NewByKey("Northwind"))
        {
            // do something with the connection instance
            // as long as you use Serenity connection extension
            // methods to query the database, you don't have to
            // manually open the connection
        }
    }
}
```

The default implementation for `ISqlConnections` which is [DefaultSqlConnections](../../api/dotnet/Serenity.Net.Data/Serenity.Data/DefaultSqlConnections.md) creates a connection by locating the connection definition from the `Data` section in the `appsettings.json` file:

```json
  "Data": {
    "Default": {
      "ConnectionString": "...",
      "ProviderName": "System.Data.SqlClient"
    },
    "Northwind": {
      "ConnectionString": "...",
      "ProviderName": "System.Data.SqlClient"
    }
  }
```

The type of connection that should be created is specified in the `ProviderName` property.  The provider names and their connection factories are mapped via the `RegisterDataProviders` method in the `Startup.cs` file:

```cs
public static void RegisterDataProviders()
{
    DbProviderFactories.RegisterFactory("System.Data.SqlClient", SqlClientFactory.Instance);
    DbProviderFactories.RegisterFactory("Microsoft.Data.SqlClient", SqlClientFactory.Instance);
    DbProviderFactories.RegisterFactory("Microsoft.Data.Sqlite", Microsoft.Data.Sqlite.SqliteFactory.Instance);

    // to enable FIREBIRD: add FirebirdSql.Data.FirebirdClient reference, set connections, and uncomment line below
    // DbProviderFactories.RegisterFactory("FirebirdSql.Data.FirebirdClient", FirebirdSql.Data.FirebirdClient.FirebirdClientFactory.Instance);
    // ...
}
```

As listed above, only the SQL Server and the `SQLite` connection factories are registered by default. If you want to use another type of server, you should uncomment the relevant line there, and add the NuGet reference for its client library in the project file.

The default implementations for the `ISqlConnections` and other related services are registered via an [AddSqlConnections](../../api/dotnet/Serenity.Net.Data/Serenity.Extensions.DependencyInjection/DataServiceCollectionExtensions.md) call. You may not see it in the `Startup.cs` file as it is indirectly called by the `AddServiceHandlers` method.

## SqlConnectionExtensions.NewFor`<TClass>` extension method

If you don't want to memorize connection string keys, but instead reuse information on a row (in form of a `ConnectionKey` attribute), you may prefer this variant.

Looking on top of a Row class, you may spot the `ConnectionKey` attribute generated by `Sergen`:

```cs
[ConnectionKey("Northwind")]
public class CustomerRow
{
}
```

When you are going to query for customers, instead of hardcoding `"Northwind"`, you may reuse this information from the `CustomerRow`:

```cs
using (var connection = sqlConnections.NewFor<CustomerRow>()) 
{
    return connection.List<CustomerRow>();
}
```

This corresponds to `SqlConnections.NewByKey("Northwind")`.

Here we didn't have to open the connection, as the `List` extension method opens it automatically.

The class used with this method doesn't have to be a `Row`, any class with a `ConnectionKey` attribute would work, even though it would be a row type most of the time.

## WrappedConnection

You may ask yourself, what is the point of using the `ISqlConnections` interface and its `New` and `NewByKey` methods instead of simply typing `new SqlConnection()`?

All the `ISqlConnections` methods return an `IDbConnection` object. You'd expect it to be a `SqlConnection`, `FirebirdConnection`, etc, but that's not exactly true.

The IDbConnection object they return is a `WrappedConnection` instance that wraps an underlying SqlConnection or FirebirdConnection etc.

This helps Serenity provide some features like auto-open, dialect support, default transactions, unit of work pattern, overriding connections for testability, etc.

You may not notice these details while working with the returned IDbConnection instances. They'll act just like the underlying connections. 

But you should prefer the methods of `ISqlConnections` to create connections. Otherwise, you might lose some of these listed features.

## Setting Database Dialect for Connections

Serenity tries to auto-determine the dialect for a connection by using the `"providerName"` in the `appsettings.json` file for the connection definition.

Sometimes, the dialect determined automatically using the `"providerName"` may not work for you, or you may want to use a dialect like `SqlServer2000` or `SqlServer2005` for some connections.

Even though it is possible to set a default global dialect, it doesn't override the automatic detection:

```cs
SqlSettings.DefaultDialect = SqlServer2005Dialect.Instance;
```

Because the provider name for "Northwind" and "Default" connections is `System.Data.SqlClient`, Serenity will automatically set their dialects to `SqlServer2012`, even if you override the global dialect.

It is possible to set the dialect in the connection definition in the `appsettings.json` file:

```json
{
  "Data": {
    "Default": {
      "ConnectionString": "...",
      "ProviderName": "System.Data.SqlClient",
      "Dialect": "SqlServer2012"
    }
  }
}
```

For the dialects provided by Serenity, it is enough to only specify the dialect class name. 

If you defined a custom dialect, you may need to use the full name of the class and the assembly name:

```json
{
  "Data": {
    "Default": {
      "ConnectionString": "...",
      "ProviderName": "System.Data.SqlClient",
      "Dialect": "MyProject.MyNamespace.MyCustomSqlDialect, MyProject.Web"
    }
  }
}
```

## UnitOfWork and IUnitOfWork

`UnitOfWork` is a simple object that just contains a transaction reference. It has two extra events that we can attach to which are `OnCommit` and `OnRollback`.

Let's say we are creating tasks, and some e-mails should be sent in case these tasks are saved to the database successfully.

If we hurry and send these e-mails before the transaction is committed, we might end up with e-mails that are sent for non-existent tasks in case the transaction fails. So we should only send the e-mail if the transaction is committed successfully, e.g. in the `OnCommit`` event.

You might say then Commit the transaction first and send e-mails right after, but what if our Create Task service call is just a step of a larger operation, so we are not controlling the transaction and it should be committed after all steps are successful?

Another scenario is about uploading files. This time we are updating an item that contains files, and let's say we replace an old file with the uploaded new file. If we again hurry and delete the old file before the transaction outcome is clear, and the transaction fails eventually, we'll end up with a file entity without an actual old file on the disk. So, we should delete the file and replace it with the new file in the `OnCommit` event, and remove the uploaded file in the `OnRollback` event.

```cs
void SomeBatchOperation() 
{
    using (var connection = sqlConnections.NewByKey("Default"))
    using (var uow = new UnitOfWork(connection))
    {
        // here we are in a transaction context
        // create several tasks in transaction
        CreateATask(new TaskRow { ... });
        CreateATask(new TaskRow { ... });
        //...
        
        // commit the transaction
        // if any exception occurs here or at prior
        // lines transaction will rollback
        // and no e-mails will be sent
        uow.Commit();
    }
}

void CreateATask(IUnitOfWork uow, TaskRow task)
{
    // insert task using the connection wrapped inside IUnitOfWork
    // this will automatically run in the current transaction context
    uow.Connection.Insert(task);
   
    uow.OnCommit += () => {
       // send e-mail for this task now, this method will only
       // be called if the transaction commits successfully
    };
    
    uow.OnRollback += () => {
       // optional, do something else if it fails
    };
}
```



