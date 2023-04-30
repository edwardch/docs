[@serenity-is](../README.md) / [Modules](../modules.md) / [corelib](../modules/corelib.md) / LookupEditorBase

# Class: LookupEditorBase<TOptions, TItem\>

[corelib](../modules/corelib.md).LookupEditorBase

## Type parameters

| Name | Type |
| :------ | :------ |
| `TOptions` | extends [`LookupEditorOptions`](../interfaces/corelib.LookupEditorOptions.md) |
| `TItem` | `TItem` |

## Hierarchy

- [`Select2Editor`](corelib.Select2Editor.md)<`TOptions`, `TItem`\>

  ↳ **`LookupEditorBase`**

  ↳↳ [`LookupEditor`](corelib.LookupEditor.md)

## Table of contents

### Constructors

- [constructor](corelib.LookupEditorBase.md#constructor)

### Properties

- [cascadeLink](corelib.LookupEditorBase.md#cascadelink)
- [element](corelib.LookupEditorBase.md#element)
- [idPrefix](corelib.LookupEditorBase.md#idprefix)
- [lastCreateTerm](corelib.LookupEditorBase.md#lastcreateterm)
- [lookup](corelib.LookupEditorBase.md#lookup)
- [onInitNewEntity](corelib.LookupEditorBase.md#oninitnewentity)
- [openDialogAsPanel](corelib.LookupEditorBase.md#opendialogaspanel)
- [options](corelib.LookupEditorBase.md#options)
- [uniqueName](corelib.LookupEditorBase.md#uniquename)
- [widgetName](corelib.LookupEditorBase.md#widgetname)

### Accessors

- [cascadeField](corelib.LookupEditorBase.md#cascadefield)
- [cascadeFrom](corelib.LookupEditorBase.md#cascadefrom)
- [cascadeValue](corelib.LookupEditorBase.md#cascadevalue)
- [filterField](corelib.LookupEditorBase.md#filterfield)
- [filterValue](corelib.LookupEditorBase.md#filtervalue)
- [itemById](corelib.LookupEditorBase.md#itembyid)
- [items](corelib.LookupEditorBase.md#items)
- [readOnly](corelib.LookupEditorBase.md#readonly)
- [selectedItem](corelib.LookupEditorBase.md#selecteditem)
- [selectedItems](corelib.LookupEditorBase.md#selecteditems)
- [text](corelib.LookupEditorBase.md#text)
- [value](corelib.LookupEditorBase.md#value)
- [values](corelib.LookupEditorBase.md#values)

### Methods

- [abortPendingQuery](corelib.LookupEditorBase.md#abortpendingquery)
- [addCssClass](corelib.LookupEditorBase.md#addcssclass)
- [addInplaceCreate](corelib.LookupEditorBase.md#addinplacecreate)
- [addItem](corelib.LookupEditorBase.md#additem)
- [addOption](corelib.LookupEditorBase.md#addoption)
- [addValidationRule](corelib.LookupEditorBase.md#addvalidationrule)
- [allowClear](corelib.LookupEditorBase.md#allowclear)
- [asyncSearch](corelib.LookupEditorBase.md#asyncsearch)
- [cascadeItems](corelib.LookupEditorBase.md#cascadeitems)
- [change](corelib.LookupEditorBase.md#change)
- [changeSelect2](corelib.LookupEditorBase.md#changeselect2)
- [clearItems](corelib.LookupEditorBase.md#clearitems)
- [createEditDialog](corelib.LookupEditorBase.md#createeditdialog)
- [destroy](corelib.LookupEditorBase.md#destroy)
- [editDialogDataChange](corelib.LookupEditorBase.md#editdialogdatachange)
- [emptyItemText](corelib.LookupEditorBase.md#emptyitemtext)
- [filterItems](corelib.LookupEditorBase.md#filteritems)
- [getCascadeFromValue](corelib.LookupEditorBase.md#getcascadefromvalue)
- [getCreateSearchChoice](corelib.LookupEditorBase.md#getcreatesearchchoice)
- [getCssClass](corelib.LookupEditorBase.md#getcssclass)
- [getDialogTypeKey](corelib.LookupEditorBase.md#getdialogtypekey)
- [getEditValue](corelib.LookupEditorBase.md#geteditvalue)
- [getGridField](corelib.LookupEditorBase.md#getgridfield)
- [getIdField](corelib.LookupEditorBase.md#getidfield)
- [getItemDisabled](corelib.LookupEditorBase.md#getitemdisabled)
- [getItemText](corelib.LookupEditorBase.md#getitemtext)
- [getItems](corelib.LookupEditorBase.md#getitems)
- [getLookup](corelib.LookupEditorBase.md#getlookup)
- [getLookupAsync](corelib.LookupEditorBase.md#getlookupasync)
- [getLookupKey](corelib.LookupEditorBase.md#getlookupkey)
- [getPageSize](corelib.LookupEditorBase.md#getpagesize)
- [getSelect2Options](corelib.LookupEditorBase.md#getselect2options)
- [getTextField](corelib.LookupEditorBase.md#gettextfield)
- [getTypeDelay](corelib.LookupEditorBase.md#gettypedelay)
- [get\_cascadeField](corelib.LookupEditorBase.md#get_cascadefield)
- [get\_cascadeFrom](corelib.LookupEditorBase.md#get_cascadefrom)
- [get\_cascadeValue](corelib.LookupEditorBase.md#get_cascadevalue)
- [get\_delimited](corelib.LookupEditorBase.md#get_delimited)
- [get\_filterField](corelib.LookupEditorBase.md#get_filterfield)
- [get\_filterValue](corelib.LookupEditorBase.md#get_filtervalue)
- [get\_itemByKey](corelib.LookupEditorBase.md#get_itembykey)
- [get\_items](corelib.LookupEditorBase.md#get_items)
- [get\_readOnly](corelib.LookupEditorBase.md#get_readonly)
- [get\_select2Container](corelib.LookupEditorBase.md#get_select2container)
- [get\_text](corelib.LookupEditorBase.md#get_text)
- [get\_value](corelib.LookupEditorBase.md#get_value)
- [get\_values](corelib.LookupEditorBase.md#get_values)
- [hasAsyncSource](corelib.LookupEditorBase.md#hasasyncsource)
- [init](corelib.LookupEditorBase.md#init)
- [initNewEntity](corelib.LookupEditorBase.md#initnewentity)
- [initialize](corelib.LookupEditorBase.md#initialize)
- [inplaceCreateClick](corelib.LookupEditorBase.md#inplacecreateclick)
- [isAutoComplete](corelib.LookupEditorBase.md#isautocomplete)
- [isMultiple](corelib.LookupEditorBase.md#ismultiple)
- [itemDisabled](corelib.LookupEditorBase.md#itemdisabled)
- [itemId](corelib.LookupEditorBase.md#itemid)
- [itemText](corelib.LookupEditorBase.md#itemtext)
- [mapItem](corelib.LookupEditorBase.md#mapitem)
- [mapItems](corelib.LookupEditorBase.md#mapitems)
- [renderContents](corelib.LookupEditorBase.md#rendercontents)
- [setCascadeFrom](corelib.LookupEditorBase.md#setcascadefrom)
- [setCreateTermOnNewEntity](corelib.LookupEditorBase.md#setcreatetermonnewentity)
- [setEditDialogReadOnly](corelib.LookupEditorBase.md#seteditdialogreadonly)
- [setEditValue](corelib.LookupEditorBase.md#seteditvalue)
- [setTermOnNewEntity](corelib.LookupEditorBase.md#settermonnewentity)
- [set\_cascadeField](corelib.LookupEditorBase.md#set_cascadefield)
- [set\_cascadeFrom](corelib.LookupEditorBase.md#set_cascadefrom)
- [set\_cascadeValue](corelib.LookupEditorBase.md#set_cascadevalue)
- [set\_filterField](corelib.LookupEditorBase.md#set_filterfield)
- [set\_filterValue](corelib.LookupEditorBase.md#set_filtervalue)
- [set\_readOnly](corelib.LookupEditorBase.md#set_readonly)
- [set\_value](corelib.LookupEditorBase.md#set_value)
- [set\_values](corelib.LookupEditorBase.md#set_values)
- [updateItems](corelib.LookupEditorBase.md#updateitems)
- [useInplaceAdd](corelib.LookupEditorBase.md#useinplaceadd)
- [create](corelib.LookupEditorBase.md#create)
- [elementFor](corelib.LookupEditorBase.md#elementfor)
- [filterByText](corelib.LookupEditorBase.md#filterbytext)
- [getWidgetName](corelib.LookupEditorBase.md#getwidgetname)

## Constructors

### constructor

• **new LookupEditorBase**<`TOptions`, `TItem`\>(`input`, `opt?`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TOptions` | extends [`LookupEditorOptions`](../interfaces/corelib.LookupEditorOptions.md) |
| `TItem` | `TItem` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `input` | `JQuery` |
| `opt?` | `TOptions` |

#### Overrides

[Select2Editor](corelib.Select2Editor.md).[constructor](corelib.Select2Editor.md#constructor)

#### Defined in

[src/ui/editors/lookupeditor.ts:13](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;13)

## Properties

### cascadeLink

• `Protected` **cascadeLink**: [`CascadedWidgetLink`](corelib.CascadedWidgetLink.md)<[`Widget`](corelib.Widget.md)<`any`\>\>

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[cascadeLink](corelib.Select2Editor.md#cascadelink)

#### Defined in

[src/ui/editors/select2editor.ts:701](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;701)

___

### element

• **element**: `JQuery`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[element](corelib.Select2Editor.md#element)

#### Defined in

[src/ui/widgets/widget.ts:61](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;61)

___

### idPrefix

• `Readonly` **idPrefix**: `string`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[idPrefix](corelib.Select2Editor.md#idprefix)

#### Defined in

[src/ui/widgets/widget.ts:65](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;65)

___

### lastCreateTerm

• `Protected` **lastCreateTerm**: `string`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[lastCreateTerm](corelib.Select2Editor.md#lastcreateterm)

#### Defined in

[src/ui/editors/select2editor.ts:64](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;64)

___

### lookup

• `Protected` **lookup**: [`Lookup`](corelib_q.Lookup.md)<`TItem`\>

#### Defined in

[src/ui/editors/lookupeditor.ts:56](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;56)

___

### onInitNewEntity

• **onInitNewEntity**: (`entity`: `TItem`) => `void`

#### Type declaration

▸ (`entity`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `entity` | `TItem` |

##### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[onInitNewEntity](corelib.Select2Editor.md#oninitnewentity)

#### Defined in

[src/ui/editors/select2editor.ts:871](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;871)

___

### openDialogAsPanel

• **openDialogAsPanel**: `boolean`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[openDialogAsPanel](corelib.Select2Editor.md#opendialogaspanel)

#### Defined in

[src/ui/editors/select2editor.ts:972](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;972)

___

### options

• `Protected` **options**: `TOptions`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[options](corelib.Select2Editor.md#options)

#### Defined in

[src/ui/widgets/widget.ts:62](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;62)

___

### uniqueName

• `Protected` **uniqueName**: `string`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[uniqueName](corelib.Select2Editor.md#uniquename)

#### Defined in

[src/ui/widgets/widget.ts:64](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;64)

___

### widgetName

• `Protected` **widgetName**: `string`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[widgetName](corelib.Select2Editor.md#widgetname)

#### Defined in

[src/ui/widgets/widget.ts:63](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;63)

## Accessors

### cascadeField

• `get` **cascadeField**(): `string`

#### Returns

`string`

#### Inherited from

Select2Editor.cascadeField

#### Defined in

[src/ui/editors/select2editor.ts:745](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;745)

• `set` **cascadeField**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Inherited from

Select2Editor.cascadeField

#### Defined in

[src/ui/editors/select2editor.ts:753](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;753)

___

### cascadeFrom

• `get` **cascadeFrom**(): `string`

#### Returns

`string`

#### Inherited from

Select2Editor.cascadeFrom

#### Defined in

[src/ui/editors/select2editor.ts:726](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;726)

• `set` **cascadeFrom**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Inherited from

Select2Editor.cascadeFrom

#### Defined in

[src/ui/editors/select2editor.ts:737](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;737)

___

### cascadeValue

• `get` **cascadeValue**(): `any`

#### Returns

`any`

#### Inherited from

Select2Editor.cascadeValue

#### Defined in

[src/ui/editors/select2editor.ts:761](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;761)

• `set` **cascadeValue**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `any` |

#### Returns

`void`

#### Inherited from

Select2Editor.cascadeValue

#### Defined in

[src/ui/editors/select2editor.ts:773](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;773)

___

### filterField

• `get` **filterField**(): `string`

#### Returns

`string`

#### Inherited from

Select2Editor.filterField

#### Defined in

[src/ui/editors/select2editor.ts:781](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;781)

• `set` **filterField**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Inherited from

Select2Editor.filterField

#### Defined in

[src/ui/editors/select2editor.ts:789](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;789)

___

### filterValue

• `get` **filterValue**(): `any`

#### Returns

`any`

#### Inherited from

Select2Editor.filterValue

#### Defined in

[src/ui/editors/select2editor.ts:797](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;797)

• `set` **filterValue**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `any` |

#### Returns

`void`

#### Inherited from

Select2Editor.filterValue

#### Defined in

[src/ui/editors/select2editor.ts:809](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;809)

___

### itemById

• `Protected` `get` **itemById**(): `Object`

#### Returns

`Object`

#### Inherited from

Select2Editor.itemById

#### Defined in

[src/ui/editors/select2editor.ts:349](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;349)

• `Protected` `set` **itemById**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `Object` |

#### Returns

`void`

#### Inherited from

Select2Editor.itemById

#### Defined in

[src/ui/editors/select2editor.ts:356](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;356)

___

### items

• `get` **items**(): `Select2Item`[]

#### Returns

`Select2Item`[]

#### Inherited from

Select2Editor.items

#### Defined in

[src/ui/editors/select2editor.ts:332](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;332)

• `set` **items**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `Select2Item`[] |

#### Returns

`void`

#### Inherited from

Select2Editor.items

#### Defined in

[src/ui/editors/select2editor.ts:339](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;339)

___

### readOnly

• `get` **readOnly**(): `boolean`

#### Returns

`boolean`

#### Inherited from

Select2Editor.readOnly

#### Defined in

[src/ui/editors/select2editor.ts:672](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;672)

• `set` **readOnly**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

Select2Editor.readOnly

#### Defined in

[src/ui/editors/select2editor.ts:693](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;693)

___

### selectedItem

• `get` **selectedItem**(): `TItem`

#### Returns

`TItem`

#### Inherited from

Select2Editor.selectedItem

#### Defined in

[src/ui/editors/select2editor.ts:598](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;598)

___

### selectedItems

• `get` **selectedItems**(): `TItem`[]

#### Returns

`TItem`[]

#### Inherited from

Select2Editor.selectedItems

#### Defined in

[src/ui/editors/select2editor.ts:608](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;608)

___

### text

• `get` **text**(): `string`

#### Returns

`string`

#### Inherited from

Select2Editor.text

#### Defined in

[src/ui/editors/select2editor.ts:664](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;664)

___

### value

• `get` **value**(): `string`

#### Returns

`string`

#### Inherited from

Select2Editor.value

#### Defined in

[src/ui/editors/select2editor.ts:565](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;565)

• `set` **value**(`v`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `v` | `string` |

#### Returns

`void`

#### Inherited from

Select2Editor.value

#### Defined in

[src/ui/editors/select2editor.ts:594](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;594)

___

### values

• `get` **values**(): `string`[]

#### Returns

`string`[]

#### Inherited from

Select2Editor.values

#### Defined in

[src/ui/editors/select2editor.ts:642](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;642)

• `set` **values**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string`[] |

#### Returns

`void`

#### Inherited from

Select2Editor.values

#### Defined in

[src/ui/editors/select2editor.ts:656](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;656)

## Methods

### abortPendingQuery

▸ `Protected` **abortPendingQuery**(): `void`

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[abortPendingQuery](corelib.Select2Editor.md#abortpendingquery)

#### Defined in

[src/ui/editors/select2editor.ts:175](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;175)

___

### addCssClass

▸ `Protected` **addCssClass**(): `void`

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[addCssClass](corelib.Select2Editor.md#addcssclass)

#### Defined in

[src/ui/widgets/widget.ts:100](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;100)

___

### addInplaceCreate

▸ `Protected` **addInplaceCreate**(`addTitle`, `editTitle`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `addTitle` | `string` |
| `editTitle` | `string` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[addInplaceCreate](corelib.Select2Editor.md#addinplacecreate)

#### Defined in

[src/ui/editors/select2editor.ts:388](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;388)

___

### addItem

▸ **addItem**(`item`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `item` | `Select2Item` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[addItem](corelib.Select2Editor.md#additem)

#### Defined in

[src/ui/editors/select2editor.ts:371](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;371)

___

### addOption

▸ **addOption**(`key`, `text`, `source?`, `disabled?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `key` | `string` |
| `text` | `string` |
| `source?` | `any` |
| `disabled?` | `boolean` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[addOption](corelib.Select2Editor.md#addoption)

#### Defined in

[src/ui/editors/select2editor.ts:379](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;379)

___

### addValidationRule

▸ **addValidationRule**(`eventClass`, `rule`): `JQuery`

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventClass` | `string` |
| `rule` | (`p1`: `JQuery`) => `string` |

#### Returns

`JQuery`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[addValidationRule](corelib.Select2Editor.md#addvalidationrule)

#### Defined in

[src/ui/widgets/widget.ts:134](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;134)

___

### allowClear

▸ `Protected` **allowClear**(): `boolean`

#### Returns

`boolean`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[allowClear](corelib.Select2Editor.md#allowclear)

#### Defined in

[src/ui/editors/select2editor.ts:162](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;162)

___

### asyncSearch

▸ `Protected` **asyncSearch**(`query`, `results`): [`Select2SearchPromise`](../interfaces/corelib.Select2SearchPromise.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `query` | [`Select2SearchQuery`](../interfaces/corelib.Select2SearchQuery.md) |
| `results` | (`result`: [`Select2SearchResult`](../interfaces/corelib.Select2SearchResult.md)<`TItem`\>) => `void` |

#### Returns

[`Select2SearchPromise`](../interfaces/corelib.Select2SearchPromise.md)

#### Overrides

[Select2Editor](corelib.Select2Editor.md).[asyncSearch](corelib.Select2Editor.md#asyncsearch)

#### Defined in

[src/ui/editors/lookupeditor.ts:106](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;106)

___

### cascadeItems

▸ `Protected` **cascadeItems**(`items`): `TItem`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `items` | `TItem`[] |

#### Returns

`TItem`[]

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[cascadeItems](corelib.Select2Editor.md#cascadeitems)

#### Defined in

[src/ui/editors/select2editor.ts:813](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;813)

___

### change

▸ **change**(`handler`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `handler` | (`e`: `JQueryEventObject`) => `void` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[change](corelib.Select2Editor.md#change)

#### Defined in

[src/ui/widgets/widget.ts:142](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;142)

▸ **change**(`handler`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `handler` | (`e`: `JQueryEventObject`) => `void` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[change](corelib.Select2Editor.md#change)

#### Defined in

[src/ui/widgets/widget.ts:259](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;259)

___

### changeSelect2

▸ **changeSelect2**(`handler`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `handler` | (`e`: `JQueryEventObject`) => `void` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[changeSelect2](corelib.Select2Editor.md#changeselect2)

#### Defined in

[src/ui/widgets/widget.ts:146](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;146)

▸ **changeSelect2**(`handler`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `handler` | (`e`: `JQueryEventObject`) => `void` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[changeSelect2](corelib.Select2Editor.md#changeselect2)

#### Defined in

[src/ui/widgets/widget.ts:260](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;260)

___

### clearItems

▸ **clearItems**(): `void`

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[clearItems](corelib.Select2Editor.md#clearitems)

#### Defined in

[src/ui/editors/select2editor.ts:363](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;363)

___

### createEditDialog

▸ `Protected` **createEditDialog**(`callback`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`dlg`: [`IEditDialog`](corelib.IEditDialog.md)) => `void` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[createEditDialog](corelib.Select2Editor.md#createeditdialog)

#### Defined in

[src/ui/editors/select2editor.ts:862](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;862)

___

### destroy

▸ **destroy**(): `void`

#### Returns

`void`

#### Overrides

[Select2Editor](corelib.Select2Editor.md).[destroy](corelib.Select2Editor.md#destroy)

#### Defined in

[src/ui/editors/lookupeditor.ts:30](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;30)

___

### editDialogDataChange

▸ `Protected` **editDialogDataChange**(): `void`

#### Returns

`void`

#### Overrides

[Select2Editor](corelib.Select2Editor.md).[editDialogDataChange](corelib.Select2Editor.md#editdialogdatachange)

#### Defined in

[src/ui/editors/lookupeditor.ts:141](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;141)

___

### emptyItemText

▸ `Protected` **emptyItemText**(): `string`

#### Returns

`string`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[emptyItemText](corelib.Select2Editor.md#emptyitemtext)

#### Defined in

[src/ui/editors/select2editor.ts:114](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;114)

___

### filterItems

▸ `Protected` **filterItems**(`items`): `TItem`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `items` | `TItem`[] |

#### Returns

`TItem`[]

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[filterItems](corelib.Select2Editor.md#filteritems)

#### Defined in

[src/ui/editors/select2editor.ts:835](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;835)

___

### getCascadeFromValue

▸ `Protected` **getCascadeFromValue**(`parent`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `parent` | [`Widget`](corelib.Widget.md)<`any`\> |

#### Returns

`any`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[getCascadeFromValue](corelib.Select2Editor.md#getcascadefromvalue)

#### Defined in

[src/ui/editors/select2editor.ts:697](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;697)

___

### getCreateSearchChoice

▸ **getCreateSearchChoice**(`getName`): (`s`: `string`) => { `id`: `string` ; `text`: `string`  }

#### Parameters

| Name | Type |
| :------ | :------ |
| `getName` | (`z`: `any`) => `string` |

#### Returns

`fn`

▸ (`s`): `Object`

##### Parameters

| Name | Type |
| :------ | :------ |
| `s` | `string` |

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `text` | `string` |

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[getCreateSearchChoice](corelib.Select2Editor.md#getcreatesearchchoice)

#### Defined in

[src/ui/editors/select2editor.ts:450](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;450)

___

### getCssClass

▸ `Protected` **getCssClass**(): `string`

#### Returns

`string`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[getCssClass](corelib.Select2Editor.md#getcssclass)

#### Defined in

[src/ui/widgets/widget.ts:104](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;104)

___

### getDialogTypeKey

▸ `Protected` **getDialogTypeKey**(): `string`

#### Returns

`string`

#### Overrides

[Select2Editor](corelib.Select2Editor.md).[getDialogTypeKey](corelib.Select2Editor.md#getdialogtypekey)

#### Defined in

[src/ui/editors/lookupeditor.ts:129](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;129)

___

### getEditValue

▸ **getEditValue**(`property`, `target`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `property` | [`PropertyItem`](../interfaces/corelib_q.PropertyItem.md) |
| `target` | `any` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[getEditValue](corelib.Select2Editor.md#geteditvalue)

#### Defined in

[src/ui/editors/select2editor.ts:508](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;508)

___

### getGridField

▸ **getGridField**(): `JQuery`

#### Returns

`JQuery`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[getGridField](corelib.Select2Editor.md#getgridfield)

#### Defined in

[src/ui/widgets/widget.ts:138](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;138)

___

### getIdField

▸ `Protected` **getIdField**(): `any`

#### Returns

`any`

#### Overrides

[Select2Editor](corelib.Select2Editor.md).[getIdField](corelib.Select2Editor.md#getidfield)

#### Defined in

[src/ui/editors/lookupeditor.ts:70](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;70)

___

### getItemDisabled

▸ `Protected` **getItemDisabled**(`item`, `lookup`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `item` | `TItem` |
| `lookup` | [`Lookup`](corelib_q.Lookup.md)<`TItem`\> |

#### Returns

`boolean`

#### Defined in

[src/ui/editors/lookupeditor.ts:91](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;91)

___

### getItemText

▸ `Protected` **getItemText**(`item`, `lookup`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `item` | `TItem` |
| `lookup` | [`Lookup`](corelib_q.Lookup.md)<`TItem`\> |

#### Returns

`any`

#### Defined in

[src/ui/editors/lookupeditor.ts:74](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;74)

___

### getItems

▸ `Protected` **getItems**(`lookup`): `TItem`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `lookup` | [`Lookup`](corelib_q.Lookup.md)<`TItem`\> |

#### Returns

`TItem`[]

#### Defined in

[src/ui/editors/lookupeditor.ts:66](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;66)

___

### getLookup

▸ `Protected` **getLookup**(): [`Lookup`](corelib_q.Lookup.md)<`TItem`\>

#### Returns

[`Lookup`](corelib_q.Lookup.md)<`TItem`\>

#### Defined in

[src/ui/editors/lookupeditor.ts:62](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;62)

___

### getLookupAsync

▸ `Protected` **getLookupAsync**(): `PromiseLike`<[`Lookup`](corelib_q.Lookup.md)<`TItem`\>\>

#### Returns

`PromiseLike`<[`Lookup`](corelib_q.Lookup.md)<`TItem`\>\>

#### Defined in

[src/ui/editors/lookupeditor.ts:58](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;58)

___

### getLookupKey

▸ `Protected` **getLookupKey**(): `string`

#### Returns

`string`

#### Defined in

[src/ui/editors/lookupeditor.ts:37](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;37)

___

### getPageSize

▸ `Protected` **getPageSize**(): `number`

#### Returns

`number`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[getPageSize](corelib.Select2Editor.md#getpagesize)

#### Defined in

[src/ui/editors/select2editor.ts:119](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;119)

___

### getSelect2Options

▸ `Protected` **getSelect2Options**(): `Select2Options`

#### Returns

`Select2Options`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[getSelect2Options](corelib.Select2Editor.md#getselect2options)

#### Defined in

[src/ui/editors/select2editor.ts:184](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;184)

___

### getTextField

▸ `Protected` **getTextField**(): `any`

#### Returns

`any`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[getTextField](corelib.Select2Editor.md#gettextfield)

#### Defined in

[src/ui/editors/select2editor.ts:134](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;134)

___

### getTypeDelay

▸ `Protected` **getTypeDelay**(): `any`

#### Returns

`any`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[getTypeDelay](corelib.Select2Editor.md#gettypedelay)

#### Defined in

[src/ui/editors/select2editor.ts:110](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;110)

___

### get\_cascadeField

▸ `Protected` **get_cascadeField**(): `string`

#### Returns

`string`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[get_cascadeField](corelib.Select2Editor.md#get_cascadefield)

#### Defined in

[src/ui/editors/select2editor.ts:741](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;741)

___

### get\_cascadeFrom

▸ `Protected` **get_cascadeFrom**(): `string`

#### Returns

`string`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[get_cascadeFrom](corelib.Select2Editor.md#get_cascadefrom)

#### Defined in

[src/ui/editors/select2editor.ts:722](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;722)

___

### get\_cascadeValue

▸ `Protected` **get_cascadeValue**(): `any`

#### Returns

`any`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[get_cascadeValue](corelib.Select2Editor.md#get_cascadevalue)

#### Defined in

[src/ui/editors/select2editor.ts:757](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;757)

___

### get\_delimited

▸ **get_delimited**(): `boolean`

#### Returns

`boolean`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[get_delimited](corelib.Select2Editor.md#get_delimited)

#### Defined in

[src/ui/editors/select2editor.ts:328](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;328)

___

### get\_filterField

▸ `Protected` **get_filterField**(): `string`

#### Returns

`string`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[get_filterField](corelib.Select2Editor.md#get_filterfield)

#### Defined in

[src/ui/editors/select2editor.ts:777](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;777)

___

### get\_filterValue

▸ `Protected` **get_filterValue**(): `any`

#### Returns

`any`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[get_filterValue](corelib.Select2Editor.md#get_filtervalue)

#### Defined in

[src/ui/editors/select2editor.ts:793](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;793)

___

### get\_itemByKey

▸ `Protected` **get_itemByKey**(): `Object`

#### Returns

`Object`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[get_itemByKey](corelib.Select2Editor.md#get_itembykey)

#### Defined in

[src/ui/editors/select2editor.ts:525](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;525)

___

### get\_items

▸ `Protected` **get_items**(): `Select2Item`[]

#### Returns

`Select2Item`[]

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[get_items](corelib.Select2Editor.md#get_items)

#### Defined in

[src/ui/editors/select2editor.ts:521](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;521)

___

### get\_readOnly

▸ **get_readOnly**(): `boolean`

#### Returns

`boolean`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[get_readOnly](corelib.Select2Editor.md#get_readonly)

#### Defined in

[src/ui/editors/select2editor.ts:668](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;668)

___

### get\_select2Container

▸ `Protected` **get_select2Container**(): `JQuery`

#### Returns

`JQuery`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[get_select2Container](corelib.Select2Editor.md#get_select2container)

#### Defined in

[src/ui/editors/select2editor.ts:517](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;517)

___

### get\_text

▸ `Protected` **get_text**(): `string`

#### Returns

`string`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[get_text](corelib.Select2Editor.md#get_text)

#### Defined in

[src/ui/editors/select2editor.ts:660](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;660)

___

### get\_value

▸ **get_value**(): `any`

#### Returns

`any`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[get_value](corelib.Select2Editor.md#get_value)

#### Defined in

[src/ui/editors/select2editor.ts:551](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;551)

___

### get\_values

▸ `Protected` **get_values**(): `string`[]

#### Returns

`string`[]

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[get_values](corelib.Select2Editor.md#get_values)

#### Defined in

[src/ui/editors/select2editor.ts:623](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;623)

___

### hasAsyncSource

▸ **hasAsyncSource**(): `boolean`

#### Returns

`boolean`

#### Overrides

[Select2Editor](corelib.Select2Editor.md).[hasAsyncSource](corelib.Select2Editor.md#hasasyncsource)

#### Defined in

[src/ui/editors/lookupeditor.ts:26](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;26)

___

### init

▸ **init**(`action?`): [`LookupEditorBase`](corelib.LookupEditorBase.md)<`TOptions`, `TItem`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `action?` | (`widget`: `any`) => `void` |

#### Returns

[`LookupEditorBase`](corelib.LookupEditorBase.md)<`TOptions`, `TItem`\>

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[init](corelib.Select2Editor.md#init)

#### Defined in

[src/ui/widgets/widget.ts:179](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;179)

___

### initNewEntity

▸ `Protected` **initNewEntity**(`entity`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `entity` | `TItem` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[initNewEntity](corelib.Select2Editor.md#initnewentity)

#### Defined in

[src/ui/editors/select2editor.ts:873](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;873)

___

### initialize

▸ **initialize**(): `void`

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[initialize](corelib.Select2Editor.md#initialize)

#### Defined in

[src/ui/widgets/widget.ts:176](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;176)

___

### inplaceCreateClick

▸ `Protected` **inplaceCreateClick**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `JQueryEventObject` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[inplaceCreateClick](corelib.Select2Editor.md#inplacecreateclick)

#### Defined in

[src/ui/editors/select2editor.ts:901](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;901)

___

### isAutoComplete

▸ `Protected` **isAutoComplete**(): `boolean`

#### Returns

`boolean`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[isAutoComplete](corelib.Select2Editor.md#isautocomplete)

#### Defined in

[src/ui/editors/select2editor.ts:446](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;446)

___

### isMultiple

▸ `Protected` **isMultiple**(): `boolean`

#### Returns

`boolean`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[isMultiple](corelib.Select2Editor.md#ismultiple)

#### Defined in

[src/ui/editors/select2editor.ts:167](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;167)

___

### itemDisabled

▸ `Protected` **itemDisabled**(`item`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `item` | `TItem` |

#### Returns

`boolean`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[itemDisabled](corelib.Select2Editor.md#itemdisabled)

#### Defined in

[src/ui/editors/select2editor.ts:145](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;145)

___

### itemId

▸ `Protected` **itemId**(`item`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `item` | `TItem` |

#### Returns

`string`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[itemId](corelib.Select2Editor.md#itemid)

#### Defined in

[src/ui/editors/select2editor.ts:127](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;127)

___

### itemText

▸ `Protected` **itemText**(`item`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `item` | `TItem` |

#### Returns

`string`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[itemText](corelib.Select2Editor.md#itemtext)

#### Defined in

[src/ui/editors/select2editor.ts:138](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;138)

___

### mapItem

▸ `Protected` **mapItem**(`item`): `Select2Item`

#### Parameters

| Name | Type |
| :------ | :------ |
| `item` | `TItem` |

#### Returns

`Select2Item`

#### Overrides

[Select2Editor](corelib.Select2Editor.md).[mapItem](corelib.Select2Editor.md#mapitem)

#### Defined in

[src/ui/editors/lookupeditor.ts:82](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;82)

___

### mapItems

▸ `Protected` **mapItems**(`items`): `Select2Item`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `items` | `TItem`[] |

#### Returns

`Select2Item`[]

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[mapItems](corelib.Select2Editor.md#mapitems)

#### Defined in

[src/ui/editors/select2editor.ts:158](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;158)

___

### renderContents

▸ `Protected` **renderContents**(): `void`

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[renderContents](corelib.Select2Editor.md#rendercontents)

#### Defined in

[src/ui/widgets/widget.ts:184](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;184)

___

### setCascadeFrom

▸ `Protected` **setCascadeFrom**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[setCascadeFrom](corelib.Select2Editor.md#setcascadefrom)

#### Defined in

[src/ui/editors/select2editor.ts:703](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;703)

___

### setCreateTermOnNewEntity

▸ `Protected` **setCreateTermOnNewEntity**(`entity`, `term`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `entity` | `TItem` |
| `term` | `string` |

#### Returns

`void`

#### Defined in

[src/ui/editors/lookupeditor.ts:137](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;137)

___

### setEditDialogReadOnly

▸ `Protected` **setEditDialogReadOnly**(`dialog`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `dialog` | `any` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[setEditDialogReadOnly](corelib.Select2Editor.md#seteditdialogreadonly)

#### Defined in

[src/ui/editors/select2editor.ts:887](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;887)

___

### setEditValue

▸ **setEditValue**(`source`, `property`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `source` | `any` |
| `property` | [`PropertyItem`](../interfaces/corelib_q.PropertyItem.md) |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[setEditValue](corelib.Select2Editor.md#seteditvalue)

#### Defined in

[src/ui/editors/select2editor.ts:498](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;498)

___

### setTermOnNewEntity

▸ `Protected` **setTermOnNewEntity**(`entity`, `term`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `entity` | `TItem` |
| `term` | `string` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[setTermOnNewEntity](corelib.Select2Editor.md#settermonnewentity)

#### Defined in

[src/ui/editors/select2editor.ts:898](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;898)

___

### set\_cascadeField

▸ `Protected` **set_cascadeField**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[set_cascadeField](corelib.Select2Editor.md#set_cascadefield)

#### Defined in

[src/ui/editors/select2editor.ts:749](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;749)

___

### set\_cascadeFrom

▸ `Protected` **set_cascadeFrom**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[set_cascadeFrom](corelib.Select2Editor.md#set_cascadefrom)

#### Defined in

[src/ui/editors/select2editor.ts:730](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;730)

___

### set\_cascadeValue

▸ `Protected` **set_cascadeValue**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `any` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[set_cascadeValue](corelib.Select2Editor.md#set_cascadevalue)

#### Defined in

[src/ui/editors/select2editor.ts:765](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;765)

___

### set\_filterField

▸ `Protected` **set_filterField**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[set_filterField](corelib.Select2Editor.md#set_filterfield)

#### Defined in

[src/ui/editors/select2editor.ts:785](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;785)

___

### set\_filterValue

▸ `Protected` **set_filterValue**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `any` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[set_filterValue](corelib.Select2Editor.md#set_filtervalue)

#### Defined in

[src/ui/editors/select2editor.ts:801](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;801)

___

### set\_readOnly

▸ **set_readOnly**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[set_readOnly](corelib.Select2Editor.md#set_readonly)

#### Defined in

[src/ui/editors/select2editor.ts:686](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;686)

___

### set\_value

▸ **set_value**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[set_value](corelib.Select2Editor.md#set_value)

#### Defined in

[src/ui/editors/select2editor.ts:569](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;569)

___

### set\_values

▸ `Protected` **set_values**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string`[] |

#### Returns

`void`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[set_values](corelib.Select2Editor.md#set_values)

#### Defined in

[src/ui/editors/select2editor.ts:646](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;646)

___

### updateItems

▸ **updateItems**(): `void`

#### Returns

`void`

#### Overrides

[Select2Editor](corelib.Select2Editor.md).[updateItems](corelib.Select2Editor.md#updateitems)

#### Defined in

[src/ui/editors/lookupeditor.ts:95](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/lookupeditor.ts#line&#x3D;95)

___

### useInplaceAdd

▸ `Protected` **useInplaceAdd**(): `boolean`

#### Returns

`boolean`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[useInplaceAdd](corelib.Select2Editor.md#useinplaceadd)

#### Defined in

[src/ui/editors/select2editor.ts:439](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;439)

___

### create

▸ `Static` **create**<`TWidget`, `TOpt`\>(`params`): `TWidget`

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TWidget` | extends [`Widget`](corelib.Widget.md)<`TOpt`, `TWidget`\> |
| `TOpt` | `TOpt` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `params` | [`CreateWidgetParams`](../interfaces/corelib.CreateWidgetParams.md)<`TWidget`, `TOpt`\> |

#### Returns

`TWidget`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[create](corelib.Select2Editor.md#create)

#### Defined in

[src/ui/widgets/widget.ts:153](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;153)

___

### elementFor

▸ `Static` **elementFor**<`TWidget`\>(`editorType`): `JQuery`

#### Type parameters

| Name |
| :------ |
| `TWidget` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `editorType` | (...`args`: `any`[]) => `TWidget` |

#### Returns

`JQuery`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[elementFor](corelib.Select2Editor.md#elementfor)

#### Defined in

[src/ui/widgets/widget.ts:128](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;128)

___

### filterByText

▸ `Static` **filterByText**<`TItem`\>(`items`, `getText`, `term`): `TItem`[]

#### Type parameters

| Name |
| :------ |
| `TItem` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `items` | `TItem`[] |
| `getText` | (`item`: `TItem`) => `string` |
| `term` | `string` |

#### Returns

`TItem`[]

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[filterByText](corelib.Select2Editor.md#filterbytext)

#### Defined in

[src/ui/editors/select2editor.ts:529](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/select2editor.ts#line&#x3D;529)

___

### getWidgetName

▸ `Static` **getWidgetName**(`type`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | `Function` |

#### Returns

`string`

#### Inherited from

[Select2Editor](corelib.Select2Editor.md).[getWidgetName](corelib.Select2Editor.md#getwidgetname)

#### Defined in

[src/ui/widgets/widget.ts:124](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;124)