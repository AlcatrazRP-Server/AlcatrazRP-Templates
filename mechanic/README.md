# Mechanic Shop template

## Data needed:
Go through and look for the lines that say: -- NEEDED: CHANGE ME!!  
Just get the vector3 coordinates, and paste them in to the appropriate spots  

That's all you need as a mechanic. Your tablet is your boss menu

<pre>
lscustoms = {
  type = "owned",
  job = "mechanic",
  jobManagementRanks = {4},
  logo = "ls_customs.png",
  commission = 0, -- %, 10 = 10%
  locations = {
    {
      coords = vector3(-337.25, -137.2, 38.35),     -- NEEDED: CHANGE ME!! This is where the customers will open the menu
      size = 6.5,
      showBlip = true,
    },
    { -- start paste here
      coords = vector3(-337.25, -137.2, 38.35),     -- OPTIONAL: Just copy everything from the starting { just above this line to the ending }
      size = 6.5,
      showBlip = false,
    } -- end paste here
  },
  blip = {
    id = 446,
    color = 47,
    scale = 0.7
  },
  mods = {
    repair           = { enabled = true, price = 500, percentVehVal = 0.01 },
    performance      = { enabled = true, price = 500, percentVehVal = 0.01, priceMult = 0.1 },
    cosmetics        = { enabled = true, price = 500, percentVehVal = 0.01, priceMult = 0.1 },
    stance           = { enabled = true, price = 500, percentVehVal = 0.01 },
    respray          = { enabled = true, price = 500, percentVehVal = 0.01 },
    wheels           = { enabled = true, price = 500, percentVehVal = 0.01, priceMult = 0.1 },
    neonLights       = { enabled = true, price = 500, percentVehVal = 0.01 },
    headlights       = { enabled = true, price = 500, percentVehVal = 0.01 },
    tyreSmoke        = { enabled = true, price = 500, percentVehVal = 0.01 },
    bulletproofTyres = { enabled = false, price = 500, percentVehVal = 0.01 },
    extras           = { enabled = true, price = 500, percentVehVal = 0.01 }
  },
  tuning = {
    engineSwaps      = { enabled = true, requiresItem = true },
    drivetrains      = { enabled = true, requiresItem = true },
    turbocharging    = { enabled = true, requiresItem = true },
    tyres            = { enabled = true, requiresItem = true },
    brakes           = { enabled = true, requiresItem = true },
    driftTuning      = { enabled = true, requiresItem = true },
    gearboxes        = { enabled = true, requiresItem = true },
  },
  carLifts = {
    -- vector4(-357.45, -114.17, 38.7, 339.89)
  },
  shops = {
    {
      name = "Servicing Supplies",
      coords = vector3(-345.54, -131.32, 39.01),    -- NEEDED: CHANGE ME!! This is where the mechanics will purchase their most used items
      size = 2.0,
      usePed = false,
      pedModel = "s_m_m_lathandy_01",
      marker = { id = 21, size = { x = 0.3, y = 0.3, z = 0.3 }, color = { r = 255, g = 255, b = 255, a = 120 }, bobUpAndDown = 0, faceCamera = 0, rotate = 1, drawOnEnts = 0 },
      items = {
        { name = "engine_oil", label = "Engine Oil", price = 50 },
        { name = "tyre_replacement", label = "Tyre Replacement", price = 2500 },
        { name = "clutch_replacement", label = "Clutch Replacement", price = 3000 },
        { name = "air_filter", label = "Air Filter", price = 300 },
        { name = "spark_plug", label = "Spark Plug", price = 100 },
        { name = "suspension_parts", label = "Suspension Parts", price = 2500 },
        { name = "brakepad_replacement", label = "Brakepad Replacement", price = 1500 },
      },
    },
    {
      name = "Advanced Upgrades",
      coords = vector3(-343.79, -139.92, 39.01),    -- NEEDED: CHANGE ME!! This is where the mechanics will purchase their more unique items
      size = 2.0,
      usePed = false,
      pedModel = "s_m_m_lathandy_01",
      marker = { id = 21, size = { x = 0.3, y = 0.3, z = 0.3 }, color = { r = 255, g = 255, b = 255, a = 120 }, bobUpAndDown = 0, faceCamera = 0, rotate = 1, drawOnEnts = 0 },
      items = {
        { name = "turbocharger", label = "Turbo Charger", price = 25000 },
        { name = "v8_engine", label = "V8 Engine Upgrade", price = 40000 },
        { name = "ceramic_brakes", label = "Ceramic Brakes", price = 15000 },
      },
    }
  },
  stashes = {
    {
      name = "Parts Bin",
      coords = vector3(-339.24, -132.2, 39.01),     -- NEEDED: CHANGE ME!! This is where the mechanics will stash their supplies
      size = 2.0,
      usePed = false,
      pedModel = "s_m_m_lathandy_01",
      marker = { id = 21, size = { x = 0.3, y = 0.3, z = 0.3 }, color = { r = 255, g = 255, b = 255, a = 120 }, bobUpAndDown = 0, faceCamera = 0, rotate = 1, drawOnEnts = 0 },
      slots = 10,
      weight = 50000,
    },
  }
}
</pre>
