# Alcatraz Templates

Welcome! Thank you for helping improve the server. It means a lot to me, and we
all benefit! If you think of any improvements for this guide please feel free to
post them in the discord or DM me directly. - Lester Morgan

### Browse through the links to find the template you are looking for

- [Boss Menu](./boss-menu/README.md#boss-menu)
- [Car Dealerships](./car-dealer/README.md#car-dealership-template)
- [Cars](./car-dealer/cars/README.md#custom-cars)
- [Crafting](./crafting/README.md#crafting)
- [Garages](./garages/README.md#garages)
- [Guards](./guards/README.md#ai-guards)
- [Hospitals](./hospitals/README.md#hospital-setup)
- [Items](./items/ITEMS.md)
- [Mechanic shops](./mechanic/README.md#mechanic-shop-template)
- [Placeable/Throwable Items](./place-throw-items/README.md#placeable-and-throwable-items)
- [Police Stations](./police/README.md#police--evidence)
- [Penal System](./police/penal-code/codes.md#alcatraz-penal-system)
- [Restaurant Recipes](./restaurants/restaurants.md/#item-categories)

## Instructions

Each file will have its own simple instructions, but they all will follow a
similar template.  
Below will be an example of a BLOCK of code. This example comes directly from
[this template](./hospitals/README.md#granny-hospital-template) in
[hospitals](./hospitals/README.md)  
Tip: You can just click the button in the upper right of the code block to copy.
Super easy!

```lua
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
        { coords = vec3(317.67, -585.37, 42.84 + 0.3), heading = 160.0 },      -- OPTIONAL: Only needed if DisableHospitalBeds = false
    }
},
```

COPY and PASTE the entire BLOCK of code into any text editor of your choosing
such as:

- notepad
- <a href="https://docs.google.com" target="_blank" rel="noopener noreferrer">Google
  Docs</a>
- etc.

Look through and read all lines that say NEEDED or OPTIONAL, and change as
necessary  
When you paste your coordinates, you may notice it says vector3(...) instead of
vec3(...) - That is okay, they are the exact same thing to the computer  
Same thing goes for vector4(...) and vec4(...)

### Tips

As you go through, it may be helpful to delete: -- NEEDED: CHANGE ME! Heading of
ped  
or any of those lines, just so you know you already did that. Here is an example
of the above, but completed:

```lua
GrannySmith = {
    Ped = 'a_f_m_fatcult_01',
    Coords = vector3(-1104.65, 4937.15, 222.71),
    Distance = 4.85,
    Heading = 36.38,
    Cost = 5,
    Duration = 15 * seconds,
    PayAccount = 'cash',
    Label = '[E] - Check In',
    HotKey = 38,
    Target = {
        enabled = false,
    },
    DisableHospitalBeds = true,
    RespawnNoBedLocation = { coords = vector3(-1112.74, 4940.66, 222.71), heading = 157.79 },
    HospitalBeds = {
        { coords = vec3(317.67, -585.37, 42.84 + 0.3), heading = 160.0 },
    }
},
```

### Complete

Once the entire BLOCK is updated, paste the complete version into the
corresponding discord channel, and I will add to the server. Simple as that!

# Future Updates

### Templates to add:

- Dispatch radio codes
- Outfits (work)
