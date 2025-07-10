# Restaurants

- [Recipes](../recipes/recipes.md/#recipes)
- [Stations](../recipes/stations.md/#stations)

- [Drinks Items](./drinks.md/#drinks)
- [Food Items](./food.md/#food)

- [Back to Items](../restaurants.md)
- [Back to Main](../../README.md)

```lua
return {
	["receipt"] = {label = "Receipt", weight = 1, stack = true, close = true },

	--#region BREAD/GRAINS
	['sdft_bun'] = {
    label = 'Burger Bun',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a burger bun'
  },
	['sdft_bun_cooked'] = {
    label = 'Toasted Bun',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a toasted bun'
  },
	['sdft_hotdogbun'] = {
    label = 'Hotdog Bun',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a hotdog bun'
  },
  ['sdft_hotdogbun_cooked'] = {
    label = 'Toasted Hotdog Bun',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a toasted hotdog bun'
  },
	['sdft_hoagie'] = {
    label = 'Hoagie',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a hoagie'
  },
  ['sdft_hoagie_cooked'] = {
    label = 'Toasted Hoagie',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a toasted hoagie'
  },
	['sdft_rawpretzel'] = {
    label = 'Raw Pretzel Dough',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some raw pretzel dough'
  },
  ['sdft_pretzel_cooked'] = {
    label = 'Cooked Pretzel',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a cooked pretzel'
  },
  ['sdft_minipretzel'] = {
    label = 'Raw Mini Pretzel',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a raw mini pretzel'
  },
  ['sdft_minipretzel_cooked'] = {
    label = 'Cooked Mini Pretzel',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a cooked mini pretzel'
  },
  ['sdft_torilla'] = {
    label = 'Torilla',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a tortilla'
  },
	["rice"] = {
		label = "Rice",
		weight = 0,
		stack = true,
		close = false,
		description = "Rice",
		client = {
			image = "rice.png",
		}
	},
	--#endregion

	-- RAW PRODUCE
	--#region veges
	['sdft_lettuce'] = {
    label = 'Lettuce',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some lettuce'
  },
	["onion"] = {
		label = "Onion",
		weight = 200,
		stack = true,
		close = true,
		description = "Fresh onion. Still smells like dirt.",
		client = {
			image = "onion.png",
			status = { hunger = 1 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious raw onion, but now you are crying.'
		},
		server = {
			export = 'bw_consumables.server:useFruit'
		}
	},
	["onions"] = {label = "Onions", weight = 1, stack = true, close = true, client = {image = 'onions.png',},},
	["potato"] = {label = "Potato", weight = 1, stack = true, close = true, client = {image = 'potato.png',},},
	["cabbage"] = {
		label = "Cabbage",
		weight = 700,
		stack = true,
		close = true,
		description = "Fresh cabbage. Still smells like dirt.",
		client = {
			image = "cabbage.png",
			status = { hunger = 1 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious raw cabbage.'
		},
		server = {
			export = 'bw_consumables.server:useFruit'
		}
	},
	["corn_crop"] = {
		label = "Corn on the Cob",
		weight = 150,
		stack = true,
		close = true,
		description = "Amazing corn still in the husk!",
		client = {
			image = "corn_crop.png",
			status = { hunger = 1 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious corn.'
		},
		server = {
			export = 'bw_consumables.server:useFruit'
		}
	},
	--#endregion

	--#region fruit
	["apple_red"] = {
		label = "Red Apple",
		weight = 200,
		stack = true,
		close = true,
		description = "A classic red apple!",
		client = {
			image = "apple_red.png",
			status = { hunger = 1 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious red apple.'
		},
		server = {
			export = 'bw_consumables.server:useFruit'
		}
	},
	["apple_green"] = {
		label = "Green Apple",
		weight = 200,
		stack = true,
		close = true,
		description = "A classic green apple!",
		client = {
			image = "apple_green.png",
			status = { hunger = 1 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious green apple.'
		},
		server = {
			export = 'bw_consumables.server:useFruit'
		}
	},
	["banana"] = {
		label = "Banana",
		weight = 150,
		stack = true,
		close = true,
		description = "A classic banana!",
		client = {
			image = "banana.png",
			status = { hunger = 5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious banana.'
		},
		server = {
			export = 'bw_consumables.server:useFruit'
		}
	},
	["blueberries"] = {
		label = "Blueberries",
		weight = 200,
		stack = true,
		close = true,
		description = "Beautiful blueberries!",
		client = {
			image = "blueberries.png",
			status = { hunger = 1 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious blueberries.'
		},
		server = {
			export = 'bw_consumables.server:useFruit'
		}
	},
	["yucca_fruit"] = {
		label = "Yucca Fruit",
		weight = 200,
		stack = true,
		close = true,
		description = "The fruit of the yucca tree. A delicacy!",
		client = {
			image = "yucca_fruit.png",
			status = { hunger = 1 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious yucca fruit.'
		},
		server = {
			export = 'bw_consumables.server:useFruit'
		}
	},
	["strawberry"] = {
		label = "Strawberry",
		weight = 30,
		stack = true,
		close = true,
		description = "Fresh strawberry straight off the vine.",
		client = {
			image = "strawberry.png",
			status = { hunger = 10 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious strawberry.'
		},
		server = {
			export = 'bw_consumables.server:useHoney'
		}
	},
	["orange"] = {
		label = "Orange",
		weight = 0,
		stack = true,
		close = false,
		description = "Orange",
	},
	["lemon"] = {
		label = "Lemon",
		weight = 60,
		stack = true,
		close = true,
		description = "Fresh, juicy lemon.",
		client = {
			image = "lemon.png",
			status = { hunger = 1 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious raw lemon.'
		},
		server = {
			export = 'bw_consumables.server:useFruit'
		}
	},
	["lime"] = {
		label = "Lime",
		weight = 60,
		stack = true,
		close = true,
		description = "Fresh, juicy lime.",
		client = {
			status = { hunger = 1 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious raw lime.'
		},
		server = {
			export = 'bw_consumables.server:useFruit'
		}
	},
	['tomato'] = {
    label = 'Tomato',
    weight = 10,
    stack = true,
    close = true,
    description = 'Knowledge is knowing a tomato is a fruit. Wisdom is knowing not to put it in a fruit salad.',
		client = {
			status = { hunger = 1 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious raw tomato.'
		},
		server = {
			export = 'bw_consumables.server:useFruit'
		}
  },
  ['sdft_tomato'] = {
    label = 'Sliced Tomato',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some sliced tomato'
  },
	--#endregion

	--#region other
	['sdft_cheese'] = {
    label = 'Cheese Slice',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a cheese slice'
  },
	['sdft_shreddedcheese'] = {
    label = 'Shredded Cheese',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some shredded cheese'
  },
	['sdft_cheesesauce'] = {
    label = 'Cheese Sauce',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some cheese sauce'
  },
	["egg_raw"] = {
		label = "Raw Egg",
		weight = 55,
		stack = true,
		close = true,
		description = "Fresh eggs! Is that... poo?",
		client = {
			image = "egg_raw.png",
			status = { hunger = 1 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious raw egg.'
		},
		server = {
			export = 'bw_consumables.server:useHoney'
		}
	},
	["honey"] = {
		label = "Honey",
		weight = 300,
		stack = true,
		close = true,
		description = "Delicious honey, fresh from the flowers of Beenwell.",
		client = {
			image = "honey.png",
			status = { hunger = 5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious honey.'
		},
		server = {
			export = 'bw_consumables.server:useHoney'
		}
	},
	--#endregion

	--#region RAW RED MEAT
  ['sdft_patty'] = {
    label = 'Raw Patty',
    weight = 110,
    stack = true,
    close = true,
    description = 'Just a raw patty'
  },
	['sdft_vpatty'] = {
    label = 'Raw Veggie Patty',
    weight = 110,
    stack = true,
    close = true,
    description = 'Just a raw veggie patty'
  },
	['sdft_dog'] = {
    label = 'Raw Dog',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a raw dog'
  },
	['sdft_sausage'] = {
    label = 'Raw Sausage',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some raw sausage'
  },
	['sdft_bacon'] = {
    label = 'Raw Bacon',
    weight = 65,
    stack = true,
    close = true,
    description = 'Just some raw bacon'
  },
	['sdft_carneasada'] = {
    label = 'Raw Carne Asada',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some raw carne asada'
  },
  ['sdft_elpastor'] = {
    label = 'Raw El Pastor',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some raw el pastor'
  },
	--#endregion

	--#region RAW WHITE MEAT
	["raw_chicken"] = {
		label = "Raw Chicken",
		weight = 0,
		stack = true,
		close = false,
		description = "Raw Chicken",
		client = {
			image = "raw_chicken.png",
		}
	},
	--#endregion

	--#region RAW FISH
	["raw_fish"] = {
		label = "Raw Fish",
		weight = 0,
		stack = true,
		close = false,
		description = "Raw Fish",
		client = {
			image = "raw_fish.png",
		}
	},
	--#endregion

	--#region COOKED RED MEAT
  ['sdft_patty_cooked'] = {
    label = 'Cooked Patty',
    weight = 100,
    stack = true,
    close = true,
    description = 'Just a cooked patty'
  },
	['sdft_vpatty_cooked'] = {
    label = 'Cooked Veggie Patty',
    weight = 100,
    stack = true,
    close = true,
    description = 'Just a cooked veggie patty'
  },
	['sdft_dog_cooked'] = {
    label = 'Cooked Dog',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a cooked dog'
  },
  ['sdft_sausage_cooked'] = {
    label = 'Cooked Sausage',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some cooked sausage'
  },
	['sdft_bacon_cooked'] = {
    label = 'Cooked Bacon',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some cooked bacon'
  },
	['sdft_carneasada_cooked'] = {
    label = 'Cooked Carne Asada',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some cooked carne asada'
  },
  ['sdft_elpastor_cooked'] = {
    label = 'Cooked El Pastor',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some cooked el pastor'
  },
	--#endregion

	--#region COOKED WHITE MEAT
	["cooked_chicken"] = {
		label = "Cooked Chicken",
		weight = 0,
		stack = true,
		close = false,
		description = "Cooked Chicken",
		client = {
			image = "cooked_chicken.png",
		},
	},
	--#endregion

	--#region COOKED FISH
	["cooked_fish"] = {
		label = "Cooked Fish",
		weight = 0,
		stack = true,
		close = false,
		description = "Cooked Fish",
		client = {
			image = "cooked_fish.png",
		}
	},
	--#endregion

	--#region BURGERS
	['sdft_burger'] = {
    label = 'Burger',
    weight = 225,
    stack = true,
    close = true,
    description = 'Just a Burger',
		client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -15, hunger = 95 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'A simple burger. Perfect for a quick bite.',
		}
  },
  ['sdft_megacheese'] = {
    label = 'Mega Cheese Burger',
    weight = 235,
    stack = true,
    close = true,
    description = 'A Super Cheesy Burger',
		client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -15, hunger = 95 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		}
  },
  ['sdft_doubleburger'] = {
    label = 'Double Burger',
    weight = 300,
    stack = true,
    close = true,
    description = 'A Double Burger',
		consume = 0.5,
		client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -15, hunger = 95 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		}

  },
  ['sdft_kingsizeburger'] = {
    label = 'King Size Burger',
    weight = 400,
    stack = true,
    close = true,
    description = 'A Huge Burger',
		consume = 0.25,
		client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -15, hunger = 95 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_baconburger'] = {
    label = 'Bacon Burger',
    weight = 230,
    stack = true,
    close = true,
    description = 'A Bacon Burger',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -15, hunger = 95 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_meatfree'] = {
    label = 'Meat Free Burger',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just A Meat Free Burger',
		client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -20, hunger = 20, thirst = 5 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_heartstopper'] = {
    label = 'Heartstopper Burger',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just A Heartstopper Burger',
		client = {
			anim = "eating burger",
			prop = "brum_burgershot_doubleshot",
			status = { stress = -25, hunger = 50 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
		consume = 0.5,
  },
  ['sdft_bleeder'] = {
    label = 'Bleeder Burger',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just A Bleeder Burger',
		client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -15, hunger = 25 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_moneyshot'] = {
    label = 'Money Shot Burger',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just A Money Shot Burger',
		client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -15, hunger = 25 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_torpedo'] = {
    label = 'Torpedo Burger',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just A Torpedo Burger',
		client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -15, hunger = 25 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
	--#endregion

	--#region HOTDOGS
	['sdft_hotdog'] = {
    label = 'Hotdog',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a Tasty Dog',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -15, hunger = 25 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_sausagedog'] = {
    label = 'Sausage Dog',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a Sausage Dog',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -15, hunger = 25 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
	--#endregion

	--#region PIZZA
	['sdft_pizzaslice'] = {
    label = 'Pizza Slice',
    weight = 10,
    stack = true,
    close = true,
    description = 'Yummy Pizza',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 15 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
	--#endregion

	--#region TACOS
	['sdft_taco_carneasada'] = {
    label = 'Carne Asada Taco',
    weight = 10,
    stack = true,
    close = true,
    description = 'Taco With Carne Asada',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 20 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_taco_elpastor'] = {
    label = 'El Pastor Taco',
    weight = 10,
    stack = true,
    close = true,
    description = 'Taco With El Pastor',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 20 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
	--#endregion

	--#region TORTAS
	['sdft_torta_carneasada'] = {
    label = 'Carne Asada Torta',
    weight = 10,
    stack = true,
    close = true,
    description = 'Torta With Carne Asada',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 20 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_torta_elpastor'] = {
    label = 'El Pastor Torta',
    weight = 10,
    stack = true,
    close = true,
    description = 'Torta With El Pastor',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 20 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
	--#endregion

	--#region BURRITOS
	['sdft_burrito_carneasada'] = {
    label = 'Carne Asada Burrito',
    weight = 10,
    stack = true,
    close = true,
    description = 'Burrito With Carne Asada',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 20 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_burrito_elpastor'] = {
    label = 'El Pastor Burrito',
    weight = 10,
    stack = true,
    close = true,
    description = 'Burrito With El Pastor',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 20 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
	--#endregion

	--#region QUESADILLAS
	['sdft_quesadilla'] = {
    label = 'Quesadilla',
    weight = 10,
    stack = true,
    close = true,
    description = 'A Tasty Quesadilla',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 20 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_tostada'] = {
    label = 'Tostada',
    weight = 10,
    stack = true,
    close = true,
    description = 'A Tasty Tostada',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 20 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
	--#endregion

	--#region CHICKEN DISHES
	["orange_chicken"] = {
		label = "Orange Chicken",
		weight = 0,
		stack = true,
		close = false,
		description = "Orange Chicken",
		client = {
			image = "orange_chicken.png",
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = nil,
			usetime = 2500,
		},
		consume = 1.0,
	},
	--#endregion

	--#region FISH DISHES
	["fish_taco"] = {
		label = "Fish Taco",
		weight = 0,
		stack = true,
		close = false,
		description = "Fish Taco",
		client = {
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = nil,
			usetime = 2500,
		},
		consume = 1.0,
	},
	--#endregion

	--#region SUSHI
	["sushi"] = {
		label = "Sushi",
		weight = 0,
		stack = true,
		close = false,
		description = "Sushi",
		client = {
			image = "sushi.png",
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = nil,
			usetime = 2500,
			notification = 'I really hope that was sushi-grade salmon...'
		},
		consume = 1.0,
	},
	--#endregion

	--#region SIDE DISHES
  ['sdft_fries'] = {
    label = 'Fries',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just Some Fries',
		consume = 0.5,
		client = {
			anim = "eating snack",
			prop = "chips",
			status = { stress = -10, hunger = 30 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Delicious, hot and salty french fries!',
		}
  },
	["basket_fries"] = {
		label = "Basket of French Fries",
		weight = 200,
		stack = true,
		close = true,
		description = "Fried, salted potato sticks in a basket.",
		consume = 0.25,
		client = {
			status = { hunger = 30, stress = -10 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'The perfect side for any burger.'
		},
	},
	["fried_rice"] = {
		label = "Fried Rice",
		weight = 0,
		stack = true,
		close = false,
		description = "Fried Rice",
		client = {
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = nil,
			usetime = 2500,
		},
		consume = 1.0,
	},
	['sdft_pretzel'] = {
    label = 'Pretzel',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a Yummy Pretzel',
		client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 15 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_minipretzels'] = {
    label = 'Mini Pretzels',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just 3 Mini Pretzels',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 15 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_roastednuts'] = {
    label = 'Roasted Nuts',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just Some Roasted Nuts',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 15 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
	['sdft_nuts'] = {
    label = 'Nuts',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some nuts'
  },
  ['sdft_nuts_cooked'] = {
    label = 'Roasted Nuts',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some roasted nuts',
		client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 15 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
	['sdft_donut'] = {
    label = 'Donut',
    weight = 10,
    stack = true,
    close = true,
    description = 'A Large Donut',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 15 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
	['sdft_rawdonut'] = {
    label = 'Donut Dough',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some donut dough'
  },
  ['sdft_donut_cooked'] = {
    label = 'Donut',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a donut',
		client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 15 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
	--#endregion

	--#region CONDIMENTS
	['mustard'] = {
		label = 'Mustard',
		weight = 550,
		client = {
			image = 'mustard.png',
			status = { hunger = 5, thirst = 5 },
			anim = 'drinking bottle',
			prop = 'mustard',
			usetime = 2500,
			notifTitle = 'Gross',
			notification = 'You.. drank mustard',
			disable = {
				combat = true,
				sprint = true
			},
			cancel = true,
		}
	},
	--#endregion

	--#region FROZEN FOODS
	['sdft_rawfries'] = {
    label = 'Frozen Fries',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some frozen fries'
  },
  ['sdft_pizza'] = {
    label = 'Frozen Pizza',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a frozen pizza'
  },
	--#endregion

	--#region FROZEN FOODS COOKED
	['sdft_fries_cooked'] = {
    label = 'Cooked Fries',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just some cooked fries',
		client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 15 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_pizza_cooked'] = {
    label = 'Cooked Pizza',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just a cooked pizza',
		client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 15 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
	--#endregion

	--#region BEVERAGES
	['sdft_milkshake'] = {
    label = 'Milkshake',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just A Milkshake',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 10, thirst = 20 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
  ['sdft_smoothie'] = {
    label = 'Smoothie',
    weight = 10,
    stack = true,
    close = true,
    description = 'Just A Smoothie',
    client = {
			anim = "eating burger",
			prop = "burger",
			status = { stress = -10, hunger = 10, thirst = 20 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Super satisfying!',
		},
  },
	--#endregion

	-- note: just need to add photos for all items, and config for restaurants
	--#region Brum Foods
	['atomshake_chocolate'] = {
			label = 'Chocolate Milkshake',
			weight = 8,
			stack = true,
			close = true,
			consume = 0.5,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 95, hunger = 15 },
					anim = 'drinking can',
					prop = 'brum_sunday_chocolate',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Sluuurrpp',
					notification = 'Choccy Milkshake satisfies your cravings!'
			}
	},
	['atomshake_rainbow'] = {
			label = 'Rainbow Milkshake',
			weight = 500,
			stack = true,
			close = true,
			consume = 0.5,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 95, hunger = 15 },
					anim = 'drinking can',
					prop = 'brum_sunday_rainbow',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Sluuurrpp',
					notification = 'Rainbow milkshake satisfies your cravings!'
			}
		},
	['atomshake_strawberry'] = {
			label = 'Strawberry Milkshake',
			weight = 500,
			stack = true,
			close = true,
			consume = 0.5,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 95, hunger = 15 },
					anim = 'drinking can',
					prop = 'brum_sunday_strawberry',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Sluuurrpp',
					notification = 'Strawberry milkshake satisfies your cravings!'
			}
	},
	['atomshake_vanilla'] = {
			label = 'Vanilla Milkshake',
			weight = 500,
			stack = true,
			close = true,
			consume = 0.5,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 95, hunger = 15 },
					anim = 'drinking can',
					prop = 'brum_sunday_vanilla',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Sluuurrpp',
					notification = 'Vanilla milkshake satisfies your cravings!'
			}
	},
	['atom_double'] = { -- double burger
    label = 'Atom Double Double',
    weight = 300,
    stack = true,
    close = true,
    description = 'A double stack burger.',
		consume = 0.5,
    buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Hamburger', 'You lick the burger like a fiend.', 4000, 'info', false)
				end
			},
			{
				label = 'Place',
				action = function(slot)
					exports['kq_placeable_items']:placeItem(slot)
				end
			}
		},
		client = {
			status = { hunger = 95 },
			anim = 'eating burger',
			prop = 'brum_burgershot_doubleshot',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Up \'n\' Atom really outdid themselves with this one!'
		},
  },
	['atom_vegan'] = { -- vegan burger
    label = 'Atom Simply Vegan',
    weight = 225,
    stack = true,
    close = true,
    description = 'A simple vegan burger made of... I never asked.',
		consume = 0.5,
    buttons = {
        {
            label = 'Lick it',
            action = function(slot)
                exports['okokNotify']:Alert('Hamburger', 'You lick the burger like a fiend.', 4000, 'info', false)
            end
        },
        {
            label = 'Place',
            action = function(slot)
                exports['kq_placeable_items']:placeItem(slot)
            end
        }
    },
    client = {
        status = { hunger = 95 },
        anim = 'eating burger',
        prop = 'brum_burgershot_simply',
        disable = { combat = true, sprint = false },
        usetime = 2500,
        cancel = true,
        notifTitle = 'Nom nom',
        notification = 'A simple burger hits the spot.'
    },
	},
	['atomfries_large'] = {
			label = 'Large Fries',
			weight = 250,
			stack = true,
			close = true,
			consume = 0.25,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Fries', 'You lick the fries... salty!', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { hunger = 35 },
					anim = 'eating snack',
					prop = 'brum_fries_large',
					disable = { combat = true, sprint = false },
					usetime = 2500,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Crispy and golden large fries!'
			},
	},
	['atomfries_medium'] = {
			label = 'Medium Fries',
			weight = 190,
			stack = true,
			close = true,
			consume = 0.5,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Fries', 'You lick the fries... salty!', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { hunger = 35, thirst = -3 },
					anim = 'eating snack',
					prop = 'brum_fries_medium',
					disable = { combat = true, sprint = false },
					usetime = 2500,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Perfect medium-sized fries!'
			},
	},
	['atomfries_small'] = {
			label = 'Small Fries',
			weight = 130,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Fries', 'You lick the fries... salty!', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { hunger = 35 },
					anim = 'eating snack',
					prop = 'brum_fries_small',
					disable = { combat = true, sprint = false },
					usetime = 2000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Small but tasty fries!'
			},
	},
	['atomsoda_large'] = {
			label = 'Large Drink',
			weight = 300,
			stack = true,
			close = true,
			consume = 0.25,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Drink', 'You lick the cup rim... refreshing?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 50 },
					anim = 'drinking can',
					prop = 'brum_tcup_large',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Glug glug',
					notification = 'Large drink quenches your thirst!'
			},
	},
	['atomsoda_small'] = {
			label = 'Small Drink',
			weight = 150,
			stack = true,
			close = true,
			consume = 0.5,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Drink', 'You lick the cup rim... refreshing?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 50 },
					anim = 'drinking can',
					prop = 'brum_tcup_small',
					disable = { combat = true, sprint = false },
					usetime = 2000,
					cancel = true,
					notifTitle = 'Glug glug',
					notification = 'Small sip of refreshment!'
			},
	},
	['atom_bag'] = {
		label = 'Up \'n\' Atom Bag',
		weight = 100,
		stack = false,
		close = false,
		consume = 0,
		description = 'A small bag used to hold items from the famous Up \'n\' Atom.',
		buttons = {{ label = 'Place', action = function(slot) exports['kq_placeable_items']:placeItem(slot) end }},
	},

	['brum_fastfoodbox_small'] = {
			label = 'Small Fast Food Box',
			weight = 15,
			stack = true,
			close = true,
			consume = 0,
			buttons = {
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
	},
	['brum_tub_ketchup'] = {
			label = 'Ketchup Tub',
			weight = 5,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Ketchup', 'You lick the ketchup... sweet and tangy!', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { hunger = 5, thirst = 5 },
					anim = 'drinking bottle',
					prop = 'brum_tub_ketchup',
					disable = { combat = true, sprint = false },
					usetime = 2000,
					cancel = true,
					notifTitle = 'Squirt',
					notification = 'Pure ketchup goodness!'
			},
	},
	--#endregion

	--#region Brum Drinks
	-- icecream cups
	['brum_icecreamcup_berrry'] = {
			label = 'Icecreamcup Berrry',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_icecreamcup_berrry',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Icecreamcup Berrry satisfies your cravings!'
			}
	},
	['brum_icecreamcup_caramel'] = {
			label = 'Icecreamcup Caramel',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_icecreamcup_caramel',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Icecreamcup Caramel satisfies your cravings!'
			}
	},
	['brum_icecreamcup_lemon_vanilla'] = {
			label = 'Icecreamcup Lemon Vanilla',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_icecreamcup_lemon_vanilla',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Icecreamcup Lemon Vanilla satisfies your cravings!'
			}
	},
	['brum_icecreamcup_rainbow'] = {
			label = 'Icecreamcup Rainbow',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_icecreamcup_rainbow',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Icecreamcup Rainbow satisfies your cravings!'
			}
	},
	['brum_icecreamcup_strawberry'] = {
			label = 'Icecreamcup Strawberry',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_icecreamcup_strawberry',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Icecreamcup Strawberry satisfies your cravings!'
			}
	},
	['brum_icecreamcup_strawberrybanana'] = {
			label = 'Icecreamcup Strawberrybanana',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_icecreamcup_strawberrybanana',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Icecreamcup Strawberrybanana satisfies your cravings!'
			}
	},
	['brum_icecreamcup_vanilla'] = {
			label = 'Icecreamcup Vanilla',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_icecreamcup_vanilla',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Icecreamcup Vanilla satisfies your cravings!'
			}
	},
	-- macaroons
	['brum_macaroon_berry'] = {
			label = 'Macaroon Berry',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_berry',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Berry satisfies your cravings!'
			}
	},
	['brum_macaroon_berrytray'] = {
			label = 'Macaroon Berrytray',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_berrytray',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Berrytray satisfies your cravings!'
			}
	},
	['brum_macaroon_blueberry'] = {
			label = 'Macaroon Blueberry',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_blueberry',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Blueberry satisfies your cravings!'
			}
	},
	['brum_macaroon_blueberrytray'] = {
			label = 'Macaroon Blueberrytray',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_blueberrytray',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Blueberrytray satisfies your cravings!'
			}
	},
	['brum_macaroon_chocolate'] = {
			label = 'Macaroon Chocolate',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_chocolate',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Chocolate satisfies your cravings!'
			}
	},
	['brum_macaroon_chocolatetray'] = {
			label = 'Macaroon Chocolatetray',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_chocolatetray',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Chocolatetray satisfies your cravings!'
			}
	},
	['brum_macaroon_lemon'] = {
			label = 'Macaroon Lemon',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_lemon',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Lemon satisfies your cravings!'
			}
	},
	['brum_macaroon_lemontray'] = {
			label = 'Macaroon Lemontray',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_lemontray',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Lemontray satisfies your cravings!'
			}
	},
	['brum_macaroon_lime'] = {
			label = 'Macaroon Lime',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_lime',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Lime satisfies your cravings!'
			}
	},
	['brum_macaroon_limetray'] = {
			label = 'Macaroon Limetray',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_limetray',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Limetray satisfies your cravings!'
			}
	},
	['brum_macaroon_mixedtray'] = {
			label = 'Macaroon Mixedtray',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_mixedtray',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Mixedtray satisfies your cravings!'
			}
	},
	['brum_macaroon_orange'] = {
			label = 'Macaroon Orange',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_orange',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Orange satisfies your cravings!'
			}
	},
	['brum_macaroon_orangetray'] = {
			label = 'Macaroon Orangetray',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_orangetray',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Orangetray satisfies your cravings!'
			}
	},
	['brum_macaroon_strawberry'] = {
			label = 'Macaroon Strawberry',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_strawberry',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Strawberry satisfies your cravings!'
			}
	},
	['brum_macaroon_strawberrytray'] = {
			label = 'Macaroon Strawberrytray',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 10, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_macaroon_strawberrytray',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Macaroon Strawberrytray satisfies your cravings!'
			}
	},
	['brum_sunday_berry'] = {
			label = 'Sunday Berry',
			weight = 8,
			stack = true,
			close = true,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 95, hunger = 15 },
					anim = 'eating burger',
					prop = 'brum_sunday_berry',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Nom nom',
					notification = 'Sunday Berry satisfies your cravings!'
			}
	},
	-- sundaes
	['brum_sunday_chocolate'] = {
			label = 'Sunday Chocolate',
			weight = 8,
			stack = true,
			close = true,
			consume = 0.5,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 95, hunger = 15 },
					anim = 'drinking can',
					prop = 'brum_sunday_chocolate',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Sluuurrpp',
					notification = 'Sunday Chocolate satisfies your cravings!'
			}
	},
	['brum_sunday_luxury_caramel'] = {
			label = 'Sunday Luxury Caramel',
			weight = 8,
			stack = true,
			close = true,
			consume = 0.5,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 95, hunger = 15 },
					anim = 'drinking can',
					prop = 'brum_sunday_luxury_caramel',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Sluuurrpp',
					notification = 'Sunday Luxury Caramel satisfies your cravings!'
			}
	},
	['brum_sunday_luxury_strawberry'] = {
			label = 'Sunday Luxury Strawberry',
			weight = 500,
			stack = true,
			close = true,
			consume = 0.5,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 95, hunger = 15 },
					anim = 'drinking can',
					prop = 'brum_sunday_luxury_strawberry',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Sluuurrpp',
					notification = 'Sunday Luxury Strawberry satisfies your cravings!'
			}
	},
	['brum_sunday_rainbow'] = {
			label = 'Sunday Rainbow',
			weight = 500,
			stack = true,
			close = true,
			consume = 0.5,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 95, hunger = 15 },
					anim = 'drinking can',
					prop = 'brum_sunday_rainbow',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Sluuurrpp',
					notification = 'Sunday Rainbow satisfies your cravings!'
			}
	},
	['brum_sunday_raspberry_ripple'] = {
			label = 'Sunday Raspberry Ripple',
			weight = 500,
			stack = true,
			close = true,
			consume = 0.5,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 95, hunger = 15 },
					anim = 'drinking can',
					prop = 'brum_sunday_raspberry_ripple',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Sluuurrpp',
					notification = 'Sunday Raspberry Ripple satisfies your cravings!'
			}
	},
	['brum_sunday_strawberry'] = {
			label = 'Sunday Strawberry',
			weight = 500,
			stack = true,
			close = true,
			consume = 0.5,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 95, hunger = 15 },
					anim = 'drinking can',
					prop = 'brum_sunday_strawberry',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Sluuurrpp',
					notification = 'Sunday Strawberry satisfies your cravings!'
			}
	},
	['brum_sunday_vanilla'] = {
	label = 'Sunday Vanilla',
			weight = 500,
			stack = true,
			close = true,
			consume = 0.5,
			buttons = {
					{
							label = 'Lick it',
							action = function(slot)
									exports['okokNotify']:Alert('Eat', 'You lick it... tasty?', 4000, 'info', false)
							end
					},
					{
							label = 'Place',
							action = function(slot)
									exports['kq_placeable_items']:placeItem(slot)
							end
					}
			},
			client = {
					status = { thirst = 95, hunger = 15 },
					anim = 'drinking can',
					prop = 'brum_sunday_vanilla',
					disable = { combat = true, sprint = false },
					usetime = 3000,
					cancel = true,
					notifTitle = 'Sluuurrpp',
					notification = 'Sunday Vanilla satisfies your cravings!'
			}
	},
	--#endregion
}
```
