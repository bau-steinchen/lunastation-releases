# space-game-releases

## preAlpha-releases

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