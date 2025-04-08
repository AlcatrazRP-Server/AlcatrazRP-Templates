# Hospital Setup
There are two templates here.
- Official Hospital
- "Granny" Hospital

### Official Hospital Template
Mostly have to change vector3 coordinates. Will create a fully functioning hospital ready for staff and patients  
Only NEED one setup in Paleto at the moment
<pre>
Pillbox = {
    RespawnPoint = {
        coords = vec3(317.8, -585.14, 44.2),        -- NEEDED: CHANGE ME! Can be same as Blip Coords below. When player dies, this point is used to see which hospital is closest
        heading = 332.22,
        useCheckInInstead = true
    },

    Blip = {
        Enabled = true,
        Coords = vec3(324.15, -583.14, 44.20),      -- NEEDED: CHANGE ME! Where blip will display
        Sprite = 61,
        Color = 2,
        Scale = 1.0,
        String = 'Pillbox Hospital'                 -- NEEDED: CHANGE ME! Name when blip is selected on the map
    },

    clockInAndOut = {
        enabled = true,
        coords = vec3(334.75, -580.24, 43.28),      -- NEEDED: CHANGE ME! Location of where to go on and off duty(If not using target)
        label = '[E] - Go On/Off Duty',
        distance = 3.0,
        target = {
            enabled = false,
        }
    },

    PersonalLocker = {
        enabled = true,
        jobLock = 'ambulance',
        coords = vec(298.61, -598.28, 43.28),        -- NEEDED: CHANGE ME! Location of where to access personal locker (If target is disabled)
        label = '[E] - Access Personal Locker',
        maxWeight = 5000,
        slots = 30,
        distance = 2.0,
        target = {
            enabled = false,
        }
    },

    CheckIn = {
        Enabled = true,
        Ped = 's_m_m_scientist_01',                  -- NEEDED: CHANGE ME! Check in ped
        Coords = vec3(308.58, -595.31, 43.28 - 0.9), -- NEEDED: CHANGE ME! Coords of ped
        Distance = 4.85,
        Heading = 63.26,                             -- NEEDED: CHANGE ME! Heading of ped
        Cost = 500,                                  -- NEEDED: CHANGE ME! Cost of using hospital check-in. Set to false for free
        Duration = 15 * seconds,
        MaxOnDuty = 3,                               -- If this amount or less you can use, otherwise it will tell you that EMS is avaliable(Set to false to always enable check-in)
        PayAccount = 'bank',
        PayHospital = true,
        Label = '[E] - Check In',
        HotKey = 38,
        Target = {
            enabled = false,
        },
        DisableHospitalBeds = false,
        RespawnNoBedLocation = { coords = vec3(316.66, -581.3, 43.28), heading = 339.02 }, -- NEEDED: CHANGE ME! Where to spawn when beds are full. Add new vector3 (same as vec3) and new heading
        HospitalBeds = {
            { coords = vec3(317.67, -585.37, 42.84 + 0.3), heading = 160.0 },              -- NEEDED: CHANGE ME! Change the vector3. Be sure to add + 0.3 to the last value like in the example. Change heading as well.
        }

    },

    Cloakroom = {
        Enabled = true,
        Coords = vec3(300.6, -597.7, 42.1), -- NEEDED: CHANGE ME! Coords of cloakroom
        Label = '[E] - Change Clothes',
        HotKey = 38,
        Range = 1.5,
        Uniforms = { 
            [1] = {                         -- Order it will display
                label = 'Medic',            -- Name of outfit that will display in menu
                minGrade = 0,               -- Min grade level that can access? Set to 0 or false for everyone to use
                male = {                    -- Male variation
                    clothing = {
                        -- Components / 0: Face 1: Mask 2: Hair 3: Torso 4: Leg 5: Parachute / bag 6: Shoes 7: Accessory 8: Undershirt 9: Kevlar 10: Badge 11: Torso 2
                        -- https://docs.fivem.net/natives/?_0xD4F7B05C
                        { component = 11, drawable = 15, texture = 0 }, -- Torso
                        { component = 8,  drawable = 58, texture = 0 }, -- Shirt
                        { component = 4,  drawable = 35, texture = 0 }, -- Pants
                        { component = 6,  drawable = 24, texture = 0 }, -- Shoes
                        { component = 3,  drawable = 15, texture = 0 }, -- Arms
                    },
                    props = {
                        -- Components / 0: Hats 1: Glasses 2: Ears 6: Watches 7: Bracelets
                        -- https://docs.fivem.net/natives/?_0x93376B65A266EB5F

                        --    { component = 0, drawable = 0, texture = 0 }, -- Hats
                    }
                },
                female = {
                    clothing = {
                        -- Components / 0: Face 1: Mask 2: Hair 3: Torso 4: Leg 5: Parachute / bag 6: Shoes 7: Accessory 8: Undershirt 9: Kevlar 10: Badge 11: Torso 2
                        -- https://docs.fivem.net/natives/?_0xD4F7B05C
                        { component = 11, drawable = 15, texture = 0 }, -- Torso
                        { component = 8,  drawable = 58, texture = 0 }, -- Shirt
                        { component = 4,  drawable = 35, texture = 0 }, -- Pants
                        { component = 6,  drawable = 24, texture = 0 }, -- Shoes
                        { component = 3,  drawable = 15, texture = 0 }, -- Arms
                    },
                    props = {
                        -- Components / 0: Hats 1: Glasses 2: Ears 6: Watches 7: Bracelets
                        -- https://docs.fivem.net/natives/?_0x93376B65A266EB5F

                        --    { component = 0, drawable = 0, texture = 0 }, -- Hats
                    }
                }
            },
            [2] = {
                label = 'Doctor',
                minGrade = 1, -- Min grade level that can access? Set to 0 or false for everyone to use
                male = {
                    clothing = {
                        -- Components / 0: Face 1: Mask 2: Hair 3: Torso 4: Leg 5: Parachute / bag 6: Shoes 7: Accessory 8: Undershirt 9: Kevlar 10: Badge 11: Torso 2
                        -- https://docs.fivem.net/natives/?_0xD4F7B05C
                        { component = 11, drawable = 15, texture = 0 }, -- Torso
                        { component = 8,  drawable = 58, texture = 0 }, -- Shirt
                        { component = 4,  drawable = 35, texture = 0 }, -- Pants
                        { component = 6,  drawable = 24, texture = 0 }, -- Shoes
                        { component = 3,  drawable = 15, texture = 0 }, -- Arms
                    },
                    props = {
                        -- Components / 0: Hats 1: Glasses 2: Ears 6: Watches 7: Bracelets
                        -- https://docs.fivem.net/natives/?_0x93376B65A266EB5F

                        --    { component = 0, drawable = 0, texture = 0 }, -- Hats
                    }
                },
                female = {
                    clothing = {
                        -- Components / 0: Face 1: Mask 2: Hair 3: Torso 4: Leg 5: Parachute / bag 6: Shoes 7: Accessory 8: Undershirt 9: Kevlar 10: Badge 11: Torso 2
                        -- https://docs.fivem.net/natives/?_0xD4F7B05C
                        { component = 11, drawable = 15, texture = 0 }, -- Torso
                        { component = 8,  drawable = 58, texture = 0 }, -- Shirt
                        { component = 4,  drawable = 35, texture = 0 }, -- Pants
                        { component = 6,  drawable = 24, texture = 0 }, -- Shoes
                        { component = 3,  drawable = 15, texture = 0 }, -- Arms
                    },
                    props = {
                        -- Components / 0: Hats 1: Glasses 2: Ears 6: Watches 7: Bracelets
                        -- https://docs.fivem.net/natives/?_0x93376B65A266EB5F

                        --    { component = 0, drawable = 0, texture = 0 }, -- Hats
                    }
                }
            },
        }
    },

    MedicalSupplies = {
        Enabled = true,
        Ped = 's_m_m_doctor_01',                                            -- OPTIONAL: Ped model
        Coords = vec3(306.63, -601.44, 43.28 - 0.95),                       -- NEEDED: CHANGE ME! Coords of ped
        Heading = 337.64,                                                   -- NEEDED: CHANGE ME! Heading of ped
        Supplies = {
            { item = 'medbag',     label = 'Medical Bag',   price = false }, -- Pretty self explanatory, price may be set to 'false' to make free
            { item = 'medikit',    label = 'First-Aid Kit', price = 250 },
            { item = 'morphine30', label = 'Morphine 30MG', price = 100 },
            { item = 'morphine15', label = 'Morphine 15MG', price = 45 },
            { item = 'perc30',     label = 'Percocet 30MG', price = 60 },
            { item = 'perc10',     label = 'Percocet 10MG', price = 40 },
            { item = 'perc5',      label = 'Percocet 5MG',  price = 30 },
            { item = 'vic10',      label = 'Vicodin 10MG',  price = 30 },
            { item = 'vic5',       label = 'Vicodin 5MG',   price = 15 },
        }
    },

    Vehicles = {
        Enabled = true,
        Zone = {
            coords = vector3(334.2, -586.71, 28.8),       -- NEEDED: CHANGE ME! Area to prompt vehicle garage
            range = 5.5,
            label = '[E] - Access Garage',
            return_label = '[E] - Return Vehicle'
        },
        Spawn = {
            land = {
                coords = vec3(296.16, -607.67, 43.25),    -- NEEDED: CHANGE ME!
                heading = 68.43                           -- NEEDED: CHANGE ME!
            },
            air = {
                coords = vec3(351.24, -587.67, 74.55),    -- NEEDED: CHANGE ME!
                heading = 289.29                          -- NEEDED: CHANGE ME!
            }
        },
        Options = {
            [0] = {                    -- Job grade
                ['ambulance'] = {      -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Ambulance',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['dodgeems'] = {       -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Dodge Charger',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['polmav'] = {         -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Maverick',
                    category = 'air',  -- Options are 'land' and 'air'
                },
            },

            [1] = {
                ['ambulance'] = {      -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Ambulance',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['dodgeems'] = {       -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Dodge Charger',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['polmav'] = {         -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Maverick',
                    category = 'air',  -- Options are 'land' and 'air'
                },
            },

            [2] = {
                ['ambulance'] = {      -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Ambulance',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['dodgeems'] = {       -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Dodge Charger',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['polmav'] = {         -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Maverick',
                    category = 'air',  -- Options are 'land' and 'air'
                },
            }
        }
    },

    -- outsourced to okokBossMenu
    BossMenu = {
        Enabled = false,
        -- PASTE BELOW JUST THE vector3 OF WHERE YOU WANT YOUR BOSS MENU
        -- replace example below with your own boss menu coordinates
        vector3(461.54, -986.17, 30.66)     -- NEEDED: CHANGE ME! Replace me with boss menu coords
    },
},
</pre>

### Granny Hospital Template
This is the criminal/private hospital template.  
These hospitals will not display on the map.  
<pre>
GrannySmith = {
    Ped = 's_m_m_scientist_01',                   -- OPTIONAL: Check in ped
    Coords = vec3(1729.03, 2563.33, 45.56 - 0.9), -- NEEDED: CHANGE ME! Coords of ped
    Distance = 4.85,
    Heading = 181.42,                             -- NEEDED: CHANGE ME! Heading of ped
    Cost = 5,                                     -- NEEDED: CHANGE ME! Cost of using hospital check-in. Set to false for free
    Duration = 15 * seconds,                      -- OPTIONAL: Time it takes to spend in hospital bed
    PayAccount = 'bank',                          -- OPTIONAL: Account dead player pays from to check-in(bank or cash)
    Label = '[E] - Check In',
    HotKey = 38,
    Target = {
        enabled = false,
    },
    DisableHospitalBeds = true,           -- Disable hospital beds for check-in at this location?(Player will spend Duration checking in before respawning in RespawnNoBedLocation coords when set to true)
    RespawnNoBedLocation = { coords = vec3(1729.03, 2563.33, 45.56), heading = 339.02 }, -- NEEDED: CHANGE ME! Coords and heading of where to spawn player if DisableHospitalBeds is set to true or beds full
    HospitalBeds = {
        { coords = vec3(317.67, -585.37, 42.84 + 0.3), heading = 160.0 },      OPTIONAL: Only needed if DisableHospitalBeds = false
    }
},
</pre>
