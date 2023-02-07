# space-game-releases

## preAlpha-releases

#### 0.1.4
As I'm planning out my prototype for itch.io i noted down the most things i want to be inside a release when i publish it on itch.io.
This brings also a lot of rework of the old code, most of the this are now quite better than before because I'm much more into things and how they should be used. One example here is the use of the Eventsystem. As i have an generic way of using Events for certain things i keep simplyfying the code and decoupling the gameobjects by using events to notify about changes. And as i was lerning Unity my code from the beginning was a huge chain of dependencies which are now just one Event from one GameObject to another whitout providing the GameObject to all Object that need to get notified of data from for example the userdata.

The things to highlight that are new in this Release are:
* With the use of events i Created a generic timerobject that can perform many different timer related parts by only usig events.
* The Cutscene is now fully clickable to get to the next page and there is no need to click on an arrow button
* The same counts for the LevelUp UI it has now a fullscreen button in the back to close the UI with any touch
* The UI panel when clicked on an obstackle are now using the full screen hight and not being too small for the buttons in them
* The space station now shows the bonus you get for certain values when youre inside the station designer
* Rewriting the complete Network funktionalties to use the UnityWebRequest module as the http Modulse is deprecated and blocking processes
* To reduce the nework calls the mission of the characters are now defined as scriptableobjects and stored inside unity as they where static 
* A new button is on the screen for providing direct feedback
* After registration you are now directly loged in and forwarded to the cutscene
* A new button is added to handle special missions for the characters (Special missions are as well a scriptable object)

Also some small changes like:
* Panelsize for clickable objects are adapted to be more intuitive
* The tutorial now overlaps the hole screen
* EP values for level ups are changed a bit to be not faster then the ressources to get (rooms unlocked but not able to have enough money to buy them)


Besides this changes during the work for this release im still improving my website. As for now most of the content is still in progress and some might not exist at all. But if youre interested check it out under [bau.steinchen website](http://bau-steinchen.duckdns.org/)

##### Release reason
Alot of things happened during the preparation for the itch.io release and this progress should be reflected in the releses

##### Known problems
* applying a room to a tile where already a room is will override the current room

#### 0.1.3
As i was worrying about the gameplay fun on my game I decided to create a prototype that contains most of the core mechanics that I wanted to implement. This will be released on itch.io to see how other players feel the gameplay. I hope i get a lot of valuable feedback out of this that i can go back into the extension of the game progressions.    
Beside this release on itch.io this release contain multiple things that i manage to implement already. First of all for a more appealing look i created a boarder around the space station that i feel more realistic not only cards sticked together.
Also i implemented a new background handler that is not interfering with the station itself. I still need to do this for the planet that is behind the station. For example if you zoom out the plance shrink aswell.
Also i started to implement the bonus functionality that you can gain by added new rooms on the space station. The basics are done and already taking into account e.g. if you finish an mission the bonus will increase your earned coinvalue.
Removing obstacles is now blocked behind reaching level 1.

Some smaler updates are:   
* Creating new elevator handler for fixing the glitched doors
* Removing lots of unnecessary debug logoutput and general code cleanup
* Fixed clicking panels that ore opening panels from objects behind the current panel
* Dive deeper in particles and create a stars effect for the login screen
* Updated API models to also save/load data like profession etc 
* Missions also add EP to the character
* Reimplement Event handling in a more generic way (your coins already updated unsing this handler)
* Adapt some of the panels to be closed when clicked outside of the panel

Besides this changes during the work for this release im still improving my website. As for now most of the content is still in progress and some might not exist at all. But if youre interested check it out under [bau.steinchen website](http://bau-steinchen.duckdns.org/)

##### Release reason
Its a new year (2023) and this brings a lot new motivations to start with tasks i was struggleing with. But also there are new worries about the gameplaymechanics so i decided to create a prototype release for itch.io

##### Known problems
* clicking the new arrow on the cutscene is only working in the corner
* The UI panel for removing the obstacles is a bit too smal and has floating buttons
* applying a room to a tile where already a room is will override the current room


#### 0.1.2
The changes in this release bring some changes that are needed for the future work of the game. The biggest change is the station designer and the abbility to buy rooms on the station. The room can be bought with the station designer after you reached level 3. This level enable also the first room (Canteen) that can be bought. In the station designer you see colored tiles that are defining the states of the station tile underneath.
Note: You need to remove obstacles to have free spaces where the rooms can be applied to.

* gray - This is the command bridge and cannot be changed at all.
* red - This tile is blocked by an obstacle you need to remove it first.
* yellow - This tile is free and you can buy a room on this tile.
* green - This tile already has a room on it's tile. Buying a new room will override the old one.
* The elevator will stay unchanged in the station designer.

For this changes i need to rewrite the most parts of the current tilemap that is used for the space station. The tilemap is now organized in layers that are currently ssplit into Obstacle, Movable(where characters and so can move), Station and a background that is not used currently.

Besides this changes during the work for this release i managed to use a new website design to build a more general website that also include some more topics beside the gamedevelopment. As for now it is still in progress and some of it contents is non existent for now but i'm quite happy with the progress and the new look. If youre interested check it out under [bau.steinchen website](http://bau-steinchen.duckdns.org/)

##### Release reason
After a long time of development i will bring the newest changes of the game to show the progress and new features.

##### Known problems
* clicking the new arrow on the cutscene is only working in the corner
* The UI panel for removing the obstacles is a bit too smal and has floating buttons
* clicking on the button to remove the obstacles could open the panel of the obstacle behind it
* clicking to apply a room on the space station could open other panels.
* applying a room to a tile where already a room is will override the current room


#### 0.1.0
This release brings quite a lot of changes to the game. Firstly the first parts of the UI are reworked to not look that plane as before. Most of the UI Frames are with a transparency to look more natural in the Scene. 
The second changes are obstacles that are applied to the space station. Character avoid walking to tiles that are blocked by obstacles. You can click on the obstacles to remove them. Currently they are quite expensive and not balanced with the reward you get from the missions.

Additional changes:
* New prefab for the obstacles
* introduced 4 new materials that are needed for character upgrades
* particles are spawned on earning coins

##### Release reason
The Reason for this release is to gether feedback about the new desinged UI and also about the obstacles.

##### Known problems
* clicking the new arrow on the cutscene is only working in the corner
* The UI panel for removing the obstacles is a bit too smal and has floating buttons

