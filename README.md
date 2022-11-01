# Minecraft Bedrock Item DB

This is a simple repo containing JSON files with list of all Minecraft Bedrock items and blocks together with useful info about them.

## Items

Item object schema:

| Name             | Value                                                           |
|------------------|-----------------------------------------------------------------|
| `id`             | ID of the item                                                  |
| `legacyId`       | Numerical ID of the item                                        |
| `metadata`       | Numerical data value of the item variant                        |
| `maxDurability`  | Maximum durability this item can have                           |
| `damage`         | Damage, that this damage can deal                               |
| `armor`          | Armor value, that this damage will give to the wearer           |
| `maxStackSize`   | Maximum stack size                                              |
| `tags`           | A list of tags, that this item has                              |
| `category`       | Creative category of this item                                  |
| `nutrition`      | Nutrition value of the food item                                |
| `fuelDuration`   | Duration, for which this item burns in a furnace                |
| `aliases`        | A list of old IDs, that this item was under                     |
| `minimumVersion` | Required Minecraft version in order to be able to use this item |
| `langKey`        | Key in language files, that will hold the name of this item     |
| `langName`       | Item name in English                                            |

## Blocks

Block object schema:

| Name             | Value                                                           |
|------------------|-----------------------------------------------------------------|
| `id`             | ID of the block                                                 |
| `legacyId`       | Numerical ID of the item                                        |
| `group`          | Item group in creative inventory                                |
| `tags`           | A list of tags, that this block has                             |
| `aliases`        | A list of old IDs, that this item was under                     |
| `minimumVersion` | Required Minecraft version in order to be able to use this item |
| `variants`       | A list of block variants                                        |

Block Variant object schema:

| Name       | Value                                                            |
|------------|------------------------------------------------------------------|
| `metadata` | Numerical data value of the block variant                        |
| `states`   | List of NBT properties, that will be defined for this data value |

NBT Property object schema:

| Name    | Value                 |
|---------|-----------------------|
| `name`  | Name of the property  |
| `type`  | Type of the property  |
| `value` | Value of the property |