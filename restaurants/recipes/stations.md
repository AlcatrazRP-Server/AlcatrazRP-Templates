# Stations

- [Recipes](./recipes.md/#recipes)

- [Drinks](../items/drinks.md/#drinks)
- [Food](../items/food.md/#food)
- [Restaurants](../items/restaurants.md/#restaurants)

- [Back to Items](../restaurants.md)
- [Back to Main](../../README.md)

```lua
['pearls'] = { -- name of location
    -- add as many targets as you want for each location, customize the target options, actions, items as you'd like
    ['pearls_prepare'] = { -- target name
        label = 'prepare', --menu header
        --target & options:
        coords = vector3(-1848.13, -1199.26, 14.31),
        length = 1,
        width = 2.5,
        size = vector3(1.0, 1.0, 2.0), -- ox_target only
        heading = 330.0,
        debug = false,
        minZ = 12.0,
        maxZ = 16.0,

        recipes = {'fish_taco', 'sushi', 'sdft_tomato'},

        animdict = "anim@amb@business@coc@coc_unpack_cut@",
        animation = "fullcut_cycle_v5_cokecutter",
        flags = 16,

        job = 'pearls', --which jobs while be able to see the target option
    },

    ['pearls_stove'] = { --cook target
        label = 'stove',

        coords = vector3(-1847.22, -1194.03, 14.31),
        length = 2.0,
        width = 0.75,
        size = vector3(1.0, 1.0, 2.0), -- ox_target only
        heading = 330.0,
        debug = false,

        minZ = 12.0,
        maxZ = 16.0,

        recipes = {'cooked_fish'},

        scenario = "PROP_HUMAN_BBQ",
        prop = 'prop_fish_slice_01', --spatula prop from scenario above

        job = 'pearls',
    },

    ['pearls_fryer'] = { --cook target
        label = 'fryer',
        coords = vector3(-1848.11, -1195.51, 14.31),
        length = 1,
        width = 1.5,
        size = vector3(1.0, 1.0, 2.0), -- ox_target only
        heading = 60.0,
        debug = false,

        minZ = 12.0,
        maxZ = 16.0,

        recipes = {'fish_taco', 'sdft_fries'},

        animdict = "amb@prop_human_bbq@male@idle_a",
        animation = "idle_b",
        flags = 16,

        job = 'pearls',
    },
},
```
