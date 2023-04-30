[@serenity-is](../README.md) / [Modules](../modules.md) / [corelib](../modules/corelib.md) / [Reporting](../modules/corelib.Reporting.md) / ReportDialog

# Class: ReportDialog

[corelib](../modules/corelib.md).[Reporting](../modules/corelib.Reporting.md).ReportDialog

## Hierarchy

- [`TemplatedDialog`](corelib.TemplatedDialog.md)<[`ReportDialogOptions`](../interfaces/corelib.Reporting.ReportDialogOptions.md)\>

  ↳ **`ReportDialog`**

## Table of contents

### Constructors

- [constructor](corelib.Reporting.ReportDialog.md#constructor)

### Properties

- [element](corelib.Reporting.ReportDialog.md#element)
- [idPrefix](corelib.Reporting.ReportDialog.md#idprefix)
- [options](corelib.Reporting.ReportDialog.md#options)
- [propertyGrid](corelib.Reporting.ReportDialog.md#propertygrid)
- [propertyItems](corelib.Reporting.ReportDialog.md#propertyitems)
- [reportKey](corelib.Reporting.ReportDialog.md#reportkey)
- [tabs](corelib.Reporting.ReportDialog.md#tabs)
- [toolbar](corelib.Reporting.ReportDialog.md#toolbar)
- [uniqueName](corelib.Reporting.ReportDialog.md#uniquename)
- [validator](corelib.Reporting.ReportDialog.md#validator)
- [widgetName](corelib.Reporting.ReportDialog.md#widgetname)
- [bootstrapModal](corelib.Reporting.ReportDialog.md#bootstrapmodal)

### Accessors

- [dialogTitle](corelib.Reporting.ReportDialog.md#dialogtitle)
- [isMarkedAsPanel](corelib.Reporting.ReportDialog.md#ismarkedaspanel)
- [isResponsive](corelib.Reporting.ReportDialog.md#isresponsive)

### Methods

- [addCssClass](corelib.Reporting.ReportDialog.md#addcssclass)
- [addValidationRule](corelib.Reporting.ReportDialog.md#addvalidationrule)
- [arrange](corelib.Reporting.ReportDialog.md#arrange)
- [byId](corelib.Reporting.ReportDialog.md#byid)
- [change](corelib.Reporting.ReportDialog.md#change)
- [changeSelect2](corelib.Reporting.ReportDialog.md#changeselect2)
- [createPropertyGrid](corelib.Reporting.ReportDialog.md#createpropertygrid)
- [destroy](corelib.Reporting.ReportDialog.md#destroy)
- [dialogClose](corelib.Reporting.ReportDialog.md#dialogclose)
- [dialogOpen](corelib.Reporting.ReportDialog.md#dialogopen)
- [executeReport](corelib.Reporting.ReportDialog.md#executereport)
- [getCssClass](corelib.Reporting.ReportDialog.md#getcssclass)
- [getDialogButtons](corelib.Reporting.ReportDialog.md#getdialogbuttons)
- [getDialogOptions](corelib.Reporting.ReportDialog.md#getdialogoptions)
- [getDialogTitle](corelib.Reporting.ReportDialog.md#getdialogtitle)
- [getFallbackTemplate](corelib.Reporting.ReportDialog.md#getfallbacktemplate)
- [getGridField](corelib.Reporting.ReportDialog.md#getgridfield)
- [getModalOptions](corelib.Reporting.ReportDialog.md#getmodaloptions)
- [getTemplate](corelib.Reporting.ReportDialog.md#gettemplate)
- [getTemplateName](corelib.Reporting.ReportDialog.md#gettemplatename)
- [getToolbarButtons](corelib.Reporting.ReportDialog.md#gettoolbarbuttons)
- [getValidatorOptions](corelib.Reporting.ReportDialog.md#getvalidatoroptions)
- [handleResponsive](corelib.Reporting.ReportDialog.md#handleresponsive)
- [init](corelib.Reporting.ReportDialog.md#init)
- [initDialog](corelib.Reporting.ReportDialog.md#initdialog)
- [initModal](corelib.Reporting.ReportDialog.md#initmodal)
- [initTabs](corelib.Reporting.ReportDialog.md#inittabs)
- [initToolbar](corelib.Reporting.ReportDialog.md#inittoolbar)
- [initValidator](corelib.Reporting.ReportDialog.md#initvalidator)
- [initialize](corelib.Reporting.ReportDialog.md#initialize)
- [loadReport](corelib.Reporting.ReportDialog.md#loadreport)
- [onDialogClose](corelib.Reporting.ReportDialog.md#ondialogclose)
- [onDialogOpen](corelib.Reporting.ReportDialog.md#ondialogopen)
- [renderContents](corelib.Reporting.ReportDialog.md#rendercontents)
- [resetValidation](corelib.Reporting.ReportDialog.md#resetvalidation)
- [set\_dialogTitle](corelib.Reporting.ReportDialog.md#set_dialogtitle)
- [useIdPrefix](corelib.Reporting.ReportDialog.md#useidprefix)
- [validateForm](corelib.Reporting.ReportDialog.md#validateform)
- [closePanel](corelib.Reporting.ReportDialog.md#closepanel)
- [create](corelib.Reporting.ReportDialog.md#create)
- [elementFor](corelib.Reporting.ReportDialog.md#elementfor)
- [getWidgetName](corelib.Reporting.ReportDialog.md#getwidgetname)
- [openPanel](corelib.Reporting.ReportDialog.md#openpanel)

## Constructors

### constructor

• **new ReportDialog**(`opt`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `opt` | [`ReportDialogOptions`](../interfaces/corelib.Reporting.ReportDialogOptions.md) |

#### Overrides

[TemplatedDialog](corelib.TemplatedDialog.md).[constructor](corelib.TemplatedDialog.md#constructor)

#### Defined in

[src/ui/widgets/reporting.ts:15](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/reporting.ts#line&#x3D;15)

## Properties

### element

• **element**: `JQuery`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[element](corelib.TemplatedDialog.md#element)

#### Defined in

[src/ui/widgets/widget.ts:61](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;61)

___

### idPrefix

• `Readonly` **idPrefix**: `string`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[idPrefix](corelib.TemplatedDialog.md#idprefix)

#### Defined in

[src/ui/widgets/widget.ts:65](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;65)

___

### options

• `Protected` **options**: [`ReportDialogOptions`](../interfaces/corelib.Reporting.ReportDialogOptions.md)

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[options](corelib.TemplatedDialog.md#options)

#### Defined in

[src/ui/widgets/widget.ts:62](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;62)

___

### propertyGrid

• `Protected` **propertyGrid**: [`PropertyGrid`](corelib.PropertyGrid.md)

#### Defined in

[src/ui/widgets/reporting.ts:23](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/reporting.ts#line&#x3D;23)

___

### propertyItems

• `Protected` **propertyItems**: [`PropertyItem`](../interfaces/corelib_q.PropertyItem.md)[]

#### Defined in

[src/ui/widgets/reporting.ts:24](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/reporting.ts#line&#x3D;24)

___

### reportKey

• `Protected` **reportKey**: `string`

#### Defined in

[src/ui/widgets/reporting.ts:25](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/reporting.ts#line&#x3D;25)

___

### tabs

• `Protected` **tabs**: `JQuery`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[tabs](corelib.TemplatedDialog.md#tabs)

#### Defined in

[src/ui/dialogs/templateddialog.ts:12](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;12)

___

### toolbar

• `Protected` **toolbar**: [`Toolbar`](corelib.Toolbar.md)

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[toolbar](corelib.TemplatedDialog.md#toolbar)

#### Defined in

[src/ui/dialogs/templateddialog.ts:13](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;13)

___

### uniqueName

• `Protected` **uniqueName**: `string`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[uniqueName](corelib.TemplatedDialog.md#uniquename)

#### Defined in

[src/ui/widgets/widget.ts:64](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;64)

___

### validator

• `Protected` **validator**: `Validator`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[validator](corelib.TemplatedDialog.md#validator)

#### Defined in

[src/ui/dialogs/templateddialog.ts:14](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;14)

___

### widgetName

• `Protected` **widgetName**: `string`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[widgetName](corelib.TemplatedDialog.md#widgetname)

#### Defined in

[src/ui/widgets/widget.ts:63](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;63)

___

### bootstrapModal

▪ `Static` **bootstrapModal**: `boolean`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[bootstrapModal](corelib.TemplatedDialog.md#bootstrapmodal)

#### Defined in

[src/ui/dialogs/templateddialog.ts:274](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;274)

## Accessors

### dialogTitle

• `get` **dialogTitle**(): `string`

#### Returns

`string`

#### Inherited from

TemplatedDialog.dialogTitle

#### Defined in

[src/ui/dialogs/templateddialog.ts:385](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;385)

• `set` **dialogTitle**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Inherited from

TemplatedDialog.dialogTitle

#### Defined in

[src/ui/dialogs/templateddialog.ts:420](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;420)

___

### isMarkedAsPanel

• `Private` `get` **isMarkedAsPanel**(): `boolean`

#### Returns

`boolean`

#### Inherited from

TemplatedDialog.isMarkedAsPanel

#### Defined in

[src/ui/dialogs/templateddialog.ts:26](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;26)

___

### isResponsive

• `Private` `get` **isResponsive**(): `boolean`

#### Returns

`boolean`

#### Inherited from

TemplatedDialog.isResponsive

#### Defined in

[src/ui/dialogs/templateddialog.ts:32](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;32)

## Methods

### addCssClass

▸ `Protected` **addCssClass**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[addCssClass](corelib.TemplatedDialog.md#addcssclass)

#### Defined in

[src/ui/dialogs/templateddialog.ts:340](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;340)

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

[TemplatedDialog](corelib.TemplatedDialog.md).[addValidationRule](corelib.TemplatedDialog.md#addvalidationrule)

#### Defined in

[src/ui/widgets/widget.ts:134](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;134)

___

### arrange

▸ **arrange**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[arrange](corelib.TemplatedDialog.md#arrange)

#### Defined in

[src/ui/dialogs/templateddialog.ts:316](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;316)

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

[TemplatedDialog](corelib.TemplatedDialog.md).[byId](corelib.TemplatedDialog.md#byid)

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

[TemplatedDialog](corelib.TemplatedDialog.md).[change](corelib.TemplatedDialog.md#change)

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

[TemplatedDialog](corelib.TemplatedDialog.md).[change](corelib.TemplatedDialog.md#change)

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

[TemplatedDialog](corelib.TemplatedDialog.md).[changeSelect2](corelib.TemplatedDialog.md#changeselect2)

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

[TemplatedDialog](corelib.TemplatedDialog.md).[changeSelect2](corelib.TemplatedDialog.md#changeselect2)

#### Defined in

[src/ui/widgets/widget.ts:260](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;260)

___

### createPropertyGrid

▸ `Protected` **createPropertyGrid**(): `void`

#### Returns

`void`

#### Defined in

[src/ui/widgets/reporting.ts:27](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/reporting.ts#line&#x3D;27)

___

### destroy

▸ **destroy**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[destroy](corelib.TemplatedDialog.md#destroy)

#### Defined in

[src/ui/dialogs/templateddialog.ts:81](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;81)

___

### dialogClose

▸ **dialogClose**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[dialogClose](corelib.TemplatedDialog.md#dialogclose)

#### Defined in

[src/ui/dialogs/templateddialog.ts:375](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;375)

___

### dialogOpen

▸ **dialogOpen**(`asPanel?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `asPanel?` | `boolean` |

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[dialogOpen](corelib.TemplatedDialog.md#dialogopen)

#### Defined in

[src/ui/dialogs/templateddialog.ts:244](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;244)

___

### executeReport

▸ **executeReport**(`targetFrame`, `exportType`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `targetFrame` | `string` |
| `exportType` | `string` |

#### Returns

`void`

#### Defined in

[src/ui/widgets/reporting.ts:60](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/reporting.ts#line&#x3D;60)

___

### getCssClass

▸ `Protected` **getCssClass**(): `string`

#### Returns

`string`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[getCssClass](corelib.TemplatedDialog.md#getcssclass)

#### Defined in

[src/ui/widgets/widget.ts:104](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;104)

___

### getDialogButtons

▸ `Protected` **getDialogButtons**(): [`DialogButton`](../interfaces/corelib_q.DialogButton.md)[]

#### Returns

[`DialogButton`](../interfaces/corelib_q.DialogButton.md)[]

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[getDialogButtons](corelib.TemplatedDialog.md#getdialogbuttons)

#### Defined in

[src/ui/dialogs/templateddialog.ts:349](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;349)

___

### getDialogOptions

▸ `Protected` **getDialogOptions**(): `any`

#### Returns

`any`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[getDialogOptions](corelib.TemplatedDialog.md#getdialogoptions)

#### Defined in

[src/ui/dialogs/templateddialog.ts:353](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;353)

___

### getDialogTitle

▸ `Protected` **getDialogTitle**(): `string`

#### Returns

`string`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[getDialogTitle](corelib.TemplatedDialog.md#getdialogtitle)

#### Defined in

[src/ui/dialogs/templateddialog.ts:371](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;371)

___

### getFallbackTemplate

▸ `Protected` **getFallbackTemplate**(): `string`

#### Returns

`string`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[getFallbackTemplate](corelib.TemplatedDialog.md#getfallbacktemplate)

#### Defined in

[src/ui/widgets/templatedwidget.ts:79](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/templatedwidget.ts#line&#x3D;79)

___

### getGridField

▸ **getGridField**(): `JQuery`

#### Returns

`JQuery`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[getGridField](corelib.TemplatedDialog.md#getgridfield)

#### Defined in

[src/ui/widgets/widget.ts:138](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;138)

___

### getModalOptions

▸ `Protected` **getModalOptions**(): [`ModalOptions`](../interfaces/corelib.ModalOptions.md)

#### Returns

[`ModalOptions`](../interfaces/corelib.ModalOptions.md)

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[getModalOptions](corelib.TemplatedDialog.md#getmodaloptions)

#### Defined in

[src/ui/dialogs/templateddialog.ts:153](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;153)

___

### getTemplate

▸ `Protected` **getTemplate**(): `string`

#### Returns

`string`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[getTemplate](corelib.TemplatedDialog.md#gettemplate)

#### Defined in

[src/ui/widgets/templatedwidget.ts:83](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/templatedwidget.ts#line&#x3D;83)

___

### getTemplateName

▸ `Protected` **getTemplateName**(): `string`

#### Returns

`string`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[getTemplateName](corelib.TemplatedDialog.md#gettemplatename)

#### Defined in

[src/ui/widgets/templatedwidget.ts:31](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/templatedwidget.ts#line&#x3D;31)

___

### getToolbarButtons

▸ `Protected` **getToolbarButtons**(): { `cssClass`: `string` = 'print-preview-button'; `onClick`: () => `void` ; `title`: `string` = 'Önizleme' }[]

#### Returns

{ `cssClass`: `string` = 'print-preview-button'; `onClick`: () => `void` ; `title`: `string` = 'Önizleme' }[]

#### Overrides

[TemplatedDialog](corelib.TemplatedDialog.md).[getToolbarButtons](corelib.TemplatedDialog.md#gettoolbarbuttons)

#### Defined in

[src/ui/widgets/reporting.ts:78](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/reporting.ts#line&#x3D;78)

___

### getValidatorOptions

▸ `Protected` **getValidatorOptions**(): `ValidationOptions`

#### Returns

`ValidationOptions`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[getValidatorOptions](corelib.TemplatedDialog.md#getvalidatoroptions)

#### Defined in

[src/ui/dialogs/templateddialog.ts:224](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;224)

___

### handleResponsive

▸ `Protected` **handleResponsive**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[handleResponsive](corelib.TemplatedDialog.md#handleresponsive)

#### Defined in

[src/ui/dialogs/templateddialog.ts:451](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;451)

___

### init

▸ **init**(`action?`): [`ReportDialog`](corelib.Reporting.ReportDialog.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `action?` | (`widget`: `any`) => `void` |

#### Returns

[`ReportDialog`](corelib.Reporting.ReportDialog.md)

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[init](corelib.TemplatedDialog.md#init)

#### Defined in

[src/ui/widgets/widget.ts:179](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;179)

___

### initDialog

▸ `Protected` **initDialog**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[initDialog](corelib.TemplatedDialog.md#initdialog)

#### Defined in

[src/ui/dialogs/templateddialog.ts:104](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;104)

___

### initModal

▸ `Protected` **initModal**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[initModal](corelib.TemplatedDialog.md#initmodal)

#### Defined in

[src/ui/dialogs/templateddialog.ts:162](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;162)

___

### initTabs

▸ `Protected` **initTabs**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[initTabs](corelib.TemplatedDialog.md#inittabs)

#### Defined in

[src/ui/dialogs/templateddialog.ts:442](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;442)

___

### initToolbar

▸ `Protected` **initToolbar**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[initToolbar](corelib.TemplatedDialog.md#inittoolbar)

#### Defined in

[src/ui/dialogs/templateddialog.ts:203](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;203)

___

### initValidator

▸ `Protected` **initValidator**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[initValidator](corelib.TemplatedDialog.md#initvalidator)

#### Defined in

[src/ui/dialogs/templateddialog.ts:228](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;228)

___

### initialize

▸ **initialize**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[initialize](corelib.TemplatedDialog.md#initialize)

#### Defined in

[src/ui/widgets/widget.ts:176](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;176)

___

### loadReport

▸ **loadReport**(`reportKey`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `reportKey` | `string` |

#### Returns

`void`

#### Defined in

[src/ui/widgets/reporting.ts:39](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/reporting.ts#line&#x3D;39)

___

### onDialogClose

▸ `Protected` **onDialogClose**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[onDialogClose](corelib.TemplatedDialog.md#ondialogclose)

#### Defined in

[src/ui/dialogs/templateddialog.ts:322](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;322)

___

### onDialogOpen

▸ `Protected` **onDialogOpen**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[onDialogOpen](corelib.TemplatedDialog.md#ondialogopen)

#### Defined in

[src/ui/dialogs/templateddialog.ts:309](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;309)

___

### renderContents

▸ `Protected` **renderContents**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[renderContents](corelib.TemplatedDialog.md#rendercontents)

#### Defined in

[src/ui/widgets/templatedwidget.ts:110](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/templatedwidget.ts#line&#x3D;110)

___

### resetValidation

▸ `Protected` **resetValidation**(): `void`

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[resetValidation](corelib.TemplatedDialog.md#resetvalidation)

#### Defined in

[src/ui/dialogs/templateddialog.ts:236](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;236)

___

### set\_dialogTitle

▸ **set_dialogTitle**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[set_dialogTitle](corelib.TemplatedDialog.md#set_dialogtitle)

#### Defined in

[src/ui/dialogs/templateddialog.ts:438](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;438)

___

### useIdPrefix

▸ `Protected` **useIdPrefix**(): `IdPrefixType`

#### Returns

`IdPrefixType`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[useIdPrefix](corelib.TemplatedDialog.md#useidprefix)

#### Defined in

[src/ui/widgets/templatedwidget.ts:131](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/templatedwidget.ts#line&#x3D;131)

___

### validateForm

▸ `Protected` **validateForm**(): `boolean`

#### Returns

`boolean`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[validateForm](corelib.TemplatedDialog.md#validateform)

#### Defined in

[src/ui/dialogs/templateddialog.ts:240](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;240)

___

### closePanel

▸ `Static` **closePanel**(`element`, `e?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `element` | `JQuery` |
| `e?` | `JQueryEventObject` |

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[closePanel](corelib.TemplatedDialog.md#closepanel)

#### Defined in

[src/ui/dialogs/templateddialog.ts:305](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;305)

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

[TemplatedDialog](corelib.TemplatedDialog.md).[create](corelib.TemplatedDialog.md#create)

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

[TemplatedDialog](corelib.TemplatedDialog.md).[elementFor](corelib.TemplatedDialog.md#elementfor)

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

[TemplatedDialog](corelib.TemplatedDialog.md).[getWidgetName](corelib.TemplatedDialog.md#getwidgetname)

#### Defined in

[src/ui/widgets/widget.ts:124](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/widgets/widget.ts#line&#x3D;124)

___

### openPanel

▸ `Static` **openPanel**(`element`, `uniqueName`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `element` | `JQuery` |
| `uniqueName` | `string` |

#### Returns

`void`

#### Inherited from

[TemplatedDialog](corelib.TemplatedDialog.md).[openPanel](corelib.TemplatedDialog.md#openpanel)

#### Defined in

[src/ui/dialogs/templateddialog.ts:276](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/dialogs/templateddialog.ts#line&#x3D;276)