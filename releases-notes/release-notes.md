# space-game-releases

## preAlpha-releases
#### 0.1.0
This release brings quite a lot of changes to the game. Firstly the first parts of the UI are reworked to not look that plane as before. Most of the UI Frames are with a transparency to look more natural in the Scene. 
The second changes are obstacles that are applied to the space station. Character avoid walking to tiles that are blocked by obstacles. You can click on the obstacles to remove them. Currently they are quite expensive and not balanced with the reward you get from the missions.

Additional changes:
* New prefab for the obstacles
* introduced 4 new materials that are needed for character upgrades
* patricles are spawned on earning coins

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
