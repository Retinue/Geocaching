Geocaching



chat commands:
 
'geo start'
'geo stop'
'geo dist'- distance between player and target location, and probe for cache
'geo rpt'- returns the number of current mappings.

Issues:


- Has not been tested with more than one player.

- getHighestBlockYAt (called on line 90 of CachMapper.java) yeilds a a y value approx
  65 blocks under target (or at bedrock).

- The distance required to complete geocaching is 100 blocks from target location (to compensate for
  getHighestBlockYAt() problem. 

- Formal commands have not yet been made. Until then, a playerChatListener is used.    

- Player gets a compass every time he/she starts Geocaching ('geo start').   
- I tried to null objects in hashmap (after player stops geocaching), but can't tell if Garbage Collector takes care.

Note: Source project has been included in .jar feel free to take a look.