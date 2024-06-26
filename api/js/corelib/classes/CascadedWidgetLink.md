[@serenity-is/corelib](../README.md) / CascadedWidgetLink

# Class: CascadedWidgetLink\<TParent\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `TParent` | extends [`Widget`](Widget.md)\<`any`\> |

## Table of contents

### Constructors

- [constructor](CascadedWidgetLink.md#constructor)

### Methods

- [bind](CascadedWidgetLink.md#bind)
- [get\_parentID](CascadedWidgetLink.md#get_parentid)
- [set\_parentID](CascadedWidgetLink.md#set_parentid)
- [unbind](CascadedWidgetLink.md#unbind)

## Constructors

### constructor

• **new CascadedWidgetLink**\<`TParent`\>(`parentType`, `widget`, `parentChange`): [`CascadedWidgetLink`](CascadedWidgetLink.md)\<`TParent`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TParent` | extends [`Widget`](Widget.md)\<`any`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `parentType` | (...`args`: `any`[]) => `TParent` |
| `widget` | [`Widget`](Widget.md)\<`any`\> |
| `parentChange` | (`p1`: `TParent`) => `void` |

#### Returns

[`CascadedWidgetLink`](CascadedWidgetLink.md)\<`TParent`\>

#### Defined in

[src/ui/editors/cascadedwidgetlink.ts:10](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/cascadedwidgetlink.ts#L10)

## Methods

### bind

▸ **bind**(): `TParent`

#### Returns

`TParent`

#### Defined in

[src/ui/editors/cascadedwidgetlink.ts:23](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/cascadedwidgetlink.ts#L23)

___

### get\_parentID

▸ **get_parentID**(): `string`

#### Returns

`string`

#### Defined in

[src/ui/editors/cascadedwidgetlink.ts:58](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/cascadedwidgetlink.ts#L58)

___

### set\_parentID

▸ **set_parentID**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Defined in

[src/ui/editors/cascadedwidgetlink.ts:62](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/cascadedwidgetlink.ts#L62)

___

### unbind

▸ **unbind**(): `TParent`

#### Returns

`TParent`

#### Defined in

[src/ui/editors/cascadedwidgetlink.ts:43](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/ui/editors/cascadedwidgetlink.ts#L43)
