# space-game-releases

## preAlpha-releases

#### 0.3.1
This version recover all systems after a datalos on the server. Sadly an poweroutage corrupted the drives on the server and make the files unreadable. So the drives data need to be recovered. Most of the Game and website related files are stored inside a git repository and just need to be ported to a new server with updating the routes for the api and the database. But all data contained in the database ist lost for now. That is sad even if there was only the data in development state but all written blogposts for the website are still los. I'll try my best to recover them.

Also in this release the name of the game is inserted into all settings and i use the created ship sprite that is kind of useless inside the game because you need level 10 for ships and they are not implemented yet, i use it at icon image.

Features and Fixes:
* The touch input on mobile devices are fixed by using event trigger instead of onClick (e.g. mouse clicks) 
* Special Missions are again usable with the characters directly from special mission menu
* Increasing the mission reward to better allign with the level ups and the new features that are needing coins

Release reason
Restored after dataloss on a new powerfull server and small fixes for the mobile version

Known problems
* Applying a room to a tile where already a room is will override the current room 
* When restarting the game with an active special mission the counter for the current active missions could be increased permanently
* loading a game sets the remaining time for the special mission as cooldown timer




