# 7d2dWalkerSim
C# mod for 7 days to die game (https://7daystodie.com/).
Credits for initial version go to ZehMatt with his work https://github.com/ZehMatt/7dtd-WalkerSim .

Mine version starts with game's Alpha 20 adaptation + some adjustments in Simulation and fixes as:
- Fixed state saving to mod's bin file. I noticed, that zombies location and numbers was resetted at every game startup (like when you use "walkersim reset" cmd).
- Changed walking behaviour: zombies now target the closest 5 POIs, not random on the whole map. So if you use high POITravellerChance, this would lead to zombies staying near their original POIs. For example, a big number of them would walk in a city, but won't stray far from it! With default behavior, they get spayed equally all over the map past time disregard the actual location (even amounts in the woods and cities).
- Changed respawn logic a bit: now killed zomibes enque to respawn to for a big amount of days. So you can feel, how you clean the world around you. No more non-stop zombies flow. I compensate this ingame with high population, high value of max zombies and high chance to spawn at POIs. Future todo: make this configurable for users. Currently it's BloodMoonFrequency * 

# Installation 
Create new folder for the mod in yors 7d2d "Mods" directory (create it, if it's your firts mod)
- Make sure you have "Mods" directory in your game for mods (https://7daystodiemods.com/how-to-install-7-days-to-die-mods/).
- Create new forlder for this mod named, "WalkerSim". Name should match exactly!
- Copy files from this repo "assets" directory to new mod's folder.
- Copy dll from this repo "bin/Release" directory to new mod's folder.
- Done!
