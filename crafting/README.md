# Crafting

This is probably the most dense/difficult section out of all of the templates.
If you have any questions just send me a message on discord.

Idea: Need a tanning bench by hunting to turn hides into leather. Better hides =
more leather

- [Back to Main Page](../README.md#alcatraz-templates)

- [Raw Materials](#raw-materials)
- [Craftable Items](#craftable-items)
- [Public Bench](#public-bench)
- [Job Specific Bench](#job-specific-bench)

- [Guns Page](./weapons/README.md#custom-guns)

## Bench Categories

- Weapons
- Health
- Ammo
- Materials
- Other
- add more to the discord

## Raw Materials

### Cold, hard cash:

- money

### Mined materials:

- gold
- silver
- steel
- brass
- iron
- copper
- sulfur
- coal_chunk

### Recycled materials:

- plastic
- cloth
- rubber
- glass
- aluminum
- electronic_parts

### Hunting materials:

- animal_fat
- bone_fragments
- skin_boar
- skin_cow
- skin_deer
- skin_pig
- skin_coyote
- skin_mtlion

### Blueprints: (need more)

- access_tool_blueprint
- micro_smg_blueprint
- pipebomb_blueprint
- brassknuckle_blueprint

### Pages:

- blueprint_scrap
- recipe_page

### Crafted Materials:

- gunpowder
- leather

### Guns:

- [guns page](./weapons/README.md)

## Craftable Items

- [Raw Materials](#raw-materials)

### These are all of the currently available items for crafting. Need to add more

- rifle
- bandage

```lua
['rifle'] = {
  item = 'weapon_assaultrifle',   -- NEEDED - CHANGE ME: Item id. Just write out the item name as you see it, and I can find the proper name. Adding list of items soon.
  amount = 1,                     -- NEEDED - CHANGE ME: Amount of the item the player will receive
  maxCraft = 1,                   -- NEEDED - CHANGE ME: Max amount of crafts at a time
  successCraftPercentage = 75,    -- NEEDED - CHANGE ME: Percentage of successful craft 0 = 0% | 50 = 50% | 100 = 100%
  isItem = true,
  isDisassemble = false,          -- OPTIONAL - CHANGE ME: true = disassemble | false = craft
  time = 6,                       -- OPTIONAL - CHANGE ME: Time to craft (in seconds)
  levelNeeded = 0,                -- OPTIONAL - CHANGE ME: What level he needs to craft this item
  xpPerCraft = 40,                -- OPTIONAL - CHANGE ME: How much XP he receives after crafting this item
  recipe = {                      -- NEEDED - CHANGE ME: Recipe to craft it. Add more/less materials (materials list above) depending on the item
    {'iron', 1, true, false},     -- READ ME: item/amount/remove item/only true for money
    {'money', 2000, true, true},
  },
  job = {''},
  data = {},
  category = 'Weapons',           -- OPTIONAL - CHANGE ME: Used Name of the category
},
```

```lua
['bandage'] = {
  item = 'bandage',               -- NEEDED - CHANGE ME: Item id. Just write out the item name as you see it, and I can find the proper name. Adding list of items soon.
  amount = 1,                     -- NEEDED - CHANGE ME: Amount of the item the player will receive
  maxCraft = 10,                  -- NEEDED - CHANGE ME: Max amount of crafts at a time
  successCraftPercentage = 75,    -- NEEDED - CHANGE ME: Percentage of successful craft 0 = 0% | 50 = 50% | 100 = 100%
  isItem = true,
  isDisassemble = false,          -- OPTIONAL - CHANGE ME: true = disassemble | false = craft
  time = 3,                       -- OPTIONAL - CHANGE ME: Time to craft (in seconds)
  levelNeeded = 0,                -- OPTIONAL - CHANGE ME: What level he needs to craft this item
  xpPerCraft = 15,                -- OPTIONAL - CHANGE ME: How much XP he receives after crafting this item
  recipe = {                      -- NEEDED - CHANGE ME: Recipe to craft it. Add more/less materials (materials list above) depending on the item
    {'cloth', 4, true, false},    -- READ ME: item/amount/remove item/only true for money
  },
  job = {
    ''
  },
  data = {},
  category = 'Health',            -- OPTIONAL - CHANGE ME: Used Name of the category
},
```

## Public Bench

- [Craftable Items](#craftable-items)

This bench will be open to all.

```lua
{
  coordinates = vector3(-817.0, 182.8, 72.3),     -- NEEDED - CHANGE ME: coordinates of the table
  radius = 1,
  showMapBlip = false,
  marker = {type = 20, r = 31, g = 94, b = 255, a = 155, bobUpAndDown = 0, faceCamera = 0, rotate = 1, textureDict = 0, textureName = 0, drawOnEnts = 0},
  showBlipRadius = 50,
  blip = {blipId = 89, blipColor = 3, blipScale = 0.9, blipText = 'Crafting'},
  tableName = 'Weapons',                          -- OPTIONAL - CHANGE ME: Title
  tableID = 'general2',
  crafts = {                                      -- NEEDED - CHANGE ME: What items are available for crafting and the recipe. Add more from the list of Craftable Items above
    'bandage',
  },
  jobs = {
    ['all'] = true
  },
},
```

## Job Specific Bench

- [Craftable Items](#craftable-items)

These benches will only be used by specific jobs, and it can also be refined to
specific job grades.

```lua
{
  coordinates = vector3(-809.4, 190.3, 72.5),   -- NEEDED - CHANGE ME: coordinates of the table
  radius = 1,                                   -- OPTIONAL - CHANGE ME: radius of the table. 1 or 2 are sane values
  showMapBlip = true,
  marker = {type = 20, r = 31, g = 94, b = 255, a = 155, bobUpAndDown = 0, faceCamera = 0, rotate = 1, textureDict = 0, textureName = 0, drawOnEnts = 0},
  showBlipRadius = 50,
  blip = {blipId = 89, blipColor = 3, blipScale = 0.9, blipText = 'Crafting'},
  tableName = 'General',                        -- OPTIONAL - CHANGE ME: Title
  tableID = 'general1',
  crafts = {                                    -- NEEDED - CHANGE ME: What items are available for crafting and the recipe. Add more from the list of craftable items
    'rifle',
    'bandage',
  },
  jobs = {                                      -- NEEDED - CHANGE ME: What jobs are able to open the workbench
    ['police'] = {
      ['boss'] = true,
      ['chief'] = true,
    },
    ['ambulance'] = {
      ['boss'] = true,
      ['chief'] = true,
    },
  },
},
```
