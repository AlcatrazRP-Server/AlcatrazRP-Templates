# Placeable and throwable items
- [Back to Main Page](../README.md#alcatraz-templates)  

These are actually quite easy. You just have to prop hunt for the right props.  
I am not super familiar with props and their shorthand meanings, but here is a useful website for finding GTA props:  
- [Forge Plebmasters](https://forge.plebmasters.de/objects)  

This example uses a brick of cocaine. The name stored in code is coke_brick. Just put in whatever name you see in your inventory, spaces included i.e. Coke Brick  
Change to false for the first two fields if you do not want it thrown or dropped, respectively.  
Sizes are what prop will be shown based on how many you drop.  
In the example below,  
- if a player drops 1-4 coke brick in their inventory it will display the 'hei_prop_hei_drug_pack_01a' prop when dropped/thrown  
- at 5 or more dropped it will be shown as the 'hei_prop_hei_drug_pack_01b' prop  

```lua
['coke_brick'] = {
    canBeThrown = true,
    canBeDropped = true,
    sizes = {
        [1] = 'hei_prop_hei_drug_pack_01a',
        [5] = 'hei_prop_hei_drug_pack_01b',
    }
},
```