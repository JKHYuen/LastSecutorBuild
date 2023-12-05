# *Last Secutor* (Cancelled 2D Turn Based RPG) - Tech Demo
*Uplaoded for my game development portfolio, see https://jkhyuen.github.io/last-secutor for full details.*

These demos are intended to provide interactive examples of all the technical and gameplay features mentioned in the portfolio page. Most of the game content (audio, visuals) is placeholder and there may be bugs.

## There are *two* seperate builds:
### 1. **Main Tech Demo**:
*Last Secutor Tech Demo\Last Secutor.exe*

Fully playable vertical slice of the game. To start combat from town, click the colosseum in the background. Click start in the popup menu without selecting any quest fights to start combat with a random AI. 

Notable features:
 - All working skills available by default, right click bottom skill bar to assign skills.
 - Get items from the two alien characters on the left to try inventory system (all items are free)
 - Open skill tree window by pressing ```X```, then pressing "Skill Tree" tab. Right click on the grey squares to pick a skill tree. Enter "sp" in console to get skillpoints.

Note the following caveats:
 - skill costs and cooldowns are disabled by default. Enter "f" in console to toggle costs. Most skills do not have a asigned skill cost.
 - Number values (e.g. damage, health) are unfinished. Combat is not balanced.
 - skills and equipment are not saved when entering combat scene, unless ```F5``` is pressed in town and ```F6``` is pressed in combat.

### 2. **AI vs AI Battle Demo**: 
*Last Secutor AI vs AI\Last Secutor (AI DEMO).exe*

This build loads directly into a combat scene with two AIs fighting. No player input is required. Press ```F6``` to load new random AIs. 

Note:
 - Console commands and time scale control (see below) works
 - the game was not designed to have AI fights, this was added only for debugging purposes
 - AI actions UI only works for the right side (some AIs don't use the action system regardless, see portfolio page for full details)

### Controls
```~```     Toggle console (enter "h" to view all commands)\
```X```     Open right side menu (inventory, skill tree, quest journal)\
```Esc```   Open game menu\
```F5```    Save (Serialize items, skill trees, and skills)\
```F6```    Load (Reload current scene with first user save found)\

```B```     Open battle log (combat only)\
```P```     View enemy stats (combat only)\
```0 - 9``` Shortcut keys for skill bar\
```PgUp```  Speed up timescale\
```PgDn```  Slow down timescale\
```End```   Set time scale to 0\
```Home```  Set time scale to 1

## Persistent Data Note:
Unity log files are created when the game boots up, user save data is also created if ```F5``` is pressed. These files are small (~15KB), but the location (Windows) is the following you wish to delete these files:

*C:\Users\<user>\AppData\LocalLow\KHY\Last Secutor*\
*C:\Users\<user>\AppData\LocalLow\KHY\Last Secutor (AI DEMO)*\
See [here](https://docs.unity3d.com/ScriptReference/Application-persistentDataPath.html) for other operating systems.
