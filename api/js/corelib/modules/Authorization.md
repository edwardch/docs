[@serenity-is/corelib](../README.md) / Authorization

# Namespace: Authorization

Contains permission related functions.

## Note
We use a namespace here both for compatibility and for allowing users to override
these functions easily in ES modules environment, which is normally hard to do.

## Table of contents

### Variables

- [isLoggedIn](Authorization.md#isloggedin)
- [isLoggedInAsync](Authorization.md#isloggedinasync)
- [userDefinition](Authorization.md#userdefinition)
- [userDefinitionAsync](Authorization.md#userdefinitionasync)
- [username](Authorization.md#username)
- [usernameAsync](Authorization.md#usernameasync)

### Functions

- [hasPermission](Authorization.md#haspermission)
- [hasPermissionAsync](Authorization.md#haspermissionasync)
- [isPermissionInSet](Authorization.md#ispermissioninset)
- [validatePermission](Authorization.md#validatepermission)
- [validatePermissionAsync](Authorization.md#validatepermissionasync)

## Variables

### isLoggedIn

• **isLoggedIn**: `boolean`

Checks if the current user is logged in. Prefer `isLoggedInAsync` as this one might block the UI if the `UserData`
is not already loaded.

**`Example`**

```ts
if (Authorization.isLoggedIn) {
    // do something
}
```

#### Defined in

[src/q/authorization.ts:151](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/q/authorization.ts#L151)

___

### isLoggedInAsync

• **isLoggedInAsync**: `Promise`\<`boolean`\>

Checks if the current user is logged in.

**`Example`**

```ts
if (await Authorization.isLoggedInAsync) {
    // do something
}
```

#### Defined in

[src/q/authorization.ts:161](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/q/authorization.ts#L161)

___

### userDefinition

• **userDefinition**: [`UserDefinition`](../interfaces/UserDefinition.md)

Returns the user data for currently logged user. Prefer `userDefinitionAsync` as this one might block the UI if the `UserData`
is not already loaded.

**`Example`**

```ts
if (Authorization.userDefinition.IsAdmin) {
    // do something
}
```

#### Defined in

[src/q/authorization.ts:190](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/q/authorization.ts#L190)

___

### userDefinitionAsync

• **userDefinitionAsync**: `Promise`\<[`UserDefinition`](../interfaces/UserDefinition.md)\>

Returns the user data for currently logged user.

**`Example`**

```ts
if ((await Authorization.userDefinitionAsync).IsAdmin) {
    // do something
}
```

#### Defined in

[src/q/authorization.ts:199](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/q/authorization.ts#L199)

___

### username

• **username**: `string`

Returns the username for currently logged user. Prefer `usernameAsync` as this one might block the UI if the `UserData`
is not already loaded.

**`Example`**

```ts
if (Authorization.username) {
    // do something
}
```

#### Defined in

[src/q/authorization.ts:171](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/q/authorization.ts#L171)

___

### usernameAsync

• **usernameAsync**: `Promise`\<`string`\>

Returns the username for currently logged user.

**`Example`**

```ts
if (await Authorization.usernameAsync) {
    // do something
}
```

#### Defined in

[src/q/authorization.ts:180](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/q/authorization.ts#L180)

## Functions

### hasPermission

▸ **hasPermission**(`permission`): `boolean`

Checks if the current user has the permission specified.
This should only be used for UI purposes and it is strongly recommended to check permissions server side.

> Please prefer the `hasPermissionAsync` variant as this may block the UI thread if the `UserData` script is not already loaded.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `permission` | `string` | Permission key. It may contain logical operators like A&B\|C. |

#### Returns

`boolean`

`false` for "null or undefined", true for "*", `IsLoggedIn` for "?". For other permissions, 
if the user has the permission or if the user has the `IsAdmin` flag (super admin) `true`, otherwise `false`.

#### Defined in

[src/q/authorization.ts:25](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/q/authorization.ts#L25)

___

### hasPermissionAsync

▸ **hasPermissionAsync**(`permission`): `Promise`\<`boolean`\>

Checks if the current user has the permission specified.
This should only be used for UI purposes and it is strongly recommended to check permissions server side.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `permission` | `string` | Permission key. It may contain logical operators like A&B\|C. |

#### Returns

`Promise`\<`boolean`\>

`false` for "null or undefined", true for "*", `IsLoggedIn` for "?". For other permissions, 
if the user has the permission or if the user has the `IsAdmin` flag (super admin) `true`, otherwise `false`.

#### Defined in

[src/q/authorization.ts:56](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/q/authorization.ts#L56)

___

### isPermissionInSet

▸ **isPermissionInSet**(`permissionSet`, `permission`): `boolean`

Checks if the hashset contains the specified permission, also handling logical "|" and "&" operators

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `permissionSet` | `Object` | Set of permissions |
| `permission` | `string` | Permission key or a permission expression containing & \| operators |

#### Returns

`boolean`

true if set contains permission

#### Defined in

[src/q/authorization.ts:82](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/q/authorization.ts#L82)

___

### validatePermission

▸ **validatePermission**(`permission`): `void`

Throws an error if the current user does not have the specified permission. 
Prefer `await validatePermissionAsync()` as this one might block the UI if the `UserData`
is not already loaded.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `permission` | `string` | Permission key. It may contain logical operators like A&B\|C. |

#### Returns

`void`

#### Defined in

[src/q/authorization.ts:120](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/q/authorization.ts#L120)

___

### validatePermissionAsync

▸ **validatePermissionAsync**(`permission`): `Promise`\<`void`\>

Throws an error if the current user does not have the specified permission.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `permission` | `string` | Permission key. It may contain logical operators like A&B\|C. |

#### Returns

`Promise`\<`void`\>

**`Example`**

```ts
await Authorization.validatePermissionAsync("A&B|C");
```

#### Defined in

[src/q/authorization.ts:133](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/q/authorization.ts#L133)
