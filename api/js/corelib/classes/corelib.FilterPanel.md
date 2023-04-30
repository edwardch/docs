[@serenity-is](../README.md) / [Modules](../modules.md) / [corelib](../modules/corelib.md) / FilterPanel

# Class: FilterPanel

[corelib](../modules/corelib.md).FilterPanel

## Hierarchy

- [`FilterWidgetBase`](corelib.FilterWidgetBase.md)<`any`\>

  ↳ **`FilterPanel`**

## Table of contents

### Constructors

- [constructor](corelib.FilterPanel.md#constructor)

### Properties

- [element](corelib.FilterPanel.md#element)
- [idPrefix](corelib.FilterPanel.md#idprefix)
- [options](corelib.FilterPanel.md#options)
- [rowsDiv](corelib.FilterPanel.md#rowsdiv)
- [showInitialLine](corelib.FilterPanel.md#showinitialline)
- [showSearchButton](corelib.FilterPanel.md#showsearchbutton)
- [uniqueName](corelib.FilterPanel.md#uniquename)
- [updateStoreOnReset](corelib.FilterPanel.md#updatestoreonreset)
- [widgetName](corelib.FilterPanel.md#widgetname)

### Methods

- [addButtonClick](corelib.FilterPanel.md#addbuttonclick)
- [addCssClass](corelib.FilterPanel.md#addcssclass)
- [addEmptyRow](corelib.FilterPanel.md#addemptyrow)
- [addValidationRule](corelib.FilterPanel.md#addvalidationrule)
- [andOrClick](corelib.FilterPanel.md#andorclick)
- [byId](corelib.FilterPanel.md#byid)
- [change](corelib.FilterPanel.md#change)
- [changeSelect2](corelib.FilterPanel.md#changeselect2)
- [deleteRowClick](corelib.FilterPanel.md#deleterowclick)
- [destroy](corelib.FilterPanel.md#destroy)
- [filterStoreChanged](corelib.FilterPanel.md#filterstorechanged)
- [findEmptyRow](corelib.FilterPanel.md#findemptyrow)
- [getCssClass](corelib.FilterPanel.md#getcssclass)
- [getFallbackTemplate](corelib.FilterPanel.md#getfallbacktemplate)
- [getFieldFor](corelib.FilterPanel.md#getfieldfor)
- [getFilteringFor](corelib.FilterPanel.md#getfilteringfor)
- [getGridField](corelib.FilterPanel.md#getgridfield)
- [getTemplate](corelib.FilterPanel.md#gettemplate)
- [getTemplateName](corelib.FilterPanel.md#gettemplatename)
- [get\_hasErrors](corelib.FilterPanel.md#get_haserrors)
- [get\_showInitialLine](corelib.FilterPanel.md#get_showinitialline)
- [get\_showSearchButton](corelib.FilterPanel.md#get_showsearchbutton)
- [get\_store](corelib.FilterPanel.md#get_store)
- [get\_updateStoreOnReset](corelib.FilterPanel.md#get_updatestoreonreset)
- [init](corelib.FilterPanel.md#init)
- [initButtons](corelib.FilterPanel.md#initbuttons)
- [initialize](corelib.FilterPanel.md#initialize)
- [leftRightParenClick](corelib.FilterPanel.md#leftrightparenclick)
- [onRowFieldChange](corelib.FilterPanel.md#onrowfieldchange)
- [onRowOperatorChange](corelib.FilterPanel.md#onrowoperatorchange)
- [populateOperatorList](corelib.FilterPanel.md#populateoperatorlist)
- [removeFiltering](corelib.FilterPanel.md#removefiltering)
- [renderContents](corelib.FilterPanel.md#rendercontents)
- [resetButtonClick](corelib.FilterPanel.md#resetbuttonclick)
- [rowFieldChange](corelib.FilterPanel.md#rowfieldchange)
- [rowOperatorChange](corelib.FilterPanel.md#rowoperatorchange)
- [search](corelib.FilterPanel.md#search)
- [searchButtonClick](corelib.FilterPanel.md#searchbuttonclick)
- [set\_showInitialLine](corelib.FilterPanel.md#set_showinitialline)
- [set\_showSearchButton](corelib.FilterPanel.md#set_showsearchbutton)
- [set\_store](corelib.FilterPanel.md#set_store)
- [set\_updateStoreOnReset](corelib.FilterPanel.md#set_updatestoreonreset)
- [updateButtons](corelib.FilterPanel.md#updatebuttons)
- [updateParens](corelib.FilterPanel.md#updateparens)
- [updateRowsFromStore](corelib.FilterPanel.md#updaterowsfromstore)
- [useIdPrefix](corelib.FilterPanel.md#useidprefix)
- [create](corelib.FilterPanel.md#create)
- [elementFor](corelib.FilterPanel.md#elementfor)
- [getWidgetName](corelib.FilterPanel.md#getwidgetname)

## Constructors

### constructor

• **new FilterPanel**(`div`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `div` | `JQuery` |

#### Overrides

[FilterWidgetBase](corelib.FilterWidgetBase.md).[constructor](corelib.FilterWidgetBase.md#constructor)

#### Defined in

[src/ui/filtering/filterpanel.ts:67](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;67)

## Properties

### element

• **element**: `JQuery`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[element](corelib.FilterWidgetBase.md#element)

#### Defined in

[src/ui/widgets/widget.ts:61](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;61)

___

### idPrefix

• `Readonly` **idPrefix**: `string`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[idPrefix](corelib.FilterWidgetBase.md#idprefix)

#### Defined in

[src/ui/widgets/widget.ts:65](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;65)

___

### options

• `Protected` **options**: `any`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[options](corelib.FilterWidgetBase.md#options)

#### Defined in

[src/ui/widgets/widget.ts:62](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;62)

___

### rowsDiv

• `Private` **rowsDiv**: `JQuery`

#### Defined in

[src/ui/filtering/filterpanel.ts:65](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;65)

___

### showInitialLine

• `Private` **showInitialLine**: `boolean`

#### Defined in

[src/ui/filtering/filterpanel.ts:76](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;76)

___

### showSearchButton

• `Private` **showSearchButton**: `boolean`

#### Defined in

[src/ui/filtering/filterpanel.ts:137](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;137)

___

### uniqueName

• `Protected` **uniqueName**: `string`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[uniqueName](corelib.FilterWidgetBase.md#uniquename)

#### Defined in

[src/ui/widgets/widget.ts:64](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;64)

___

### updateStoreOnReset

• `Private` **updateStoreOnReset**: `boolean`

#### Defined in

[src/ui/filtering/filterpanel.ts:150](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;150)

___

### widgetName

• `Protected` **widgetName**: `string`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[widgetName](corelib.FilterWidgetBase.md#widgetname)

#### Defined in

[src/ui/widgets/widget.ts:63](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;63)

## Methods

### addButtonClick

▸ `Protected` **addButtonClick**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `JQueryEventObject` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:249](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;249)

___

### addCssClass

▸ `Protected` **addCssClass**(): `void`

#### Returns

`void`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[addCssClass](corelib.FilterWidgetBase.md#addcssclass)

#### Defined in

[src/ui/widgets/widget.ts:100](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;100)

___

### addEmptyRow

▸ `Protected` **addEmptyRow**(`popupField`): `JQuery`

#### Parameters

| Name | Type |
| :------ | :------ |
| `popupField` | `boolean` |

#### Returns

`JQuery`

#### Defined in

[src/ui/filtering/filterpanel.ts:291](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;291)

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

[FilterWidgetBase](corelib.FilterWidgetBase.md).[addValidationRule](corelib.FilterWidgetBase.md#addvalidationrule)

#### Defined in

[src/ui/widgets/widget.ts:134](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;134)

___

### andOrClick

▸ `Protected` **andOrClick**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `JQueryEventObject` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:494](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;494)

___

### byId

▸ `Protected` **byId**(`id`): `JQuery`

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |

#### Returns

`JQuery`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[byId](corelib.FilterWidgetBase.md#byid)

#### Defined in

[src/ui/widgets/templatedwidget.ts:10](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/templatedwidget.ts#line&#x3D;10)

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

[FilterWidgetBase](corelib.FilterWidgetBase.md).[change](corelib.FilterWidgetBase.md#change)

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

[FilterWidgetBase](corelib.FilterWidgetBase.md).[change](corelib.FilterWidgetBase.md#change)

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

[FilterWidgetBase](corelib.FilterWidgetBase.md).[changeSelect2](corelib.FilterWidgetBase.md#changeselect2)

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

[FilterWidgetBase](corelib.FilterWidgetBase.md).[changeSelect2](corelib.FilterWidgetBase.md#changeselect2)

#### Defined in

[src/ui/widgets/widget.ts:260](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;260)

___

### deleteRowClick

▸ `Protected` **deleteRowClick**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `JQueryEventObject` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:474](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;474)

___

### destroy

▸ **destroy**(): `void`

#### Returns

`void`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[destroy](corelib.FilterWidgetBase.md#destroy)

#### Defined in

[src/ui/filtering/filterwidgetbase.ts:19](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterwidgetbase.ts#line&#x3D;19)

___

### filterStoreChanged

▸ `Protected` **filterStoreChanged**(): `void`

#### Returns

`void`

#### Overrides

[FilterWidgetBase](corelib.FilterWidgetBase.md).[filterStoreChanged](corelib.FilterWidgetBase.md#filterstorechanged)

#### Defined in

[src/ui/filtering/filterpanel.ts:91](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;91)

___

### findEmptyRow

▸ `Protected` **findEmptyRow**(): `JQuery`

#### Returns

`JQuery`

#### Defined in

[src/ui/filtering/filterpanel.ts:271](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;271)

___

### getCssClass

▸ `Protected` **getCssClass**(): `string`

#### Returns

`string`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[getCssClass](corelib.FilterWidgetBase.md#getcssclass)

#### Defined in

[src/ui/widgets/widget.ts:104](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;104)

___

### getFallbackTemplate

▸ `Protected` **getFallbackTemplate**(): `string`

#### Returns

`string`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[getFallbackTemplate](corelib.FilterWidgetBase.md#getfallbacktemplate)

#### Defined in

[src/ui/widgets/templatedwidget.ts:79](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/templatedwidget.ts#line&#x3D;79)

___

### getFieldFor

▸ `Protected` **getFieldFor**(`row`): [`PropertyItem`](../interfaces/corelib_q.PropertyItem.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `JQuery` |

#### Returns

[`PropertyItem`](../interfaces/corelib_q.PropertyItem.md)

#### Defined in

[src/ui/filtering/filterpanel.ts:396](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;396)

___

### getFilteringFor

▸ `Protected` **getFilteringFor**(`row`): [`IFiltering`](corelib.IFiltering.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `JQuery` |

#### Returns

[`IFiltering`](corelib.IFiltering.md)

#### Defined in

[src/ui/filtering/filterpanel.ts:410](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;410)

___

### getGridField

▸ **getGridField**(): `JQuery`

#### Returns

`JQuery`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[getGridField](corelib.FilterWidgetBase.md#getgridfield)

#### Defined in

[src/ui/widgets/widget.ts:138](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;138)

___

### getTemplate

▸ `Protected` **getTemplate**(): `string`

#### Returns

`string`

#### Overrides

[FilterWidgetBase](corelib.FilterWidgetBase.md).[getTemplate](corelib.FilterWidgetBase.md#gettemplate)

#### Defined in

[src/ui/filtering/filterpanel.ts:162](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;162)

___

### getTemplateName

▸ `Protected` **getTemplateName**(): `string`

#### Returns

`string`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[getTemplateName](corelib.FilterWidgetBase.md#gettemplatename)

#### Defined in

[src/ui/widgets/templatedwidget.ts:31](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/templatedwidget.ts#line&#x3D;31)

___

### get\_hasErrors

▸ **get_hasErrors**(): `boolean`

#### Returns

`boolean`

#### Defined in

[src/ui/filtering/filterpanel.ts:190](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;190)

___

### get\_showInitialLine

▸ **get_showInitialLine**(): `boolean`

#### Returns

`boolean`

#### Defined in

[src/ui/filtering/filterpanel.ts:78](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;78)

___

### get\_showSearchButton

▸ **get_showSearchButton**(): `boolean`

#### Returns

`boolean`

#### Defined in

[src/ui/filtering/filterpanel.ts:139](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;139)

___

### get\_store

▸ **get_store**(): [`FilterStore`](corelib.FilterStore.md)

#### Returns

[`FilterStore`](corelib.FilterStore.md)

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[get_store](corelib.FilterWidgetBase.md#get_store)

#### Defined in

[src/ui/filtering/filterwidgetbase.ts:33](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterwidgetbase.ts#line&#x3D;33)

___

### get\_updateStoreOnReset

▸ **get_updateStoreOnReset**(): `boolean`

#### Returns

`boolean`

#### Defined in

[src/ui/filtering/filterpanel.ts:152](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;152)

___

### init

▸ **init**(`action?`): [`FilterPanel`](corelib.FilterPanel.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `action?` | (`widget`: `any`) => `void` |

#### Returns

[`FilterPanel`](corelib.FilterPanel.md)

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[init](corelib.FilterWidgetBase.md#init)

#### Defined in

[src/ui/widgets/widget.ts:179](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;179)

___

### initButtons

▸ `Protected` **initButtons**(): `void`

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:174](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;174)

___

### initialize

▸ **initialize**(): `void`

#### Returns

`void`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[initialize](corelib.FilterWidgetBase.md#initialize)

#### Defined in

[src/ui/widgets/widget.ts:176](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;176)

___

### leftRightParenClick

▸ `Protected` **leftRightParenClick**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `JQueryEventObject` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:501](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;501)

___

### onRowFieldChange

▸ `Protected` **onRowFieldChange**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `JQueryEventObject` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:356](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;356)

___

### onRowOperatorChange

▸ `Protected` **onRowOperatorChange**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `JQueryEventObject` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:433](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;433)

___

### populateOperatorList

▸ `Protected` **populateOperatorList**(`row`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `JQuery` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:381](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;381)

___

### removeFiltering

▸ `Protected` **removeFiltering**(`row`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `JQuery` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:376](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;376)

___

### renderContents

▸ `Protected` **renderContents**(): `void`

#### Returns

`void`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[renderContents](corelib.FilterWidgetBase.md#rendercontents)

#### Defined in

[src/ui/widgets/templatedwidget.ts:110](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/templatedwidget.ts#line&#x3D;110)

___

### resetButtonClick

▸ `Protected` **resetButtonClick**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `JQueryEventObject` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:254](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;254)

___

### rowFieldChange

▸ `Protected` **rowFieldChange**(`row`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `JQuery` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:363](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;363)

___

### rowOperatorChange

▸ `Protected` **rowOperatorChange**(`row`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `JQuery` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:444](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;444)

___

### search

▸ **search**(): `void`

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:195](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;195)

___

### searchButtonClick

▸ `Protected` **searchButtonClick**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `JQueryEventObject` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:185](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;185)

___

### set\_showInitialLine

▸ **set_showInitialLine**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:82](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;82)

___

### set\_showSearchButton

▸ **set_showSearchButton**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:143](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;143)

___

### set\_store

▸ **set_store**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`FilterStore`](corelib.FilterStore.md) |

#### Returns

`void`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[set_store](corelib.FilterWidgetBase.md#set_store)

#### Defined in

[src/ui/filtering/filterwidgetbase.ts:37](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterwidgetbase.ts#line&#x3D;37)

___

### set\_updateStoreOnReset

▸ **set_updateStoreOnReset**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:156](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;156)

___

### updateButtons

▸ `Protected` **updateButtons**(): `void`

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:487](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;487)

___

### updateParens

▸ `Protected` **updateParens**(): `void`

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:507](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;507)

___

### updateRowsFromStore

▸ **updateRowsFromStore**(): `void`

#### Returns

`void`

#### Defined in

[src/ui/filtering/filterpanel.ts:96](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/filtering/filterpanel.ts#line&#x3D;96)

___

### useIdPrefix

▸ `Protected` **useIdPrefix**(): `IdPrefixType`

#### Returns

`IdPrefixType`

#### Inherited from

[FilterWidgetBase](corelib.FilterWidgetBase.md).[useIdPrefix](corelib.FilterWidgetBase.md#useidprefix)

#### Defined in

[src/ui/widgets/templatedwidget.ts:131](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/templatedwidget.ts#line&#x3D;131)

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

[FilterWidgetBase](corelib.FilterWidgetBase.md).[create](corelib.FilterWidgetBase.md#create)

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

[FilterWidgetBase](corelib.FilterWidgetBase.md).[elementFor](corelib.FilterWidgetBase.md#elementfor)

#### Defined in

[src/ui/widgets/widget.ts:128](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;128)

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

[FilterWidgetBase](corelib.FilterWidgetBase.md).[getWidgetName](corelib.FilterWidgetBase.md#getwidgetname)

#### Defined in

[src/ui/widgets/widget.ts:124](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;124)