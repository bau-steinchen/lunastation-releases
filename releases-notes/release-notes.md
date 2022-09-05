# space-game-releases

## preAlpha-releases
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


#### 0.0.8
This release will bring the following improvements

* Introduces an new text font that is used in the game now with a pixelated style
* a basic shop design is introduced and will be used to gather feedback until the finishing up with graphics and images

##### Release reason
The Reason for this release was to gather feedback about the basic functionality of the shop and the new pixelated font style.


#### 0.0.6
This release give the player the opportunity to save his user data to server

* and into text is showing that it using a development build
* the intro is only shown for the first startup of a new registered member
* currently only one character is usable for the user
* a mission that is not finished when closing the app will be changed and the reward will be provided on the next login

There need to be some changes made in the back-end to provide more flexible characters in the future. The current test characters are hard-coded

##### Release reason
The gameEngine is basically finished and open for feedback. The Shop and the Space station not finished.

#### 0.0.4
This release has multiple bugfixes that are gathered from the feedback.
The main bugfixes are:

* removed Userlevel from userdata and calculate via current ep
* only 2 characters where allowed to entered for passwords
* different problems in the communication with the database trough the API
* improving the error messages shown to user when API call failed

In addition to the bugfixes the app get some new features.
The main features are:

* A complete new scene that can show cutscenes to introduce story telling
* The API get a new route to handle cutscenes with text, image and an image for speaker
* The http Request module is using the dns name to the server now that make the app access the API from outside of the local network
* Refactor and delete old unused code that can cause confusion for different type of implementations

##### Release reason
The main reason for releasing this version is to get feedback about the registration and the new cutscene because with the dns included other people can give their feedback too. They do not need to be part of my local network anymore.

#### 0.0.1
##### First Release
This release is the very initial first release to test basis behavior on mobile devices.

The main features are:
* Login
* Register of new Users
* Userdata is saved to the server
* Userdata is loaded from server
* Simple space station is in place
* 2 dummy character walking around in the space station
* The character have dummy missions to be started
* Gaining xp and coins for the user through character missions

##### Release reason
* The main reason for this release is to gather some feedback and test the app on mobile devices
