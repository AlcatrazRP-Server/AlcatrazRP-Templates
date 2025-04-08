# Boss menu
### Super simple. Need to change the whole line, but it's straightforward  
- ballas: name of the "job"
- bossCoords = {vector3(), vector3()}
- dutyCoords = {vector3(), vector3()}

### Multiple locations for one job
Multiple boss menus can be placed for one job. I.e. police in Paleto and MRPD can access the same global funds if part of the same department  
Same thing with the dutyCoords, or the clock-in location. Police and Ambulance have built in dutyCoords, but still need bossCoords to access menu.  
<pre>
['ballas'] = { bossCoords = {vector3(114.18, -1960.81, 21.33)}, dutyCoords = {vector3(109.48, -1961.42, 20.96)} },
</pre>