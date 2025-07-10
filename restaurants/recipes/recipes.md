# Recipes

- [Stations](./stations.md/#stations)

- [Drinks](../items/drinks.md/#drinks)
- [Food](../items/food.md/#food)
- [Restaurants](../items/restaurants.md/#restaurants)

- [Back to Items](../restaurants.md)
- [Back to Main](../../README.md)

```lua
config.recipes = {
-- INGREDIENT PREP
--#region PREPARED INGREDIENTS
['sdft_tomato'] = {
    ['label'] = 'Tomato Slices',
    ['time_per_item'] = 1500, -- in ms
    ['base_output'] = 3,      -- Always gives 3 per craft
    ['ingredients'] = {
        {label = "Whole Tomato",        ingredient = 'tomato',       amount = 1},
    },
},
['onions'] = {
    ['label'] = 'Onion Slices',
    ['time_per_item'] = 1500,
    ['base_output'] = 3, -- Always gives 3 per craft
    ['ingredients'] = {
        {label = "Whole Onion",        ingredient = 'onion',       amount = 1},
    },
},
--#endregion

-- COOKED MEATS
--#region COOKED RED MEAT
['sdft_patty_cooked'] = {
    ['label'] = 'Cooked Patty',
    ['time_per_item'] = 1000,
    ['ingredients'] = {
        {label = "Raw Patty",        ingredient = 'sdft_patty',       amount = 1},
    },
},
['sdft_bacon_cooked'] = {
    ['label'] = 'Cooked Bacon',
    ['time_per_item'] = 1000,
    ['ingredients'] = {
        {label = "Raw Bacon",        ingredient = 'sdft_bacon',       amount = 1},
    },
},
['sdft_vpatty_cooked'] = {
    ['label'] = 'Cooked Vegan Patty',
    ['time_per_item'] = 1000,
    ['ingredients'] = {
        {label = "Raw Vegan Patty",        ingredient = 'sdft_vpatty',       amount = 1},
    },
},
--#endregion

--#region COOKED WHITE MEAT
['cooked_chicken'] = {
    ['label'] = 'Cooked Chicken',
    ['time_per_item'] = 6000,
    ['ingredients'] = {
        {label = "Raw Chicken",      ingredient = 'raw_chicken',     amount = 1},
    },
},
--#endregion

--#region COOKED FISH
['cooked_fish'] = {
    ['label'] = 'Cooked Fish',
    ['time_per_item'] = 5000,
    ['ingredients'] = {
        {label = "Raw Fish",         ingredient = 'raw_fish',        amount = 1},
    },
},
--#endregion

-- MAIN DISHES
--#region BURGERS
['sdft_burger'] = { -- must match the item_name in your inventory
    ['label'] = 'Burger',
    ['time_per_item'] = 1200,
    ['ingredients'] = {
        {label = "Lettuce",          ingredient = 'sdft_lettuce',         amount = 1},
        {label = "Tomato",           ingredient = 'sdft_tomato',          amount = 1},
        {label = "Cheese",           ingredient = 'sdft_cheese',          amount = 1},
        {label = "Buns",             ingredient = 'sdft_bun',             amount = 1},
        {label = "Onions",           ingredient = 'onions',               amount = 1},
        {label = "Cooked Patty",     ingredient = 'sdft_patty_cooked',    amount = 1},
    },
},
['atom_vegan'] = {
    ['label'] = 'Vegan Burger',
    ['time_per_item'] = 1200,
    ['ingredients'] = {
        {label = "Lettuce",          ingredient = 'sdft_lettuce',         amount = 1},
        {label = "Tomato",           ingredient = 'sdft_tomato',          amount = 1},
        {label = "Cheese",           ingredient = 'sdft_cheese',          amount = 1},
        {label = "Buns",             ingredient = 'sdft_bun',             amount = 1},
        {label = "Onions",           ingredient = 'onions',               amount = 1},
        {label = "Cooked Vegan Patty",     ingredient = 'sdft_vpatty_cooked',    amount = 1},
    },
},
['sdft_doubleburger'] = { -- must match the item_name in your inventory
    ['label'] = 'Double Burger',
    ['time_per_item'] = 1500,
    ['ingredients'] = {
        {label = "Lettuce",          ingredient = 'sdft_lettuce',         amount = 1},
        {label = "Tomato",           ingredient = 'sdft_tomato',          amount = 1},
        {label = "Cheese",           ingredient = 'sdft_cheese',          amount = 2},
        {label = "Buns",             ingredient = 'sdft_bun',             amount = 1},
        {label = "Onions",           ingredient = 'onions',               amount = 1},
        {label = "Cooked Patty",     ingredient = 'sdft_patty_cooked',    amount = 2},
    },
},
['atom_double'] = { -- must match the item_name in your inventory
    ['label'] = 'Double Burger',
    ['time_per_item'] = 1500,
    ['ingredients'] = {
        {label = "Lettuce",          ingredient = 'sdft_lettuce',         amount = 1},
        {label = "Tomato",           ingredient = 'sdft_tomato',          amount = 1},
        {label = "Cheese",           ingredient = 'sdft_cheese',          amount = 2},
        {label = "Buns",             ingredient = 'sdft_bun',             amount = 1},
        {label = "Onions",           ingredient = 'onions',               amount = 1},
        {label = "Cooked Patty",     ingredient = 'sdft_patty_cooked',    amount = 2},
    },
},
['sdft_kingsizeburger'] = { -- must match the item_name in your inventory
    ['label'] = 'Triple Burger',
    ['time_per_item'] = 1800,
    ['ingredients'] = {
        {label = "Lettuce",          ingredient = 'sdft_lettuce',         amount = 1},
        {label = "Tomato",           ingredient = 'sdft_tomato',          amount = 1},
        {label = "Cheese",           ingredient = 'sdft_cheese',          amount = 3},
        {label = "Buns",             ingredient = 'sdft_bun',             amount = 1},
        {label = "Onions",           ingredient = 'onions',               amount = 1},
        {label = "Cooked Patty",     ingredient = 'sdft_patty_cooked',    amount = 3},
    },
},
['sdft_baconburger'] = { -- must match the item_name in your inventory
    ['label'] = 'Bacon Burger',
    ['time_per_item'] = 1500,
    ['ingredients'] = {
        {label = "Cheese",           ingredient = 'sdft_cheese',          amount = 2},
        {label = "Buns",             ingredient = 'sdft_bun',             amount = 1},
        {label = "Cooked Patty",     ingredient = 'sdft_patty_cooked',    amount = 1},
        {label = "Cooked Bacon",     ingredient = 'sdft_bacon_cooked',    amount = 2},
    },
},
--#endregion

--#region FISH DISHES
['fish_taco'] = {
    ['label'] = 'Fish Taco',
    ['time_per_item'] = 7000,
    ['ingredients'] = {
        {label = "Tortilla",         ingredient = 'sdft_torilla',        amount = 1},
        {label = "Cooked Fish",      ingredient = 'cooked_fish',     amount = 1},
        {label = "Lettuce",          ingredient = 'sdft_lettuce',         amount = 1},
        {label = "Tomato",           ingredient = 'sdft_tomato',          amount = 1},
    },
},
--#endregion

--#region WHITE MEAT DISHES
['orange_chicken'] = {
    ['label'] = 'Orange Chicken',
    ['time_per_item'] = 8000,
    ['ingredients'] = {
        {label = "Cooked Chicken",   ingredient = 'cooked_chicken',  amount = 1},
        {label = "Orange",           ingredient = 'orange',          amount = 1},
    },
},
['chicken_fried_rice'] = {
    ['label'] = 'Chicken Fried Rice',
    ['time_per_item'] = 9000,
    ['ingredients'] = {
        {label = "Cooked Chicken",   ingredient = 'cooked_chicken',  amount = 1},
        {label = "Fried Rice",        ingredient = 'fried_rice',      amount = 1},
    },
},
--#endregion

--#region SUSHI
['sushi'] = {
    ['label'] = 'Sushi',
    ['time_per_item'] = 6000,
    ['ingredients'] = {
        {label = "Rice",             ingredient = 'rice',           amount = 1},
        {label = "Raw Fish",         ingredient = 'raw_fish',        amount = 1},
    },
},
--#endregion

--#region SIDE DISHES
['sdft_fries'] = {
    ['label'] = 'Fries',
    ['time_per_item'] = 4000,
    ['ingredients'] = {
        {label = "potato",           ingredient = 'potato',          amount = 1},
    },
},
['atomfries_small'] = {
    ['label'] = 'Small Fries',
    ['time_per_item'] = 1100,
    ['ingredients'] = {
        {label = "potato",           ingredient = 'potato',          amount = 1},
    },
},
['atomfries_medium'] = {
    ['label'] = 'Medium Fries',
    ['time_per_item'] = 1600,
    ['ingredients'] = {
        {label = "potato",           ingredient = 'potato',          amount = 2},
    },
},
['atomfries_large'] = {
    ['label'] = 'Large Fries',
    ['time_per_item'] = 2000,
    ['ingredients'] = {
        {label = "potato",           ingredient = 'potato',          amount = 3},
    },
},
['fried_rice'] = {
    ['label'] = 'Fried Rice',
    ['time_per_item'] = 5000,
    ['ingredients'] = {
        {label = "Rice",             ingredient = 'rice',           amount = 1},
        {label = "Fresh Egg",              ingredient = 'egg_raw',            amount = 1},
    },
},
--#endregion
}
```
