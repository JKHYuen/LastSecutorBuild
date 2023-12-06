# *Last Secutor* - Tech Demo (2014 — 2022)
*Uploaded for my game development portfolio, see https://jkhyuen.github.io/last-secutor for full details.*

***Windows 64-bit required** 

![last-secutor](https://github.com/JKHYuen/LastSecutorBuild/assets/53157428/2eb9e8d6-0fd0-4f9e-8589-0ca0a219762a)

*Last Secutor* is an unfinished 2D turn based RPG with ARPG inspired mechanics such as an original skill tree system, expansive loot, and complex character progression. These demos are intended to provide interactive examples of all the technical and gameplay features mentioned in the portfolio page. Most of the game content (audio, visuals) is placeholder.

## To Start:
Pick one of the two builds and launch the exe listed below.

## 1. **Main Tech Demo**:
*Last Secutor Tech Demo\Last Secutor.exe*

Fully playable vertical slice of the game. To start combat from town, click the colosseum in the background. Click start in the popup menu without selecting any quest fights to start combat with a random AI. 

Notable features:
 - All working skills are available by default, right click bottom skill bar to assign skills. You can change skills and equipment in combat, this would not be possible in real gameplay.
 - Get items in town from the two alien characters on the left to try the inventory system (all items are free)
 - Items can be acquired in combat by entering "shop 1" in console. Press ```X``` to open shop menu.
 - Open the skill tree window by pressing ```X```, then pressing the "Skill Tree" tab. Right click on the grey squares to pick a skill tree. Enter "sp" in console to get skillpoints.
 - Press the "Help" button on the bottom bar for a simple, searchable game encyclopedia.

Note:
 - skill costs and cooldowns are disabled by default. Enter "f" in console to toggle costs. Most skills do not have an assigned skill cost.
 - skills and equipment are not saved when entering combat scene, unless ```F5``` is pressed in town and ```F6``` is pressed in combat.
 - Number values (e.g. damage, health) are unfinished. Combat is not balanced.

## 2. **AI vs AI Battle Demo**: 
*Last Secutor AI vs AI\Last Secutor (AI DEMO).exe*

This build loads directly into a combat scene with two AIs fighting. No user input is required. This demo is designed to quickly show different AI behaviors  and combat interactions. Press ```F6``` to load new random AIs. 

Note:
 - Console commands and time scale control (see below) can still be used
 - the game was not designed to have AI fights, this was added only for debugging purposes
 - AI actions UI only works for the right side (some AIs don't use the action system regardless, see "AI Combat" section on portfolio page for full details)

## Controls
       ~:  Toggle console (enter "h" to view all commands)
       X:  Open right side menu (inventory, skill tree, quest journal)
     Esc:  Open game menu
      F5:  Save (Serialize items, skill trees, and skills)
      F6:  Load (Reload current scene with first user save found)
      
    COMBAT ONLY
       B:  Open battle log
       P:  View enemy stats
     0-9:  Shortcut keys for skill bar
    PgUp:  Speed up time scale
    PgDn:  Slow down time scale
     End:  Set time scale to 0
    Home:  Set time scale to 1

## Persistent Data Note:
Unity log files are created when the game boots up, user save data is also created if ```F5``` is pressed. These files are small (~15KB), but the location is the following you wish to delete these files:

*C:\Users\<user>\AppData\LocalLow\KHY\Last Secutor*\
*C:\Users\<user>\AppData\LocalLow\KHY\Last Secutor (AI DEMO)*
