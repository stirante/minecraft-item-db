# Minecraft Bedrock Item DB

This is a simple repo containing JSON files with list of all Minecraft Bedrock items and blocks together with useful info about them.

To save some space, some properties are hidden, when set to default or empty value.

## Items

Item object schema:

| Name             | Description                                                     | Default |
|------------------|-----------------------------------------------------------------|---------|
| `id`             | ID of the item                                                  |         |
| `legacyId`       | Numerical ID of the item                                        |         |
| `metadata`       | Numerical data value of the item variant                        |         |
| `maxDurability`  | Maximum durability this item can have                           | 0       |
| `damage`         | Damage, that this damage can deal                               | 0       |
| `armor`          | Armor value, that this damage will give to the wearer           | 0       |
| `maxStackSize`   | Maximum stack size                                              | 64      |
| `tags`           | A list of tags, that this item has                              |         |
| `category`       | Creative category of this item                                  |         |
| `nutrition`      | Nutrition value of the food item                                | 0       |
| `fuelDuration`   | Duration, for which this item burns in a furnace                | 0       |
| `aliases`        | A list of old IDs, that this item was under                     |         |
| `minimumVersion` | Required Minecraft version in order to be able to use this item |         |
| `langKey`        | Key in language files, that will hold the name of this item     |         |
| `langName`       | Item name in English                                            |         |

## Blocks

Block object schema:

| Name             | Description                                                      |
|------------------|------------------------------------------------------------------|
| `id`             | ID of the block                                                  |
| `legacyId`       | Numerical ID of the block                                        |
| `group`          | Item group in creative inventory                                 |
| `tags`           | A list of tags, that this block has                              |
| `aliases`        | A list of old IDs, that this block was under                     |
| `minimumVersion` | Required Minecraft version in order to be able to use this block |
| `variants`       | A list of block variants                                         |
| `mapColor`       | A hex color on the map in format `#RRGGBB`                       |

Block Variant object schema:

| Name       | Description                                                      |
|------------|------------------------------------------------------------------|
| `metadata` | Numerical data value of the block variant                        |
| `states`   | List of NBT properties, that will be defined for this data value |
| `mapColor` | A hex color on the map in format `#RRGGBB`                       |

NBT Property object schema:

| Name    | Description           |
|---------|-----------------------|
| `name`  | Name of the property  |
| `type`  | Type of the property  |
| `value` | Value of the property |