# Police & Evidence
Police and Evidence are set up separately  
They both use the same job at the moment. There is always room for an evidence department  
- [Police Station Setup](#police-station-setup)  
- [Evidence Setup](#evidence-setup)

### Police Station Setup
Here is the configuration on how to set up an entire police department.  
Just past this will be the Evidence configuration.  
```lua
LSPD = {
    blip = {
        enabled = true,
        coords = vec3(464.57, -992.0, 30.69),
        sprite = 60,
        color = 29,
        scale = 1.0,
        string = 'Mission Row PD'
    },

    clockInAndOut = {
        enabled = true,                        
        jobLock = 'police',                    -- OPTIONAL: change to different job. Police will be the only one until room for new depts.
        coords = vec3(464.87, -977.37, 30.69), 
        label = '[E] - Go On/Off Duty',        
        distance = 3.0,                        
        target = {
            enabled = false,
        }
    },

    armoury = {
        enabled = true,
        coords = vec3(480.32, -996.67, 30.69 - 0.9),                             -- Coords where NPC stands
        heading = 86.95,                                                         -- Heading of armoury NPC (direction they face)
        ped = 's_f_y_cop_01',                                                    -- Ped model or false for no ped
        label = '[E] - Access Armoury',
        target = {
            enabled = false,
        },
        jobLock = 'police',                                        -- OPTIONAL: change to different job. Police will be the only one until room for new depts.
        weapons = {
            [0] = {                                                                                  -- Grade number will be the name of each table(this would be grade 0)
                { name = 'WEAPON_PISTOL',     label = 'Pistol',      multiple = false, price = false },    -- Set price to false if undesired
                { name = 'WEAPON_NIGHTSTICK', label = 'Night Stick', multiple = false, price = false },
                { name = 'ammo-9' , label = '9mm Ammo', multiple = true, price = 10 },
                { name = 'armour', label = 'Bulletproof Vest', multiple = false, price = 100 },

            },
            [1] = { -- This would be grade 1
                { name = 'WEAPON_COMBATPISTOL', label = 'Combat Pistol', multiple = false, price = 150 },
                { name = 'WEAPON_NIGHTSTICK',   label = 'Night Stick',   multiple = false, price = 50 },
                { name = 'ammo-9', label = '9mm Ammo', multiple = true, price = 10 },
                { name = 'armour', label = 'Bulletproof Vest', multiple = false, price = 100 },
            },
            [2] = { -- This would be grade 2
                { name = 'WEAPON_COMBATPISTOL', label = 'Combat Pistol', multiple = false, price = 150 },
                { name = 'WEAPON_NIGHTSTICK',   label = 'Night Stick',   multiple = false, price = 50 },
                { name = 'WEAPON_ASSAULTRIFLE', label = 'Assault Rifle', multiple = false, price = 1100 },
            },
            [3] = { -- This would be grade 3
                { name = 'WEAPON_COMBATPISTOL', label = 'Combat Pistol', multiple = false, price = 150 },
                { name = 'WEAPON_NIGHTSTICK',   label = 'Night Stick',   multiple = false, price = 50 },
                { name = 'WEAPON_ASSAULTRIFLE', label = 'Assault Rifle', multiple = false, price = 1100 },
            },
        }
    },

    cloakroom = {
        enabled = true,
        jobLock = 'police',                    -- OPTIONAL: change to different job. Police will be the only one until room for new depts.
        coords = vec3(462.36, -999.62, 30.69), -- NEEDED: CHANGE ME! Coords of cloakroom
        label = '[E] - Change Clothes',
        range = 2.0,
        uniforms = {                           -- Uniform choices
            [1] = {                            -- Order it will display
                label = 'Patrol',              -- Name of outfit that will display in menu
                minGrade = 0,                  -- Min grade level that can access? Set to 0 or false for everyone to use
                male = {                       -- Male variation
                    clothing = {
                        -- Components / 0: Face 1: Mask 2: Hair 3: Torso 4: Leg 5: Parachute / bag 6: Shoes 7: Accessory 8: Undershirt 9: Kevlar 10: Badge 11: Torso 2
                        -- https://docs.fivem.net/natives/?_0xD4F7B05C
                        { component = 11, drawable = 5,  texture = 2 }, -- Torso
                        { component = 8,  drawable = 15, texture = 0 }, -- Shirt
                        { component = 4,  drawable = 6,  texture = 1 }, -- Pants
                        { component = 6,  drawable = 16, texture = 7 }, -- Shoes
                        { component = 3,  drawable = 5,  texture = 0 }, -- Arms
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
                        { component = 11, drawable = 4,  texture = 0 }, -- Torso
                        { component = 8,  drawable = 15, texture = 0 }, -- Shirt
                        { component = 4,  drawable = 25, texture = 0 }, -- Pants
                        { component = 6,  drawable = 16, texture = 4 }, -- Shoes
                        { component = 3,  drawable = 4,  texture = 0 }, -- Arms
                    },
                    props = {
                        -- Components / 0: Hats 1: Glasses 2: Ears 6: Watches 7: Bracelets
                        -- https://docs.fivem.net/natives/?_0x93376B65A266EB5F

                        --    { component = 0, drawable = 0, texture = 0 }, -- Hats
                    }
                }
            },
            [2] = {              -- Order it will display
                label = 'Chief', -- Name of outfit that will display in menu
                minGrade = 0,    -- Min grade level that can access? Set to 0 or false for everyone to use
                male = {         -- Male variation
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
                        { component = 11, drawable = 4,  texture = 0 }, -- Torso
                        { component = 8,  drawable = 15, texture = 0 }, -- Shirt
                        { component = 4,  drawable = 25, texture = 0 }, -- Pants
                        { component = 6,  drawable = 16, texture = 4 }, -- Shoes
                        { component = 3,  drawable = 4,  texture = 0 }, -- Arms
                    },
                    props = {
                        -- Components / 0: Hats 1: Glasses 2: Ears 6: Watches 7: Bracelets
                        -- https://docs.fivem.net/natives/?_0x93376B65A266EB5F

                        --    { component = 0, drawable = 0, texture = 0 }, -- Hats
                    }
                }
            },
            [3] = {              -- Order it will display
                label = 'Chief 2', -- Name of outfit that will display in menu
                minGrade = 0,    -- Min grade level that can access? Set to 0 or false for everyone to use
                male = {         -- Male variation
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
                        { component = 11, drawable = 4,  texture = 0 }, -- Torso
                        { component = 8,  drawable = 15, texture = 0 }, -- Shirt
                        { component = 4,  drawable = 25, texture = 0 }, -- Pants
                        { component = 6,  drawable = 16, texture = 4 }, -- Shoes
                        { component = 3,  drawable = 4,  texture = 0 }, -- Arms
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
    
    personalLocker = {
        enabled = true,
        jobLock = 'police',                    -- OPTIONAL: change to different job. Police will be the only one until room for new depts.
        coords = vec3(462.64, -995.88, 30.69), -- NEEDED: CHANGE ME! Location of personal locker
        range = 2.0, 
        label = '[E] - Access Personal Locker',
        target = {
            enabled = false,
        }
    },

    vehicles = {
        enabled = true,                            -- Enable? False if you have you're own way for medics to obtain vehicles.
        jobLock = 'police',                        -- OPTIONAL: change to different job. Police will be the only one until room for new depts.
        zone = {
            coords = vector3(456.78, -987.68, 25.7),   -- NEEDED: CHANGE ME! Where employees will go to spawn their police car
            range = 5.5, 
            label = '[E] - Access Garage',
            return_label = '[E] - Return Vehicle'
        },
        spawn = {
            land = {
                coords = vec3(449.37, -1025.46, 28.59),     -- NEEDED: CHANGE ME!  Coords of where land vehicle spawn/return
                heading = 3.68                              -- NEEDED: CHANGE ME!  Direction vehicle faces when spawning
            },
            air = {
                coords = vec3(449.29, -981.76, 43.69),    -- NEEDED: CHANGE ME!  Coords of where air vehicles spawn/return
                heading = 0.01                            -- NEEDED: CHANGE ME!  Direction vehicle faces when spawning
            }
        },
        options = {
            [0] = {                    -- Job grade as table name
                ['police'] = {         -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Police Cruiser',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['police2'] = {        -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Police Cruiser #2',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['polmav'] = {         -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Maverick',
                    category = 'air',  -- Options are 'land' and 'air'
                },
            },

            [1] = {                    -- Job grade as table name
                ['police'] = {         -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Police Cruiser',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['police2'] = {        -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Police Cruiser #2',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['polmav'] = {         -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Maverick',
                    category = 'air',  -- Options are 'land' and 'air'
                },
            },

            [2] = {                    -- Job grade as table name
                ['police'] = {         -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Police Cruiser',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['police2'] = {        -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Police Cruiser #2',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['polmav'] = {         -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Maverick',
                    category = 'air',  -- Options are 'land' and 'air'
                },
            },

            [3] = {                    -- Job grade as table name
                ['police'] = {         -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Police Cruiser',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['police2'] = {        -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Police Cruiser #2',
                    category = 'land', -- Options are 'land' and 'air'
                },
                ['polmav'] = {         -- Car/Helicopter/Vehicle Spawn Code/Model Name
                    label = 'Maverick',
                    category = 'air',  -- Options are 'land' and 'air'
                },
            },
        }
    },
    -- outsourced to wasabi_evidence
    evidenceLocker = {
        enabled = false
    },

    -- outsourced to okokBossMenu
    bossMenu = {
        enabled = false
        -- PASTE BELOW JUST THE vector3 OF WHERE YOU WANT YOUR BOSS MENU
        -- replace example below with your own boss menu coordinates
        vector3(461.54, -986.17, 30.66)     -- NEEDED: CHANGE ME! Replace me with boss menu coords
    }
    
},
```

### Evidence Setup
- [Back to Top](#police--evidence)
Here is the configuration on how to set up an the evidence section of any police department  
```lua
LSPD = {
    label = 'LSPD',                                         -- NEEDED: CHANGE ME! Display label

    analyze = {
        coords = vec3(483.63, -987.9, 30.68),               -- NEEDED: CHANGE ME! Coords for location(If target is not enabled)
        range = 1.8,
        label = '[E] - Analyze Evidence',
        target = {
            enabled = false,
        }
    },

    fingerprinting = {
        enabled = true,
        coords = vec3(473.24, -1007.58, 26.26),             -- NEEDED: CHANGE ME! Coords for fingerprinting
        range = 1.8,
        label = '[E] - Take Suspect\'s Fingerprints',
        target = {
            enabled = false,
        }
    },

    storage = {
        enabled = true,
        coords = vec3(480.84, -984.55, 30.68),              -- NEEDED: CHANGE ME! Coords for evidence storage
        range = 1.8,
        label = '[E] - Access Evidence Storage',
        target = {
            enabled = false,
        }
    },
    ---------------------------------------------------------------------------------------------------------------------
    jobLock = false,        -- OPTIONAL: Put job here if want this specific crime lab locked to only one job
    -- leave as false if all Config.PoliceJobs can access)                                                             --
    -- Can be string (ex. 'police' or table ex. {'police', 'sheriff'})                                                 --
    ---------------------------------------------------------------------------------------------------------------------
},
```
