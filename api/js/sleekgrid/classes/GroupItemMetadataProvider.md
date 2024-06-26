[@serenity-is/sleekgrid](../README.md) / GroupItemMetadataProvider

# Class: GroupItemMetadataProvider

## Table of contents

### Constructors

- [constructor](GroupItemMetadataProvider.md#constructor)

### Properties

- [getGroupRowMetadata](GroupItemMetadataProvider.md#getgrouprowmetadata)
- [getTotalsRowMetadata](GroupItemMetadataProvider.md#gettotalsrowmetadata)
- [grid](GroupItemMetadataProvider.md#grid)
- [pluginName](GroupItemMetadataProvider.md#pluginname)
- [defaults](GroupItemMetadataProvider.md#defaults)

### Methods

- [destroy](GroupItemMetadataProvider.md#destroy)
- [getOptions](GroupItemMetadataProvider.md#getoptions)
- [groupCellPosition](GroupItemMetadataProvider.md#groupcellposition)
- [handleGridClick](GroupItemMetadataProvider.md#handlegridclick)
- [handleGridKeyDown](GroupItemMetadataProvider.md#handlegridkeydown)
- [init](GroupItemMetadataProvider.md#init)
- [setOptions](GroupItemMetadataProvider.md#setoptions)
- [defaultGroupFormat](GroupItemMetadataProvider.md#defaultgroupformat)
- [defaultTotalsFormat](GroupItemMetadataProvider.md#defaulttotalsformat)

## Constructors

### constructor

• **new GroupItemMetadataProvider**(`opt?`): [`GroupItemMetadataProvider`](GroupItemMetadataProvider.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `opt?` | [`GroupItemMetadataProviderOptions`](../interfaces/GroupItemMetadataProviderOptions.md) |

#### Returns

[`GroupItemMetadataProvider`](GroupItemMetadataProvider.md)

#### Defined in

[data/groupitemmetadataprovider.ts:29](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L29)

## Properties

### getGroupRowMetadata

• **getGroupRowMetadata**: (`item`: [`Group`](Group.md)\<`any`\>) => [`ItemMetadata`](../interfaces/ItemMetadata.md)\<`any`\>

#### Type declaration

▸ (`item`): [`ItemMetadata`](../interfaces/ItemMetadata.md)\<`any`\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `item` | [`Group`](Group.md)\<`any`\> |

##### Returns

[`ItemMetadata`](../interfaces/ItemMetadata.md)\<`any`\>

#### Defined in

[data/groupitemmetadataprovider.ts:193](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L193)

___

### getTotalsRowMetadata

• **getTotalsRowMetadata**: (`item`: [`GroupTotals`](GroupTotals.md)\<`any`\>) => [`ItemMetadata`](../interfaces/ItemMetadata.md)\<`any`\>

#### Type declaration

▸ (`item`): [`ItemMetadata`](../interfaces/ItemMetadata.md)\<`any`\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `item` | [`GroupTotals`](GroupTotals.md)\<`any`\> |

##### Returns

[`ItemMetadata`](../interfaces/ItemMetadata.md)\<`any`\>

#### Defined in

[data/groupitemmetadataprovider.ts:217](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L217)

___

### grid

• `Protected` **grid**: [`Grid`](Grid.md)\<`any`\>

#### Defined in

[data/groupitemmetadataprovider.ts:26](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L26)

___

### pluginName

• `Readonly` **pluginName**: ``"GroupItemMetadataProvider"``

#### Defined in

[data/groupitemmetadataprovider.ts:77](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L77)

___

### defaults

▪ `Static` `Readonly` **defaults**: [`GroupItemMetadataProviderOptions`](../interfaces/GroupItemMetadataProviderOptions.md)

#### Defined in

[data/groupitemmetadataprovider.ts:37](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L37)

## Methods

### destroy

▸ **destroy**(): `void`

#### Returns

`void`

#### Defined in

[data/groupitemmetadataprovider.ts:79](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L79)

___

### getOptions

▸ **getOptions**(): [`GroupItemMetadataProviderOptions`](../interfaces/GroupItemMetadataProviderOptions.md)

#### Returns

[`GroupItemMetadataProviderOptions`](../interfaces/GroupItemMetadataProviderOptions.md)

#### Defined in

[data/groupitemmetadataprovider.ts:86](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L86)

___

### groupCellPosition

▸ **groupCellPosition**(): `Object`

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `cell` | `number` |
| `colspan` | `number` \| ``"*"`` |

#### Defined in

[data/groupitemmetadataprovider.ts:156](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L156)

___

### handleGridClick

▸ **handleGridClick**(`e`, `args`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `MouseEvent` |
| `args` | [`ArgsCell`](../interfaces/ArgsCell.md) |

#### Returns

`void`

#### Defined in

[data/groupitemmetadataprovider.ts:94](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L94)

___

### handleGridKeyDown

▸ **handleGridKeyDown**(`e`, `args`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `KeyboardEvent` |
| `args` | [`ArgsCell`](../interfaces/ArgsCell.md) |

#### Returns

`void`

#### Defined in

[data/groupitemmetadataprovider.ts:120](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L120)

___

### init

▸ **init**(`grid`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `grid` | [`Grid`](Grid.md)\<`any`\> |

#### Returns

`void`

#### Defined in

[data/groupitemmetadataprovider.ts:71](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L71)

___

### setOptions

▸ **setOptions**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`GroupItemMetadataProviderOptions`](../interfaces/GroupItemMetadataProviderOptions.md) |

#### Returns

`void`

#### Defined in

[data/groupitemmetadataprovider.ts:90](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L90)

___

### defaultGroupFormat

▸ **defaultGroupFormat**(`ctx`, `opt?`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ctx` | [`FormatterContext`](../interfaces/FormatterContext.md)\<`any`\> |
| `opt?` | [`GroupItemMetadataProviderOptions`](../interfaces/GroupItemMetadataProviderOptions.md) |

#### Returns

`string`

#### Defined in

[data/groupitemmetadataprovider.ts:53](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L53)

___

### defaultTotalsFormat

▸ **defaultTotalsFormat**(`ctx`, `grid?`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ctx` | [`FormatterContext`](../interfaces/FormatterContext.md)\<`any`\> |
| `grid?` | [`Grid`](Grid.md)\<`any`\> |

#### Returns

`string`

#### Defined in

[data/groupitemmetadataprovider.ts:63](https://github.com/serenity-is/sleekgrid/blob/master/src/data/groupitemmetadataprovider.ts#L63)
