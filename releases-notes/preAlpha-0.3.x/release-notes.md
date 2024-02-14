# lunastation-releases

## preAlpha-releases

# 0.3.2
For this release there are many different parts involved where features where added and things have changed. Also the hole ui in the gameview is now build from the same schema like the sign in and cutscene.

The next big part is my Mission Manager. This object handle all related things regarding the missions for the characters and the special mission. This takes effect because i use scriptable objects for missions instead of REST calls to the API. The things are already in place for the ship missions that will also be included inside the Mission Manager. That means i do not have to save all the missions the character have inside the database. All missions are stored as scriptable objects at one songle point and not multiplied inside the database on many different characters.

This also provide the functionality i want to have with leveling up the character, so the different level provide more/different missions. Every character now get a new missionlist after finishing a mission. In the Future this will bring more randomnes to the play and maybe some kind of differentiaton between characters.

On the UI side a new loading screen is implemented to show the progress loading the game view and the game view get an black screen at startup and fade in the UI and the space station. This hides loading all the data into the ui elements and disabling buttons if they are not needed.

Fixed Problems:
* guest users are not able to skip the intro cutscene
* character now get a new list of missions if they are about to display them but their missionlist ist still empty (mostly for new characters)
* the new ui for the player info screen was too big and parts where outside the screen
* sign up now have a check if a local progress should be inserted with the registration(before it was not able to register because the local progress was blocking the new dataset)
* Guest user now getting the full game data associated only by the id not the username
* sign up input fields are now scaled correct with the screen size
* there is the functionality to request a new password. The functionality to change password is still missing



### Release reason
After the last version a lot of visauals where changed and bugfixes are solved. Most of the Gameview UI elements are changed and build in the same assets like the startup.

Known problems
* applying a room to a tile where already a room is will override the current room
* When a special mission is finsihed and the game is restartet the cooldown timer for the special mission is gone.    
* guest player that used the optional player name cant use the local progress because the username is already used and bind to the progress
* Request sending an new password is not correctly sending an email or may sending no email at all
* the character mission list is just a mock up and not all information can be provided correctly 

#### 0.3.1
This version recover all systems after a datalos on the server. Sadly an poweroutage corrupted the drives on the server and make the files unreadable. So the drives data need to be recovered. Most of the Game and website related files are stored inside a git repository and just need to be ported to a new server with updating the routes for the api and the database. But all data contained in the database ist lost for now. That is sad even if there was only the data in development state but all written blogposts for the website are still los. I'll try my best to recover them.

Also in this release the name of the game is inserted into all settings and i use the created ship sprite that is kind of useless inside the game because you need level 10 for ships and they are not implemented yet, i use it at icon image.

Features and Fixes:
* The touch input on mobile devices are fixed by using event trigger instead of onClick (e.g. mouse clicks) 
* Special Missions are again usable with the characters directly from special mission menu
* Increasing the mission reward to better allign with the level ups and the new features that are needing coins
* Loading a game update the concurrent Mission panel to the correct number
* Fix the problem that loading with an active special Mission set the remaining mission timer as cooldown
* The Missions are no longer stored in the database, from now on as scriptable objects

Release reason
Restored after dataloss on a new powerfull server and small fixes for the mobile version

Known problems
* Applying a room to a tile where already a room is will override the current room 
* When restarting the game with an active special mission the counter for the current active missions could be increased permanently
* loading a game sets the remaining time for the special mission as cooldown timer




