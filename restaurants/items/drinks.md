# Drinks

- [Recipes](../recipes/recipes.md/#recipes)
- [Stations](../recipes/stations.md/#stations)

- [Food Items](./food.md/#food)
- [Restaurant Items](./restaurants.md/#restaurants)

- [Back to Items](../restaurants.md)
- [Back to Main](../../README.md)

```lua
return {
	--#region HOT COFFEES
  ["coffee"] = {
		label = "Coffee",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -8, thirst = 10 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'Aaah, now that\'s fresh mountain grown coffee from the hills of Colombia',
		}
	},

	["coffee_chocolate_cream_frappuccino"] = {
		label = "Chocolate Cream Frappuccino",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -5, thirst = 15 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'Aaah, now that\'s fresh mountain grown coffee from the hills of Colombia',
		}
	},
	["coffee_cold_brew_coffee"] = {
		label = "Cold Brew Coffee",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -5, thirst = 15 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'Aaah, now that\'s fresh mountain grown coffee from the hills of Colombia',
		}
	},
	["coffee_cold_brew_latte"] = {
		label = "Cold Brew Latte",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -5, thirst = 15 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'Aaah, now that\'s fresh mountain grown coffee from the hills of Colombia',
		}
	},
	["coffee_cookies_cream_frappuccino"] = {
		label = "Cookies & Cream Frappuccino",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -5, thirst = 15 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'Aaah, now that\'s fresh mountain grown coffee from the hills of Colombia',
		}
	},
	["coffee_double_choc_chip_frappuccino"] = {
		label = "Double Chocolate Chip Frappuccino",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -5, thirst = 15 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,

			notifTitle = 'Gulp',
			notification = 'Aaah, now that\'s fresh mountain grown coffee from the hills of Colombia',
		}
	},
	["coffee_frappuccino"] = {
		label = "Frappuccino",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -5, thirst = 15 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'Aaah, now that\'s fresh mountain grown coffee from the hills of Colombia',
		}
	},
	--#endregion

	--#region ICED COFFEES
	["coffee_iced_black_tea"] = {
		label = "Iced Black Tea",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -5, thirst = 15 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'You quench your thirst with delicious iced coffee',
		}
	},
	["coffee_iced_black_tea_lemonade"] = {
		label = "Iced Black Tea Lemonade",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -5, thirst = 15 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'You quench your thirst with delicious iced coffee',
		}
	},
	["coffee_iced_caffe_americano"] = {
		label = "Iced Americane",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -5, thirst = 15 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'You quench your thirst with delicious iced coffee',
		}
	},
	["coffee_iced_caffe_latte"] = {
		label = "Iced Latte",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -5, thirst = 15 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'You quench your thirst with delicious iced coffee',
		}
	},
	["coffee_iced_green_tea"] = {
		label = "Iced Green Tea",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -5, thirst = 15 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'You quench your thirst with delicious iced coffee',
		}
	},
	["coffee_iced_green_tea_lemonade"] = {
		label = "Iced Green Tea Lemonade",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -5, thirst = 15 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'You quench your thirst with delicious iced coffee',
		}
	},
	["coffee_java_chip_frappuccino"] = {
		label = "Java Chip Frappuccino",
		weight = 200,
		stack = true,
		close = true,
		description = "What happens if I drink 100 cups?",
		client = {
			status = { stress = -5, thirst = 15 },
			anim = 'drinking can',
			prop = 'coffee',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'You quench your thirst with delicious iced coffee',
		}
	},
	--#endregion

	--#region SODAS
  ["cola"] = {
		label = "Cola",
		weight = 500,
		stack = true,
		close = true,
		allowArmed = true,
		description = "For all the thirsty out there",
		client = {
			status = { thirst = 20 },
			anim = 'drinking can',
			prop = 'cola',
			usetime = 2500,
      disable = { combat = true, sprint = true },
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'You quenched your thirst with a refreshing cola',
		}
	},
  ["drink_sprite"] = {
		label = "Sprite",
		weight = 500,
		stack = true,
		close = false,
		client = {
        status = { thirst = 20 },
        anim = 'drinking bottle',
        prop = 'water',
        disable = { combat = true, sprint = true },
        usetime = 2500,
        cancel = true,
        notifTitle = 'Gulp',
        notification = 'Nothing like a spicy sprite!',
		}
	},
  ['sprunk'] = {
		label = 'Sprunk',
		weight = 350,
		allowArmed = true,
		client = {
			status = { thirst = 20 },
			anim = 'drinking can',
			prop = 'sprunk',
			disable = {
				combat = true,
				sprint = true
			},
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'You quenched your thirst with a sprunk',
		}
	},
	['ecola'] = {
    label = 'eCola',
    weight = 10,
    stack = true,
    close = true,
    description = 'A Yummy Soda',
    client = {
			status = { thirst = 20 },
			anim = 'drinking can',
			prop = 'cola',
			disable = {
				combat = true,
				sprint = true
			},
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'You quenched your thirst with an eCola',
		}
  },
	--#endregion

	--#region WATER/JUICE/MILK
  ['water'] = {
		label = 'Water',
		weight = 500,
		stack = true,
		close = true,
		description = "For all the thirsty out there",
		client = {
			status = { thirst = 20 },
			anim = 'drinking bottle',
			prop = 'water',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'Your thirst is quenched by fresh, crisp water',
		}
		-- server = {
		-- 	export = 'bw_consumables.server:useWater'
		-- }
	},
  ["water_bottle"] = {
		label = "Bottle of Water",
		weight = 500,
		stack = true,
		close = true,
		description = "For all the thirsty out there",
		client = {
			status = { thirst = 20 },
			anim = 'drinking bottle',
			prop = 'water',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'Your thirst is quenched by fresh, crisp water',
		}
	},
	["grapejuice"] = {
		label = "Grape Juice",
		weight = 200,
		stack = true,
		close = true,
		description = "Grape juice is said to be healthy",
		client = {
			status = { thirst = 15 },
      anim = 'drinking bottle',
			prop = 'water',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Gulp',
			notification = 'You hear a feint chirp in the distance',
		}
	},
	["milk"] = {
		label = "Milk",
		weight = 500,
		stack = true,
		close = true,
		description = "Milk fresh from the farm!",
		client = {
			status = { hunger = 10, thirst = 10 },
			anim = 'drinking bottle',
			prop = 'milk',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger and thirst and satiated by natures perfect beverage.'
		},
		server = {
			export = 'bw_consumables.server:useHoney'
		}
	},
	["honey_milk"] = {
		label = "Honey Milk",
		weight = 500,
		stack = true,
		close = true,
		description = "Milk fresh from the farm with a hint of honey!",
		client = {
			status = { hunger = 50, thirst = 50, stress = -50 },
			anim = 'drinking bottle',
			prop = 'milk',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger and thirst and satiated by natures perfect beverage mixed with honey.'
		},
		server = {
			export = 'bw_consumables.server:useHoney'
		}
	},
	--#endregion

	--#region SHOTS
	['vodka_shot'] = {
    label = 'Shot of Vodka',
    weight = 250,
    close = true,
    consume = 0,
    server = {
        export = 'rcore_drunk.vodka',
    },
		description = "May you be in heaven half an hour before the devil knows you're dead",
	},
	['whiskey_shot'] = {
		label = 'Shot of Whiskey',
		weight = 250,
		close = true,
		consume = 0,
		description = "May your glass be ever full!",
		server = {
				export = 'rcore_drunk.whiskey_shot',
		},
	},
	['voodoo'] = {
		label = 'Shot of Voodoo',
		weight = 250,
		close = true,
		consume = 0,
		description = "Bottoms up!",
		server = {
				export = 'rcore_drunk.voodoo',
		},
	},
	['woowoo'] = {
		label = 'Shot of Woowoo',
		weight = 250,
		close = true,
		consume = 0,
		description = "Bottoms up!",
		server = {
				export = 'rcore_drunk.woowoo',
		},
	},
	['brussian'] = {
		label = 'Brussian Shot',
		weight = 250,
		close = true,
		consume = 0,
		description = "Bottoms up!",
		server = {
				export = 'rcore_drunk.brussian',
		},
	},
	['cappucc'] = {
		label = 'Shot of Cappucc',
		weight = 250,
		close = true,
		consume = 0,
		description = "Bottoms up!",
		server = {
				export = 'rcore_drunk.cappucc',
		},
	},
	['iflag'] = {
		label = 'Shot of Ireland',
		weight = 250,
		close = true,
		consume = 0,
		description = "May your troubles be less, and your blessings be more!",
		server = {
				export = 'rcore_drunk.iflag',
		},
	},
	['b52'] = {
		label = 'B52 Shot',
		weight = 250,
		close = true,
		consume = 0,
		description = "May your troubles be less, and your blessings be more!",
		server = {
				export = 'rcore_drunk.b52',
		},
	},
	--#endregion

	--#region BOTTLES
	['vodka'] = {
    label = 'Vodka',
    weight = 250,
    close = true,
    consume = 0,
    server = {
        export = 'rcore_drunk.vodka',
    },
		description = "A Russian once told me that all he needs in life is vodka and pickles.",
	},
	['whiskey'] = {
		label = 'Whiskey',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.whiskey',
		},
		description = "Buckle up cowboy! This ain't you pappys liquor.",
	},
	['tequila'] = {
		label = 'Tequila',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.tequila',
		},
		description = "A bit of salt, some lime, and you are set.",
	},
	['rum'] = {
		label = 'Rum',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.rum',
		},
		description = "Yarr better be ready to drive after this one!",
	},
	['nineteenfourtytwo'] = {
		label = '1942',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.nineteenfourtytwo',
		},
		description = "Is it for the clout or...?",
	},
	['amaretto'] = {
		label = 'Amaretto',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.amaretto',
		},
		description = "For all the thirsty out there",
	},
	['gin'] = {
		label = 'Gin',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.gin',
		},
		description = "Sippin' on gin and juice!",
	},
	--#endregion

	--#region BOTTLED WINE
	['housered'] = {
		label = 'Red Wine',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.housered',
		},
		description = "A classy red wine.",
	},
	['housewhite'] = {
		label = 'White Wine',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.housewhite',
		},
		description = "A classy white wine.",
	},
	['barbera'] = {
		label = 'Barbera Fine Red Wine',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.barbera',
		},
		description = "A robust red with notes of oak, walnut, dark chocolate and a hint of deez.",
	},
	['rosso'] = {
		label = 'Rosso Fine Red Wine',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.rosso',
		},
		description = "A delicate red that truly sticks to the palette.",
	},
	['vinewoodrose'] = {
		label = 'Vinewood Rose Wine',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.vinewoodrose',
		},
		description = "A wonderful blend of vinewoods best red and white grapes.",
	},
	--#endregion

	--#region BEER
	['beer'] = {
		label = 'Beer',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.ambeer',
		},
		description = "Chuck it out!",
	},
	['ambeer'] = {
		label = 'A.M. Beer',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.ambeer',
		},
		description = "Nothing like the hair of the dog!",
	},
	['blarneys'] = {
		label = "Blarney's",
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.blarneys',
		},
		description = "Nothing like an ice cold blarney's!",
	},
	['corona'] = {
		label = 'Corona Extra',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.corona',
		},
		description = "A slice of lime brings it all together.",
	},
	['pisswaser'] = {
		label = 'Pisswaser',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.pisswaser',
		},
		description = "I guess when you are thirsty, you really are thirsty.",
	},
	['stellaartois'] = {
		label = 'Stella Artois',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.stellaartois',
		},
		description = "Nothing like an ice cold stella!",
	},
	['logger'] = {
		label = 'Logger',
		weight = 250,
		close = true,
		consume = 0,
		server = {
				export = 'rcore_drunk.logger',
		},
		description = "Nothing like an ice cold lager!",
	},
	--#endregion

	--#region WINE GLASSES
	['wine_glass'] = {
			label = 'Glass of Wine',
			weight = 250,
			close = true,
			description = "Some good wine to drink on a fine evening",
			consume = 0,
			server = {
					export = 'rcore_drunk.wine_glass',
			},
	},
	--#endregion

	--#region MIXED DRINKS
	['orangepaloma'] = {
		label = 'Orange Paloma Cocktail',
		weight = 250,
		close = true,
		description = "Some good wine to drink on a fine evening",
		consume = 0,
		server = {
				export = 'rcore_drunk.orangepaloma',
		},
	},
	['kamikaze'] = {
		label = 'Kamikaze Cocktail',
		weight = 250,
		close = true,
		description = "Some good wine to drink on a fine evening",
		consume = 0,
		server = {
				export = 'rcore_drunk.kamikaze',
		},
	},
	['peach_raspberry_oats'] = {
		label = 'Peach Raspberry Oat Cocktail',
		weight = 250,
		close = true,
		description = "Some good wine to drink on a fine evening",
		consume = 0,
		server = {
				export = 'rcore_drunk.peach_raspberry_oats',
		},
	},
	['yoshishooter'] = {
		label = 'Yoshi Shooter Cocktail',
		weight = 250,
		close = true,
		description = "Some good wine to drink on a fine evening",
		consume = 0,
		server = {
				export = 'rcore_drunk.yoshishooter',
		},
	},
	['vitodaiquiri'] = {
		label = "Strawberry Daiquiri",
		weight = 250,
		close = true,
		description = "Some good wine to drink on a fine evening",
		consume = 0,
		server = {
				export = 'rcore_drunk.vitodaiquiri',
		},
	},
	['pinacolada'] = {
		label = "Pina Colada Cocktail",
		weight = 250,
		close = true,
		description = "Pineapple, coconut and rum? Yes please!",
		consume = 0,
		server = {
				export = 'rcore_drunk.pinacolada',
		},
	},
	--#endregion

	--#region MINIGAME DRINK
	['supervodka'] = {
			label = 'Super Vodka',
			weight = 250,
			close = true,
			consume = 0,
			description = "Even Russians don't touch this stuff.",
			server = {
					export = 'rcore_drunk.supervodka',
			},
	},
	--#endregion
}
```
