# AI Guards
These are criminal guards, so they will only protect specific gangs.  
This example uses the lostmc as the gang. Needs testing, but I believe the guards will attack people not part of the gang when they are in the zone.  

# Tweak the stationary and footPatrol guards as needed.  
```lua
['lostmc'] = {                -- NEEDED: CHANGE ME! Change to gangs code. If unknown, just the name of the gang is fine
    name = "lostmc",          -- NEEDED: CHANGE ME! Same as above
    zone = {
        enabled = true,
        position = vector3(-1556.98, 122.26, 56.86),    -- NEEDED: CHANGE ME! Center of the zone
        radius = 10,
    },
    guards = {
        stationary = {
            {
                position = vector4(-1541.33, 128.97, 56.78, 134.55),
                model = "s_m_m_armoured_01", 
                weapon = "weapon_carbinerifle",
                weapon_hidden = true, -- if true the weapon wont be shown when spawned
                ammo = 100,
            },
            {
                position = vector4(-1569.45, 116.76, 59.18, 47.17),
                model = "s_m_m_armoured_01",
                weapon = "WEAPON_ASSAULTRIFLE",
                weapon_hidden = true, -- if true the weapon wont be shown when spawned
                ammo = 150,
            },
            {
                position = vector4(-1579.47, 150.38, 58.7, 205.36),
                model = "s_m_m_armoured_01",
                weapon = "WEAPON_ASSAULTRIFLE",
                weapon_hidden = false, -- if true the weapon wont be shown when spawned
                ammo = 150,
            },
            {
                position = vector4(-1536.68, 156.82, 60.61, 0.12),
                model = "s_m_m_armoured_01",
                weapon = "WEAPON_SNIPERRIFLE",
                weapon_hidden = false, -- if true the weapon wont be shown when spawned
                ammo = 150,
            },
            -- add more guards if needed
        },

        footPatrol = {
            {
                  route = {
                        vector4(-1568.7, 116.42, 59.18, 132.41),
                        vector4(-1597.41, 85.62, 60.81, 145.28),
                        vector4(-1596.71, 72.4, 60.81, 204.78),
                        vector4(-1579.46, 70.89, 60.81, 313.3),
                        vector4(-1551.92, 99.99, 59.18, 316.77)
                      },
                      model = "a_f_m_salton_01",
                      weapon = "WEAPON_CARBINERIFLE",
                      weapon_hidden = false, -- if true the weapon wont be shown
                      ammo = 200,
                      behavior = "walking" -- walking or running
              },
              {
                route = {
                    vector4(-1514.19, 153.83, 55.65, 321.37),
                    vector4(-1501.81, 154.06, 55.65, 243.48),
                    vector4(-1497.16, 140.71, 55.65, 230.55),
                    vector4(-1474.58, 137.24, 55.65, 269.43),
                    vector4(-1472.76, 118.41, 55.65, 184.57)
                    },
                    model = "s_m_y_swat_01",
                    weapon = "WEAPON_CARBINERIFLE",
                    weapon_hidden = false, -- if true the weapon wont be shown
                    ammo = 200,
                    behavior = "walking" -- 'walking' or 'running'
            },
            -- add more guards if needed
        },
        -- completely ignore carPatrol. Too bugged out
        carPatrol = {
        }
    }
}
```
