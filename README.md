# AmongUs-Challenger-Map

ChallengerLevel is a mod that allows adding several maps to Among Us. The mod comes from AmongUs Challenger.

### Exclusive available maps:

Challenger Polus / Polus Nuclear (version 2.0)
Mira Challenger (version 2.1)
Challenger Skeld (version 1.1)
Other available maps:

Better Polus (By brybry)
Better Skeld (By Dadoum)
Warning

The mod is not distributed as open source; it is protected by copyright and a custom license. You can use the files as they are and combine them with other mods. However, any modification, reproduction, or commercial use is strictly prohibited. You must also retain the visible watermark in the game (information text under the "ping"). If you want to integrate the maps into your mods, you must add links to this repo and AmongUs Challenger as credits on your GitHub page, mentioning the author's name and the initial project as follows: "AmongUs Challenger - Maps Nuclear Polus & Challenger Mira by Lunastellia."

Installation

We recommend using ModManager for installation, either combined with other mods or for a simple installation.
Make sure you are using a version of the game similar and compatible with the version of the map you're using.
Installation without mod manager: Download all the files and then copy/paste them into your Among Us game folder.
Information for Developers

Compatibility: The used RPCs (Remote Procedure Calls) are 230 to 235.

**CONFIG**

*ChallengerLevel.Setting*

polusID => 0-2 [Defaut 2] (0 - Normal, 1 - Better by BryBry, 2 - Challenger & Nuclear By Lunastellia)
miraID => 0-1 [Defaut 1] (0 - Normal, 1 - Challenger By Lunastellia)
skeldID => 0-2 [Defaut 0] (0 - Normal, 1 - Better by Dadoum, 2 - Challenger By Lunastellia)
airshipID => 0 [Defaut 0] (0 - Normal)

polusNuclear_Enable => True/False [Defaut True] (Enable Nuclear polus)
polusNuclear_SpawnChance => 0-100 [Defaut 100] (Chance to spawn nuclear polus in Challenger polus map)
polusNuclear_Timer => 60-240 [Defaut 90] (Nuclear timer)
polusNuclear_RandomTimer => 60-240 [Defaut 90] (Additional random range for Nuclear timer)
polusNuclear_AlertTimer => 10-40 [Defaut 25] (Alerte Nuclear duration)

polusNuclear_TimerVisibility => 0-2 (0 - Timer hide for everyone, 1 - everyone can show Nuclear the  timer, 2 - Only impostors can show the timer)

polusNuclear_RandomSide => true/false [Defaut True] (if true, you can select "polusNuclear_RamdomLevel" for change difficulty mod)
polusNuclear_RamdomLevel => 0-6 [Defaut 1] (0 - Normal, 1 - Medium, 2 - Hard, 3 - Very Hard, 4 - Nightmare, 5 - Very easy, 6 - Easy)

polusNuclear_Fixed_Lab => true/false [Defaut false] (Select this elements destroyed after alerte only if polusNuclear_RandomSide = false)
polusNuclear_Com => true/false [Defaut false] (Select this elements destroyed after alerte only if polusNuclear_RandomSide = false)
polusNuclear_Weapon => true/false [Defaut false] (Select this elements destroyed after alerte only if polusNuclear_RandomSide = false)
polusNuclear_O2 => true/false [Defaut false] (Select this elements destroyed after alerte only if polusNuclear_RandomSide = false)

MiraDroneSurvSpeed => 1-6 [Defaut 3] (ajust the drone Speed in mira challenger)

KeycodeDroneRight => [Defaut KeyCode.D] (Modify the Keybind for the drone)
KeycodeDroneLeft => [Defaut KeyCode.A] (Modify the Keybind for the drone)
KeycodeDroneUp => [Defaut KeyCode.W] (Modify the Keybind for the drone)
KeycodeDroneDown => [Defaut KeyCode.S] (Modify the Keybind for the drone)

**IMPORTANT DATA**

*ChallengerLevel.Data*

BreakTime = false/True (stop all nucleartimer)
ScreenColored = false/True (ignore Yellon screen during the alerte)
BlockSab = false/True (block the sabotage)

- avoid using the other functions in the data or risk breaking the functioning of the mod

- 
