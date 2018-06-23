# ZPS Infection Stocks
This is an include file and an associated gamedata specifically for infection-based plugins in ZPS. On its own, it does nothing, but it can be used to create plugins that utilize the ZPS infection functions used on players.

# How To Install
The files are setup in the same directory structure as they would be for a regular sourcemod install, so simply download the files, copy the addons folder into your game server's main directory, and copy over any files (if necessary).

1.0 Initial Update (6-20-2018)
------------------------------------------
- Added all relevant infection game data and associated offsets. At this time, these offsets are the working/correct offsets.
- A few notes about the method calls: 
    * Infect/ForceInfect are similar in that both require a float to ADD time to the infection timer. If you want to reduce time, you must use negative numbers. 
    * The difference Infect/ForceInfect is that Infect is for basic infection (ie: whitey hits you) and ForceInfect is for (or is assumed for) infecting a player when no zombies exist on the server.
    * UnInfect has no return values or variables to pass. It is simply a method that is called when a player needs to have infection removed.