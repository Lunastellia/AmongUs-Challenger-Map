# AmongUs-Challenger-Map

• ChallengerLevel is a mod that allows adding maps to Among Us. The mod comes from AmongUs Challenger.

## Exclusive available maps:

• Challenger Polus / Polus Nuclear (version 2.0)

• Mira Challenger (version 2.1)

• Challenger Skeld (version 1.1)


## Other available maps:

• Better Polus (By brybry)

• Better Skeld (By Dadoum)


## Advise, Licence & Copyright

-> The mod is not distributed as open source; it is protected by copyright (Oriana / OrianaGames.com) and a custom license. You can use the files as they are and combine them with other mods. However, any modification, reproduction, or commercial use is strictly prohibited. You must also retain the visible watermark in the game (information text under the "ping"). If you want to integrate the maps into your mods, you must add links to this repo and AmongUs Challenger as credits on your GitHub page, mentioning the author's name and the initial project as follows: "AmongUs Challenger - Maps Nuclear Polus & Challenger Mira by Lunastellia."

## Installation

-> We recommend using ModManager for installation, either combined with other mods or for a simple installation.

-> Installation without mod manager: Make sure you are using a version of the game similar and compatible with the version of the map you're using, download all the files and then copy/paste them into your Among Us game folder.


## Information for Developers

*- If you edit the settings, you must patch them before launching the game. Once the game is launched, the map will be constructed directly based on the indicated values!
Exemple : patch in " [HarmonyPatch(typeof(HudManager), nameof(HudManager.Update))]" and use this condition "if (AmongUsClient.Instance.GameState != InnerNetClient.GameStates.Started)" then link your settings to edit the different values, exemple "if (Setting_polusID == 1 && !polusID != 1) { polusID = 1; };". this way no matter how your settings work you should be able to link them to the ChallengerLevel settings*

*- Compatibility: The used RPCs (Remote Procedure Calls) are 230 to 234. don't use the same values ​​otherwise it won't work properly*

**-> Way for edit maps settings : "ChallengerLevel.Setting"**

**Map Selection Settings**

• (float) polusID => 0-2 [Defaut 2] (0 - Normal, 1 - Better by BryBry, 2 - Challenger & Nuclear By Lunastellia)

• (float) miraID => 0-1 [Defaut 1] (0 - Normal, 1 - Challenger By Lunastellia)

• (float) skeldID => 0-2 [Defaut 0] (0 - Normal, 1 - Better by Dadoum, 2 - Challenger By Lunastellia)

• (float) airshipID => 0 [Defaut 0] (0 - Normal)

**Challenger/Nuclear polus settings Settings**

• (bool) polusNuclear_Enable => True/False [Defaut True] (Enable Nuclear polus)

• (float) polusNuclear_SpawnChance => 0-100 [Defaut 100] (Chance to spawn nuclear polus in Challenger polus map)

• (float) polusNuclear_Timer => 60-240 [Defaut 90] (Nuclear timer)

• (float) polusNuclear_RandomTimer => 60-240 [Defaut 90] (Additional random range for Nuclear timer)

• (float) polusNuclear_AlertTimer => 10-40 [Defaut 25] (Alerte Nuclear duration)

• (float) polusNuclear_TimerVisibility => 0-2 (0 - Timer hide for everyone, 1 - everyone can show Nuclear the  timer, 2 - Only impostors can show the timer)

• (bool) polusNuclear_RandomSide => true/false [Defaut True] (if true, you can select "polusNuclear_RamdomLevel" for change difficulty mod)

• (float) polusNuclear_RamdomLevel => 0-6 [Defaut 1] (0 - Normal, 1 - Medium, 2 - Hard, 3 - Very Hard, 4 - Nightmare, 5 - Very easy, 6 - Easy)

• (bool) polusNuclear_Fixed_Lab => true/false [Defaut false] (Select this elements destroyed after alerte only if polusNuclear_RandomSide = false)

• (bool) polusNuclear_Com => true/false [Defaut false] (Select this elements destroyed after alerte only if polusNuclear_RandomSide = false)

• (bool) polusNuclear_Weapon => true/false [Defaut false] (Select this elements destroyed after alerte only if polusNuclear_RandomSide = false)

• (bool) polusNuclear_O2 => true/false [Defaut false] (Select this elements destroyed after alerte only if polusNuclear_RandomSide = false)


**Challenger Mira Settings**

• (float) MiraDroneSurvSpeed => 1-6 [Defaut 3] (ajust the drone Speed in mira challenger)

• (Keycode) KeycodeDroneRight => [Defaut KeyCode.D] (Modify the Keybind for the drone)

• (Keycode) KeycodeDroneLeft => [Defaut KeyCode.A] (Modify the Keybind for the drone)

• (Keycode) KeycodeDroneUp => [Defaut KeyCode.W] (Modify the Keybind for the drone)

• (Keycode) KeycodeDroneDown => [Defaut KeyCode.S] (Modify the Keybind for the drone)


**-> Way for important data : "ChallengerLevel.Data"***
*(You can use the following values to make minor internal modifications, but be cautious of potential conflicts)*


• (bool) BreakTime => true/false [Defaut false] (Use this if you want to temporarily stop the timer, affects both the timer and the alert)

• (bool) ScreenColored => false/True (ignore Yellon screen during the alerte)


**-> do not modify this, only use get)**


• (bool) PolusNuclear => (Map Polus nuclear enabled)

• (bool) IsMapPolusV2 => (Polus Nuclear Alerte finished and map destroyed)

• (int) NuclearSide => 0-16 (identifies which SIDE is active) 

• (bool) TransformNuclear1 => (identifies which part of the map is destroyed and activates collisions and displays sprites)

• (bool) TransformNuclear2 => (identifies which part of the map is destroyed and activates collisions and displays sprites)

• (bool) TransformNuclear3 => (identifies which part of the map is destroyed and activates collisions and displays sprites)

• (bool) TransformNuclear4 => (identifies which part of the map is destroyed and activates collisions and displays sprites)

      
• (int) timerN => (allows to retrieve the value of the timer)

• (int) timerLN => (allows to retrieve the value of the alerte timer)

• (float) SafeTimer => (allows you to know if the player is in a safe zone or in danger, if the value is greater than 0 the player is safe, otherwise he will be killed at the end of the alert)

   
• (bool) StartNuclear =>  (Execute once at the end of the alert to exit the loop)

• (bool) StartSabNuclear => (Execute once at the start of the alert to exit the loop)

• (bool) EmergencyDestroy => (the alert is active the sabotage and the buzz are deactivated during this period)

• (bool) SetNuclearTimeOn => (allows to decrease the time on the timer)

• (bool) SetNuclearSabTimeOn => (allows to decrease the time on the Alerte timer)


•  *avoid using the other functions in the data or risk breaking the functioning of the mod*



