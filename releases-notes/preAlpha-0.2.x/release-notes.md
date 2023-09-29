# space-game-releases

## preAlpha-releases

#### 0.2.2
This version provides some Bugfixes and also some new Festures. One of the main Features is that i now have a decent ui design that i will evolve for the game. Currently only the startup view with the sign up/in and the cutscene are basically changed but will be improved with future updates and feedback.

Also one big change you will notice when starting the game is a new button with the text "GUEST" on it. This button will be in the near future start the game with dummy values for most of the user part. Currently the API ist not updated accordingly to have all "guest" features but the ui is prepared for it.

Besides the new ui the game itself got multiple fixes and new features. Below is a detailed list with all the things happened to the game besides it is still using the old ui:

Features and Fixes:
* the data for special missions are now stored correctly in the database when reaching level 7 or above and starting the game, the station designer was not showing correctly
* Fixed the display time of the special mission timer from end date to remaining seconds the character that was clicked by the user now gets a dummy highlight to see which character is selected
* increasing the values for the user levels to make level 20 reachable(previously only 10 levels) the user is now able to change the display name of characters
* Fixed the problem that the special mission was always resetet after game restart in the missionlist of a selected character, a banner with the stats of the character is added
* Fixed the problem the the characters are able to walk behind the station and not being visible a new ui element is added that show how many active missions ongoing.(will be extended in the future)
* the bonus values for the station and the collected parts are now displayed in percentage not some magic numbers

Release reason
Quite a lot of things where added and to test and gather feedback for the new ui elements

Known problems
* Applying a room to a tile where already a room is will override the current room 
* When restarting the game with an active special mission the counter for the current active missions could be increased permanently
* loading a game sets the remaining time for the special mission as cooldown timer

#### 0.2.1
In this version i fixed a lot of bugs and problems inside the mechanics of the game. I had a very patient tester who spend a hole evening with me testing out the mechanics and try to exploit the functionality.

Nevertheless i also implemented some small functionalities. Here the main part is that you find a new area in the top row on the ui that os highlighting the current characters that are performing a mission. In the future this will be clicable and show a list with the characters that are currently on a mission or finished a mission but the reward was not claimed yet.
The next small thing was that the game on pc can now be closed using the esc key. (Currently without an promt if you really want to close the game)

Fixed Problems:
* Fast clicking on collecting the reward on a character would increase the Concurrent mission counter permanently.
* The bonus of the station tiles where multiplied wrong ending up the canteen provide 50% coin bonus instead of 0.5%
* The text for the ep needed until the next level are calcated wrong.
* An empty string in the timer time could result in an empty gameobject for special missions because no mission is picked.

Release reason
Small updates but this release fixes multiple bugs

Known problems
* Applying a room to a tile where already a room is will override the current room
* When a special mission is finsihed and the game is restartet the cooldown timer for the special mission is gone.
* When the game is restartet while the current special mission is performing the player can start the next special mission immediately after finish of the special mission

#### 0.2.0
First of all in this release i fixed the really buggy intro. There is no forward button anymore just click anywhere to progress
For the game there where sadly no real big changes but here is a list of the most value things that have changed:    
* On the bottom left is a new button for special missions (the button will disapear when the mission is accepted until the next mission is available)
* There is now a better timer management that in used via events and can be used for varius different scenarios
* Code refactor and adding more use of events to decouple the UI from the models
* There is a linux build available from now on in the releases. If that worked out i will add windows too.

This are the main points to mention for this release as i was busy with other stuff.
Also i did a lot of work for the new website design. Still missing lots of texts for my post but the design and the structure is coming out nicely. But if youre interested check it out under [bau.steinchen website](http://bau-steinchen.duckdns.org/) and any feedback is appreciated.

##### Release reason
As there is already a lot of time since the last release and also this time including a PC release this time (Linux for now for testing)

##### Known problems
* playing on PC need to use ALT+F4 to exit
* applying a room to a tile where already a room is will override the current room


