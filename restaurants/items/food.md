# Food

- [Recipes](../recipes/recipes.md/#recipes)
- [Stations](../recipes/stations.md/#stations)

- [Drinks Items](./drinks.md/#drinks)
- [Restaurant Items](./restaurants.md/#restaurants)

- [Back to Items](../restaurants.md)
- [Back to Main](../../README.md)

```lua
return {
	--#region POTATO/CORN CHIPS
  ["hot_cheetos"] = {
		label = "Hot Cheetos",
		weight = 100,
		stack = true,
		close = true,
		description = "Who cares about a little red40?",
		client = {
			anim = "eating snack",
			prop = "chips",
			status = { stress = -2, hunger = 10 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Delicious hot cheetos! A classic.',
		}
	},
  ["hot_cheetos_lime"] = {
		label = "Lime Hot Cheetos",
		weight = 100,
		stack = true,
		close = true,
		description = "Spice with lime, a cultural classic.",
		client = {
			anim = "eating snack",
			prop = "chips",
			status = { stress = -2, hunger = 15 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Put the lime in the hot cheetos? Hell yeah.',
		}
	},
  ["doritos"] = {
		label = "Doritos",
		weight = 100,
		stack = true,
		close = true,
		description = "I heard these are good for starting fires",
		client = {
			anim = "eating snack",
			prop = "chips",
			status = { stress = -2, hunger = 10 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'You knew just one was not an option',
		}
	},
  ["lays_original"] = {
		label = "Lays Original",
		weight = 100,
		stack = true,
		close = true,
		description = "Thinly sliced potato fried to a crisp. Simply delicious.",
		client = {
			anim = "eating snack",
			prop = "chips",
			status = { stress = -2, hunger = 10 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'This would pair perfectly with a sandwich.',
		}
	},
  ["lays_sourcream"] = {
		label = "Lays Sour Cream & Onion",
		weight = 100,
		stack = true,
		close = true,
		description = "A chip with a dip flavor. Ingenious!",
		client = {
			anim = "eating snack",
			prop = "chips",
			status = { stress = -2, hunger = 15 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'The thought of devouring another bag plagues your mind.',
		}
	},
	["lays_bbq"] = {
		label = "Lays Barbecue",
		weight = 100,
		stack = true,
		close = true,
		description = "Crispy, savory potato chips seasoned with a bold and smoky barbecue flavor, perfect for snacking anytime.",
		client = {
			anim = "eating snack",
			prop = "chips",
			status = { stress = -2, hunger = 10 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'I heard these pair well with a dab of A1.',
		}
	},
  ["sunchips_cheddar"] = {
		label = "Sunchips Harvest Cheddar",
		weight = 100,
		stack = true,
		close = true,
		description = "A delicious hint of cheddar cheese in each bite",
		client = {
			anim = "eating snack",
			prop = "chips",
			status = { stress = -2, hunger = 10 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'You toss the biodegradable, decomposable bag onto the floor with no worries about the environment',
		}
	},
	--#endregion

	--#region CANDY
  ["twerks_candy"] = {
		label = "Twerks Bar",
		weight = 50,
		stack = true,
		close = true,
		description = "A delicious combination of crunchy cookie, creamy caramel, and smooth milk chocolate in every irresistible bite.",
		allowArmed = true,
		client = {
			anim = "eating burger",
			prop = "twerks",
			status = { stress = -8, hunger = 10 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Twerks so good they make you wanna twerk',
		}
	},
  ["snikkel_candy"] = {
		label = "Snikkel Bar",
		weight = 50,
		stack = true,
		close = true,
		description = "A satisfying blend of roasted peanuts, gooey caramel, and nougat, all coated in rich milk chocolate for the perfect hunger-busting treat.",
		allowArmed = true,
		client = {
			anim = "eating burger",
			prop = "twerks",
			status = { stress = -8, hunger = 10 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Nothing like a good ole snikkel',
		}
	},
	["jail_breakers"] = {
		label = "Jail Breaker Bar",
		weight = 50,
		stack = true,
		close = true,
		description = "No longer allowed in commissary due to smuggling issues.",
		allowArmed = true,
		client = {
			anim = "eating burger",
			prop = "twerks",
			status = { stress = -2, hunger = 10 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'You feel like committing a felony.',
		}
	},
	["nerd_tats"] = {
		label = "Nerd Tats Candy",
		weight = 50,
		stack = true,
		close = true,
		description = "Put the tit back in that tat, and get your bullies back!",
		allowArmed = true,
		client = {
			anim = "eating snack",
			prop = "candy",
			status = { stress = -2, hunger = 10 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'You feel better as you pick the last bits of candy out of your teeth.',
		}
	},
	["sugar_butts"] = {
		label = "Sugar Butts Candy",
		weight = 50,
		stack = true,
		close = true,
		description = "Sugar butt, sugar butt, sugar sugar sugar sugar SUGAR BUTT! Ba-dum-dum-dum-dum.",
		allowArmed = true,
		client = {
			anim = "eating snack",
			prop = "candy",
			status = { stress = -10, hunger = 5 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'A sugar high brings you back to reality!',
		}
	},
	["rock_busters"] = {
		label = "Rock Busters Candy",
		weight = 50,
		stack = true,
		close = true,
		description = "Don't let Hunter get his hands on these rocks!",
		allowArmed = true,
		client = {
			anim = "eating snack",
			prop = "candy",
			status = { stress = -2, hunger = 10 },
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Delicious, chocolate bits rejuvenate your spirit.',
		}
	},
	["jolly_ranchers"] = {
		label = "Jolly Ranchers",
		weight = 50,
		stack = true,
		close = true,
		allowArmed = true,
		client = {
			status = { hunger = 3, stress = -3},
			anim = "eating snack",
			prop = "twerks",
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'It is not much, but the satisfying crunch is more than enough',
		}
	},
	--#endregion

	--#region CHICKEN SANDWICHES
  ['chicken_sandwich'] = {
		label = 'Chicken Sandwich',
		weight = 220,
		close = true,
		description = 'A hot, juicy chicken sandwich',
		client = {
			status = { hunger = 15, stress = -10 },
			anim = 'eating burger',
			prop = 'burger',
			usetime = 3000,
		},
		-- server = {
		-- 	export = 'ox_inventory_examples.testburger',
		-- 	test = 'what an amazingly delicious burger, amirite?'
		-- },
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					-- print('You licked the burger')
					exports['okokNotify']:Alert('Hamburg', 'You licked it... how about you just eat it weirdo', 4000, 'info', false)
				end
			},
			{
				label = 'Squeeze it',
				action = function(slot)
					-- print('You squeezed the burger :(')
					exports['okokNotify']:Alert('Hamburg', 'You feel the tender, warm buns between your fingers as you squeeze', 4000, 'info', false)
				end
			},
			{
				label = 'What do you call a vegan burger?',
				group = 'Hamburger Puns',
				action = function(slot)
					-- print('A misteak.')
					exports['okokNotify']:Alert('Hamburg', 'A misteak.', 4000, 'info', false)
				end
			},
			{
				label = 'What do frogs like to eat with their hamburgers?',
				group = 'Hamburger Puns',
				action = function(slot)
					-- print('French flies.')
					exports['okokNotify']:Alert('Hamburg', 'French flies.', 4000, 'info', false)
				end
			},
			{
				label = 'Why were the burger and fries running?',
				group = 'Hamburger Puns',
				action = function(slot)
					-- print('Because they\'re fast food.')
					exports['okokNotify']:Alert('Hamburg', 'Because they\'re fast food.', 4000, 'info', false)
				end
			}
		},
		consume = 0.3
	},
	--#endregion

	--#region SANDWICHES
  ["tosti"] = {
		label = "Tosti Sandwich",
		weight = 150,
		stack = true,
		close = true,
		description = "A fantastic looking grilled cheese sandwich",
		client = {
			status = { hunger = 10 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'You just ate the most delicious tosti this side of the Mississippi'
		}
	},
	["sandwich"] = {
		label = "Sandwich",
		weight = 200,
		stack = true,
		close = true,
		description = "A classic sandwich!",
		client = {
			status = { hunger = 10 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Your hunger is slightly satisfied by the delicious sandwich.'
		}
	},
	["bacon_grilled_cheese"] = {
		label = "Grilled Cheese with Bacon",
		weight = 180,
		stack = true,
		close = true,
		description = "The only thing that could make this better is guacamole.",
		client = {
			status = { hunger = 15, stress = -5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'The bacon with the melted cheese are enough to revive the dead.'
		},
	},
	--#endregion

	--#region DONUTS
	["donut_choc_sprinkles"] = {
		label = "Chocolate Donut with Sprinkles",
		weight = 40,
		stack = true,
		close = true,
		description = "Chocolate glaze on a fried donut with sprinkles.",
		client = {
			status = { hunger = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["donut_pink"] = {
		label = "Donut with Pink Icing and Sprinkles",
		weight = 40,
		stack = true,
		close = true,
		description = "Pink glaze on a fried donut with sprinkles.",
		client = {
			status = { hunger = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["donut_blue"] = {
		label = "Blue Icing Donut with Sprinkles",
		weight = 40,
		stack = true,
		close = true,
		description = "Blue icing on a fried donut with sprinkles.",
		client = {
			status = { hunger = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["donut_choc_filled"] = {
		label = "Cream Filled Chocolate Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A delicious cream filled donut with chocolate icing.",
		client = {
			status = { hunger = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["donut_choc_glaze"] = {
		label = "Chocolate Glazed Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "Milk chocolate icing with white chocolate drizzle on a fried donut.",
		client = {
			status = { hunger = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["donut_double_choc"] = {
		label = "Chocolate Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A delicious chocolate donut.",
		client = {
			status = { hunger = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["donut_light_pink"] = {
		label = "Creamy Strawberry Donut with Sprinkles",
		weight = 40,
		stack = true,
		close = true,
		description = "Creamy strawberry glaze on a fried donut with sprinkles.",
		client = {
			status = { hunger = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["donut_plain"] = {
		label = "Plain Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A classic, fried donut without the frill.",
		client = {
			status = { hunger = 15 },
			anim = 'eating burger',
			prop = 'donut',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["donut_twist"] = {
		label = "Twisted Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A classic donut with a twist!",
		client = {
			status = { hunger = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	--#endregion

	--#region DONUTS WITH PROPS
	["brum_donut_banana"] = {
		label = "Banana Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A banana donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_banana',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_blue"] = {
		label = "Blue Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A blue donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_blue',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_caramel"] = {
		label = "Caramel Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A caramel donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_caramel',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_chip"] = {
		label = "Choco Chip Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A chocolate chip donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_chip',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},

	["brum_donut_darkblue"] = {
		label = "Dark Blue Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A dark blue donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_darkblue',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_drizzle_blue"] = {
		label = "Blue Drizzle Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A blue drizzle donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_drizzle_blue',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_drizzle_darkblue"] = {
		label = "Dark Blue Drizzle Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A dark blue drizzle donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_drizzle_darkblue',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_drizzle_green"] = {
		label = "Green Drizzle Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A green drizzle donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_drizzle_green',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},

	["brum_donut_drizzle_mint"] = {
		label = "Mint Drizzle Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A mint drizzle donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_drizzle_mint',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_drizzle_pink"] = {
		label = "Pink Drizzle Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A pink drizzle donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_drizzle_pink',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_drizzle_purple"] = {
		label = "Purple Drizzle Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A purple drizzle donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_drizzle_purple',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_drizzle_red"] = {
		label = "Red Drizzle Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A red drizzle donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_drizzle_red',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_drizzle_yellow"] = {
		label = "Yellow Drizzle Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A yellow drizzle donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_drizzle_yellow',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},

	["brum_donut_fudge_ring"] = {
		label = "Fudge Ring Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A fudge ring donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_fudge_ring',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_green"] = {
		label = "Green Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A green donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_green',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_mint"] = {
		label = "Mint Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A yellow drizzle donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_mint',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_oreo"] = {
		label = "Oreo Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "An oreo donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_oreo',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},

	["brum_donut_pecan"] = {
		label = "Pecan Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A pecan donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_pecan',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_pink"] = {
		label = "Pink Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A pink donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_pink',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_purple"] = {
		label = "Purple Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A purple donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_purple',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_red"] = {
		label = "Red Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A red donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_red',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_strawberrycream"] = {
		label = "Strawberry Cream Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A strawberry cream donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_strawberrycream',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donut_tiramisu"] = {
		label = "Tiramisu Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A tiramisu donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_tiramisu',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},

	["brum_donut_yellow"] = {
		label = "Yellow Donut",
		weight = 40,
		stack = true,
		close = true,
		description = "A yellow donut you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating burger',
			prop = 'donut_yellow',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},

	["brum_donuthole"] = {
		label = "Donut Hole",
		weight = 40,
		stack = true,
		close = true,
		description = "A donut hole you donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 5 },
			anim = 'eating snack',
			prop = 'donuthole',
			disable = { combat = false, sprint = false },
			usetime = 300,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	["brum_donuthole_cup"] = {
		label = "Cup of Donut Holes",
		weight = 40,
		stack = true,
		close = true,
		description = "A wonderful cup of donut holes you... whole donut!",
		buttons = {
			{
				label = 'Lick it',
				action = function(slot)
					exports['okokNotify']:Alert('Dough Nut', 'You lick the donut like a fiend.', 4000, 'info', false)
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
			status = { hunger = 25 },
			anim = 'eating snack',
			prop = 'donuthole_cup',
			disable = { combat = true, sprint = false },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Donuts make the hunger go away.'
		},
	},
	--#endregion

	--region DESSERTS
	["tiramisu"] = {
		label = "Tiramisu",
		weight = 70,
		stack = true,
		close = true,
		description = "A classic Italian dessert made with layers of coffee-soaked ladyfingers, creamy mascarpone cheese filling, and a dusting of cocoa powder.",
		client = {
			status = { hunger = 10 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'The complexity satisfies the soul.'
		},
	},
	["cannoli"] = {
		label = "Cannoli",
		weight = 100,
		stack = true,
		close = true,
		description = "A traditional Italian pastry consisting of a crispy, fried tube-shaped shell filled with a sweet, creamy ricotta cheese mixture, often flavored with vanilla, citrus, or chocolate.",
		client = {
			status = { hunger = 10 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Nothing like a fresh filled cannoli.'
		},
	},
	--#endregion

	--#region BAKED GOODS
	["cherry_crown_pastry"] = {
		label = "Cherry Crown Pastry",
		weight = 80,
		stack = true,
		close = true,
		description = "A round pastry stuffed with fresh cherry filling!",
		client = {
			status = { hunger = 10 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'You lick the sticky cherry filling off your fingers.'
		},
	},
	["almond_croissant"] = {
		label = "Almond Croissant",
		weight = 80,
		stack = true,
		close = true,
		description = "Layer upon beautiful layer of flaky pastry and almond.",
		client = {
			status = { hunger = 10 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'The complexity satisfies the soul.'
		},
	},
	["butter_croissant"] = {
		label = "Butter Croissant",
		weight = 70,
		stack = true,
		close = true,
		description = "Layer upon beautiful layer of flaky, buttery pastry.",
		client = {
			status = { hunger = 10 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'The complexity satisfies the soul.'
		},
	},
	["muffin"] = {
		label = "Blueberry Muffin",
		weight = 110,
		stack = true,
		close = true,
		description = "A delicious, dense blueberry muffin!",
		client = {
			status = { hunger = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Simple, yet satisfying.'
		},
	},
	["chocolate_muffin"] = {
		label = "Chocolate Muffin",
		weight = 130,
		stack = true,
		close = true,
		description = "A delicious, dense chocolate muffin!",
		client = {
			status = { hunger = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Simple, yet satisfying.'
		},
	},
	["sausageroll"] = {
		label = "Breakfast Sausage Roll",
		weight = 180,
		stack = true,
		close = true,
		description = "Hot sausage inside a steamy pastry.",
		client = {
			status = { hunger = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Nothing like filling the gut with sausage.'
		},
	},
	--#endregion

	--#region ICE CREAM
	["cone_blueberry"] = {
		label = "Bubblegum Ice Cream",
		weight = 70,
		stack = true,
		close = true,
		description = "Bubble YUM YUM lollipop gum!",
		client = {
			status = { hunger = 10, thirst = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Delicious bubblegum ice cream slo..... FUCKING BRAIN FREEZE!'
		},
	},
	["cone_chocolate"] = {
		label = "Chocolate Ice Cream",
		weight = 70,
		stack = true,
		close = true,
		description = "Decadent chocolate ice cream.",
		client = {
			status = { hunger = 10, thirst = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Delicious chocolate ice cream slo..... FUCKING BRAIN FREEZE!'
		},
	},
	["cone_pistachio"] = {
		label = "Pistachio Ice Cream",
		weight = 70,
		stack = true,
		close = true,
		description = "Decadent pistachio ice cream.",
		client = {
			status = { hunger = 10, thirst = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Delicious pistachio ice cream slo..... FUCKING BRAIN FREEZE!'
		},
	},
	["cone_strawberry"] = {
		label = "Strawberry Ice Cream",
		weight = 70,
		stack = true,
		close = true,
		description = "Decadent strawberry ice cream.",
		client = {
			status = { hunger = 10, thirst = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Delicious strawberry ice cream slo..... FUCKING BRAIN FREEZE!'
		},
	},
	["cone_vanilla"] = {
		label = "Vanilla Ice Cream",
		weight = 70,
		stack = true,
		close = true,
		description = "Decadent vanilla ice cream.",
		client = {
			status = { hunger = 10, thirst = 15 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Delicious vanilla ice cream slo..... FUCKING BRAIN FREEZE!'
		},
	},
	--#endregion

	--#region HOTDOGS
	["hotdog_chili"] = {
		label = "Hotdog with Chili",
		weight = 120,
		stack = true,
		close = true,
		description = "A hotdog smothered in chili. I didn't ask what the meat was...",
		client = {
			status = { hunger = 10, stress = -5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Despite the mysterious meat, you crave another chili dog.'
		},
	},
	["hotdog_chilicheesedog"] = {
		label = "Hotdog with Chili and Cheese",
		weight = 135,
		stack = true,
		close = true,
		description = "A hotdog smothered in chili and topped with cheese. I didn't ask what the meat was...",
		client = {
			status = { hunger = 10, stress = -5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Despite the mysterious meat, you crave another chili dog with cheese.'
		},
	},
	["hotdog_deluxe"] = {
		label = "Hotdog with Chili, Cheese, and Corn Chips",
		weight = 150,
		stack = true,
		close = true,
		description = "A hotdog with a slice of American cheese smothered in chili and topped with corn chips. Simply amazing.",
		client = {
			status = { hunger = 10, stress = -5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Despite the mysterious meat, you crave another chili dog with cheese.'
		},
	},
	["hotdog_ketchup"] = {
		label = "Hotdog with Ketchup",
		weight = 110,
		stack = true,
		close = true,
		description = "This server is recommended for adults.",
		client = {
			status = { hunger = 10, stress = -5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Like the child you must be, you enjoy the hotdog with ketchup.'
		},
	},
	["hotdog_mustard"] = {
		label = "Hotdog with Mustard",
		weight = 110,
		stack = true,
		close = true,
		description = "A simple, yet delicious combo.",
		client = {
			status = { hunger = 10, stress = -5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'It may be simple, but you are oddly satisfied by the hotdog with mustard.'
		},
	},
	["hotdog_plain"] = {
		label = "Plain Hotdog",
		weight = 100,
		stack = true,
		close = true,
		description = "This server is recommended for adults.",
		client = {
			status = { hunger = 10, stress = -5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Like the child you must be, you enjoy the plain hotdog.'
		},
	},
	["hotdog_taco"] = {
		label = "Taco Hotdog",
		weight = 180,
		stack = true,
		close = true,
		description = "If you close your eyes, you will still know it's a hotdog entering your mouth.",
		client = {
			status = { hunger = 10, stress = -5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'The flavorful combination of hotdog and taco melt together on your tongue.'
		},
	},
	["hotdog_veggie"] = {
		label = "Vegan Hotdog with Veggies",
		weight = 150,
		stack = true,
		close = true,
		description = "There are two types of people in this world. You are neither of them.",
		client = {
			status = { hunger = 10, stress = -5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'You hold back the urge to scream at the top of your lungs that you are vegan.'
		},
	},
	--#endregion

	--#region BURGERS
	["burger_loaded"] = {
		label = "Deluxe Cheeseburger",
		weight = 230,
		stack = true,
		close = true,
		description = "A burger with cheese, lettuce, tomato, special sauce, and topped with a seasame seed bun.",
		client = {
			status = { hunger = 10, stress = -5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'The loaded burger leaves you stuffed.'
		},
	},
	["burger_pickle"] = {
		label = "Cheeseburger with Pickles",
		weight = 240,
		stack = true,
		close = true,
		description = "There are definitely pickles on there.",
		client = {
			status = { hunger = 10, stress = -5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'You never knew you loved pickles this much until now.'
		},
	},
	["burger_vegan"] = {
		label = "Vegan Burger",
		weight = 200,
		stack = true,
		close = true,
		description = "It looks like a burger, but it does not smell like a burger.",
		client = {
			status = { hunger = 15, stress = -10 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'You hold back the urge to scream at the top of your lungs that you are vegan.'
		},
	},
	["burger_plain"] = {
		label = "Burger with Ketchup",
		weight = 200,
		stack = true,
		close = true,
		description = "There are two types of people in this world. You are neither of them.",
		client = {
			status = { hunger = 10, stress = -5 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Simple, yet satisfying.'
		},
	},
	--#endregion

	--#region HORNYS ITEMS
	["hornburger"] = {
		label = "Horny's Single Burger",
		weight = 200,
		stack = true,
		close = true,
		description = "A classic from Horny's! A delicious, single patty, juicy burger",
		client = {
			status = { hunger = 10, stress = -10 },
			anim = 'eating burger',
			prop = 'burger',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Simple, yet satisfying.'
		},
	},
	["hornburger_dbl"] = {
		label = "Horny's Double Burger",
		weight = 300,
		stack = true,
		close = true,
		description = "The classic, turned up a notch. Two charbroiled patties surrounded by perfection.",
		client = {
			status = { hunger = 15, stress = -10 },
			anim = 'eating burger',
			prop = 'burger',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'You are curious how much better one more patty might be...'
		},
	},
	["hornburger_triple"] = {
		label = "Horny's Triple Burger",
		weight = 500,
		stack = true,
		close = true,
		description = "Three charbroiled patties each with their own slice of American cheese!",
		client = {
			status = { hunger = 99, stress = -10 },
			anim = 'eating burger',
			prop = 'burger',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Damn big back! Slow down.'
		},
	},
	["horn_chickensandwich"] = {
		label = "Horny's Chicken Sandwich",
		weight = 500,
		stack = true,
		close = true,
		description = "A golden, deep-fried chicken breast with lettuce, tomato, and that classic Horny's sauce!",
		client = {
			status = { hunger = 99, stress = -10 },
			anim = 'eating burger',
			prop = 'burger',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Tastes like chicken!'
		},
	},
	["hornsandwich"] = {
		label = "Horny's Classic Sandwich",
		weight = 200,
		stack = true,
		close = true,
		description = "Turkey, ham, lettuce, tomato, and Horny's secret sauce!",
		client = {
			status = { hunger = 10, stress = -10 },
			anim = 'eating burger',
			prop = 'tosti',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'You never question the secret sauce because this is the best sandwich you have ever had.'
		},
	},
	["hornburger_baconcheesemelt"] = {
		label = "Horny's Bacon Cheese Melt",
		weight = 250,
		stack = true,
		close = true,
		description = "The classic with a cheesy bacon twist!",
		client = {
			status = { hunger = 10, stress = -10 },
			anim = 'eating burger',
			prop = 'burger',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'The combo of melted cheese on top of perfectly crisped bacon leaves you craving more.'
		},
	},
	["hornfries_small"] = {
		label = "Horny's Salty French Fries",
		weight = 100,
		stack = true,
		close = true,
		description = "Slightly over-salted french fries.",
		client = {
			status = { hunger = 10, stress = -10 },
			anim = 'eating burger',
			prop = 'burger',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'When you wipe your hands, you notice there is no salt on your finger tips...'
		},
	},
	["horncone_vanilla"] = {
		label = "Horny's Classic Vanilla Cone",
		weight = 100,
		stack = true,
		close = true,
		description = "A perfectly normal vanilla ice cream cone.",
		client = {
			status = { hunger = 10, stress = -10 },
			anim = 'eating burger',
			prop = 'burger',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Nothing more refreshing than an ice cream cone on a hot day!'
		},
	},
	["horncone_chocolate"] = {
		label = "Horny's Classic Chocolate Cone",
		weight = 100,
		stack = true,
		close = true,
		description = "A perfectly normal chocolate ice cream cone.",
		client = {
			status = { hunger = 10, stress = -10 },
			anim = 'eating burger',
			prop = 'burger',
			disable = { combat = true, sprint = true },
			usetime = 2500,
			cancel = true,
			notifTitle = 'Nom nom',
			notification = 'Nothing more refreshing than an ice cream cone on a hot day!'
		},
	},
	--#endregion

	--#region BAGS/BOXES
	['paperbag'] = {
		label = 'Paper Bag',
		weight = 100,
		stack = false,
		close = false,
		consume = 0,
		description = 'A small bag used to hold items.',
		buttons = {{ label = 'Place', action = function(slot) exports['kq_placeable_items']:placeItem(slot) end }},
	},
	["bag_burger"] = {
    label = "Burger Bag",
    weight = 100,
    stack = false,
    close = false,
		consume = 0,
    description = "A large paper bag for holding burgers.",
	},
	["donutbox"] = {
    label = "Donut Box",
    weight = 100,
    stack = false,
    close = false,
		consume = 0,
    description = "A large box for holding donuts.",
		buttons = {{ label = 'Place', action = function(slot) exports['kq_placeable_items']:placeItem(slot) end }},
	},
	["pizzabox"] = {
    label = "Pizza Box",
    weight = 100,
    stack = false,
    close = false,
		consume = 0,
    description = "A large box for holding pizza.",
	},
		["pizzabox2"] = {
    label = "Pizza Box",
    weight = 100,
    stack = false,
    close = false,
		consume = 0,
    description = "A large box for holding pizza.",
	},
	--#endregion
}
```
