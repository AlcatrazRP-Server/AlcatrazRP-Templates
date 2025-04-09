# Boss menu
- [Back to Main Page](../README.md#alcatraz-templates)  
  
Super simple. Need to change the whole line, but it's straightforward  
- ballas: name of the "job/gang"
- bossCoords = {vector3(...), vector3(...)}
- dutyCoords = {vector3(...), vector3(...)}

### Multiple locations for one job
Multiple boss menus can be placed for one job. I.e.  
- police in Paleto and MRPD can access the same global funds if part of the same department/job    
Same thing with the dutyCoords, or the clock-in location.  
Police and Ambulance have built in dutyCoords (clock in/out), but still need bossCoords (boss menu) to access menu.  
Copy and paste the one line below, and change as needed
```lua
['ballas'] = { bossCoords = {vector3(114.18, -1960.81, 21.33)}, dutyCoords = {vector3(109.48, -1961.42, 20.96)} },
```

For only the menu and no clock in/clock out, you can leave dutyCoords empty like so:  
```lua
['police'] = { bossCoords = {vector3(114.18, -1960.81, 21.33), vector3(114.18, -1960.81, 21.33)}, dutyCoords = {} },
```
Separating two or more coordinates with a comma will allow for the same menu at multiple locations
