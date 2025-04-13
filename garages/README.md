# Garages

- [Back to Main Page](../README.md#alcatraz-templates)

Below you will find different categories for each type of garage:

- [Public](#public-garages)
- [Employee Only](#employee-only)
- [Business Spawner](#business-spawner)

### Public Garages

Public garages for everybody to use.

```lua
["Legion Square"] = {                             -- NEEDED: CHANGE ME! Name that will show up on the map
  coords = vector3(215.09, -805.17, 30.81),       -- NEEDED: CHANGE ME! This is where users will activate the garage menu
  spawn = {
    vector4(216.84, -802.02, 30.78, 69.82),
    -- add more spawn locations by just pasting in more vector4 coords.
  },
  distance = 15,
  type = "car",
  hideBlip = false,               -- OPTIONAL: change to true to remove blip from map (make hidden, but still public)
  blip = {
    id = 357,
    color = 0,
    scale = 0.7
  },
  hideMarkers = true,
  markers = { id = 21, size = { x = 0.3, y = 0.3, z = 0.3 }, color = { r = 255, g = 255, b = 255, a = 120 }, bobUpAndDown = 0, faceCamera = 0, rotate = 1, drawOnEnts = 0 },
},
```

### Employee Only

These are player owned vehicles

```lua
["Mechanic"] = {                                      -- NEEDED: CHANGE ME! Just name business i.e. Burgershot, LSCustoms, etc.
  coords = vector3(157.86, -3005.9, 7.03),
  spawn = vector4(165.26, -3014.94, 5.9, 268.8),
  distance = 15,
  job = {"mechanic"},
  type = "car",
  hideBlip = false,
  blip = {
    id = 357,
    color = 0,
    scale = 0.7
  },
  hideMarkers = true,
  markers = { id = 21, size = { x = 0.3, y = 0.3, z = 0.3 }, color = { r = 255, g = 255, b = 255, a = 120 }, bobUpAndDown = 0, faceCamera = 0, rotate = 1, drawOnEnts = 0 },
  vehiclesType = "owned", -- Use owned vehicles that can anyone in this society can access - more details: https://docs.jgscripts.com/advanced-garages/job-and-gang-garages
},
```

### Business Spawner

This type of garage spawn vehicles. Mainly for emergency services such as police
and EMS  
Police and EMS have built in garages, so this would only be necessary for towing
or other jobs such as taxi, bus driver etc.  
Might use this for emergency services since the minJobGrade feature is nice and
uses less code

```lua
["Towing"] = {                                        -- NEEDED: CHANGE ME! Just name the service i.e. Police, EMS, Towing, etc.
  coords = vector3(434.48, -1016.97, 28.83),          -- NEEDED: CHANGE ME! This is where users will activate the garage menu
  spawn = vector4(434.55, -1014.54, 28.49, 91.56),    -- NEEDED: CHANGE ME! This is where vehicles will spawn
  distance = 15,
  job = {"towtruck"},
  type = "car",
  hideBlip = false,
  blip = {
    id = 357,
    color = 0,
    scale = 0.7
  },
  hideMarkers = true,
  markers = { id = 21, size = { x = 0.3, y = 0.3, z = 0.3 }, color = { r = 255, g = 255, b = 255, a = 120 }, bobUpAndDown = 0, faceCamera = 0, rotate = 1, drawOnEnts = 0 },
  vehiclesType = "spawner", -- Spawn a basic vehicle from a list
  showLiveriesExtrasMenu = true, -- Allow player to select a livery and extras before pulling vehicle out
  vehicles = {
    [1] = {
      model = "police",         -- spawn code for vehicle
      plate = false,            -- set as false for a random plate; do not use a plate already in use in the DB!
      minJobGrade = 0,          -- only available to players with set minimum grade
      nickname = "Police car",  -- Show a custom name instead of the vehicle's real name
      livery = 1,               -- only need to change four lines above
      extras = {1, 2},
      maxMods = true
    },
    [2] = {
      model = "police2",
      plate = false,
      minJobGrade = 3,
      nickname = "Police car 2",
      livery = 2,
      extras = {},
      maxMods = true
    }
  }
}
```

- [Back to Top](#garages)
- [Back to Main Page](../README.md#alcatraz-templates)
