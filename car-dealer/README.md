# Car Dealership template
- [Back to Main Page](../README.md#alcatraz-templates)  
- [Car Categories](#categories)
- [Dealership Template](#dealership-template)
- [Giant List of Cars](./cars/README.md#custom-cars)

## Data needed:
Go through and look for the lines that say: -- NEEDED: CHANGE ME!!  
Just get the vector3 coordinates, and paste them in to the appropriate spots.  
Highlight the whole vector3 or vector4, and replace with your own coordinates. Must match original type (vector3 or vector4)  

### Categories
Select from the categories to determine which vehicles the dealership can sell
- "planes"  
- "sportsclassics"  
- "sedans"  
- "compacts"  
- "motorcycles"  
- "super"  
- "offroad"  
- "helicopters"  
- "coupes"  
- "muscle"  
- "boats"  
- "vans"  
- "sports"  
- "suvs"  
- "commercial"  
- "industrial"  
  
### Dealership Template
Copy the template below, and replace appropriate fields  
```lua
["pdm"] = {
  type = "owned",
  openShowroom = {
    coords = vector3(-55.99, -1096.59, 26.42),
    size = 5
  },
  openManagement = {
    coords = vector3(-30.43, -1106.84, 26.42),                  -- NEEDED: CHANGE ME!! This is the Car Dealers boss menu location
    size = 5
  },
  sellVehicle = {
    coords = vector3(-27.89, -1082.1, 26.64),                   -- NEEDED: CHANGE ME!! This is where customers can sell their car back
    size = 5
  },
  purchaseSpawn = vector4(-13.68, -1092.31, 26.67, 159.82),     -- NEEDED: CHANGE ME!! Where a newly purchased vehicle will spawn
  testDriveSpawn = vector4(-49.77, -1110.83, 26.44, 75.94),     -- NEEDED: CHANGE ME!! Test drive spawn location
  camera = {
    name = "Car",
    coords = vector4(-146.6166, -596.6301, 166.0, 270.0),
    positions = {5.0, 8.0, 12.0, 8.0}
  },
  categories = {"sedans", "compacts", "motorcycles", "offroad", "coupes", "muscle", "suvs", "sportsclassics"},    -- NEEDED: CHANGE ME!! Refer to list of categories above
  enableTestDrive = true,
  hideBlip = false,
  blip = {
    id = 326,
    color = 2,
    scale = 0.6
  },
  enableSellVehicle = true, -- Allow players to sell vehicles back to dealer
  sellVehiclePercent = 0.6,  -- 60% of current sale price
  enableFinance = true,
  hideMarkers = false,
  markers = { id = 21, size = { x = 0.3, y = 0.3, z = 0.3 }, color = { r = 255, g = 255, b = 255, a = 120 }, bobUpAndDown = 0, faceCamera = 0, rotate = 1, drawOnEnts = 0 },
  showroomJobWhitelist = {},
  showroomGangWhitelist = {},
  societyPurchaseJobWhitelist = {},
  societyPurchaseGangWhitelist = {},
  disableShowroomPurchase = false,
  job = "cardealer", -- Owned dealerships only
  directSaleDistance = 50,
},
```
