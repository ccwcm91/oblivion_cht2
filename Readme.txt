*****************************************
     The Elder Scrolls IV
           OBLIVION
       Version 1.2.0416
*****************************************

Index:

1. Known Issues and Troubleshooting

2. Manual Errata and Addendum

3. Performance Tuning

4. System Requirements

5. Update 1.2.0416 Notes

6. Update 1.2.0214 Notes

7. Update 1.1 Notes



*****************************************
     1. Known Issues and Troubleshooting
*****************************************

-Uninstalling Shivering Isles
	Uninstalling Shivering Isles removes many files that are required by Oblivion to play. To play Oblivion after uninstalling Shivering Isles, you must first uninstall and reinstall Oblivion to properly replace the needed files.

-Installation Issue
	If you repeatedly uninstall and re-install Oblivion, certain systems will display an error message if you try to uninstall Oblivion again. To fix this, put your Oblivion disk in and run setup.exe. This will clear up the error and you can uninstall and reinstall the game.

-Saved Games 
	Your saved games are located in your \My Documents\My Games\Oblivion directory.

-Prior to Installing the Game
	Before attempting to install Oblivion, please verify that your computer meets system requirements.
	
	We also recommend that you prepare your hard drive for installation by running ScanDisk and Disk Defragmenter prior to installation. These utilities are part of Windows® and can identify and resolve problems with your disk drive which could hinder installation and/or playing of the game.
	
	To launch these programs and optimize your hard disk drive:
	
	   1. Open "My Computer".
	   
	   2. Right-click the disk drive you wish to install the game onto (usually C:).
	   
	   3. Click on "Properties".
	   
	   4. Select the "Tools" tab.
	   
	   5. Click "Check Now" to launch Scandisk.
	   
	   6. When Scandisk has completed, follow steps 1-3 and click "Defragment Now" to launch Disk Defragmenter.
	
	Note that defragmenting your disk drive can take a long time. It's a good idea to start disk defragmenter and let it run overnight.

-ATI Crossfire
	Performance on systems using ATI Crossfire will be reduced until ATI releases an updated driver with Oblivion listed as a Crossfire Compatible game.

-Error messages when launching Oblivion:

	This will appear as a missing dll error similar to "d3dx9_27.dll not found."

	This can be corrected by Exploring the Oblivion DVD. On the disk there is a folder named DXREDIST. Open the folder and run the DXSETUP.exe. This will install the version of DirectX required to run Oblivion.

-Unable to make new saves
	If the Tab key is pressed while entering a name during character creation, a problem may occur when the game goes to write a save to the save location. This is because the name of the character is included in the name of the save file used in Windows. This is most commonly a result of attempting to Alt-Tab out of the application during name entry. If this occurs, autosaves and quicksaves will continue to function correctly, but saves made through the menu will not. The issue will be fixed if the Tab is deleted when renaming the character before exiting the sewer at the end of the character generation.

	The following may also be of assistance if the character has progressed beyond character generation:

	The player name can be changed through the console by pressing the ` (tilde) key, and entering the following: player.SetActorFullName "Player Name" (where Player Name = the name of the character). Press RETURN, and then exit the console by pressing the tilde again.

	Also, saves can be made through the console by pressing the ` (tilde) key, and entering the following: save filename (where filename = the name of the save that you would like to make). Press RETURN, and then exit the console by pressing the tilde again.


-Input Problems
	Keyboard input problems could be the result of a control peripheral. Editting the Oblivion.ini may correct this issue. The Oblivion.ini file is located in the My Documents\My Games\Oblivion directory. In the [Controls] section, change the “bUse Joystick=1” setting to “bUse Joystick=0” or simply disconnect the peripheral. Make sure the settings are saved. Note, changes to the Oblivion.ini file will not be saved if Oblivion in running when the changes are made.

-Frequent Crashing possibly due to old system file
	Some users may experience frequent crashing due to an older system file. These crashes may be attributed to the 'mpeg2dmx.ax' file. Simply renaming the file to "mpeg2dmx.ax.old" may correct this issue.

-Frequent Crashing possibly due to connected HP printer
	A program related to HP printers may cause Oblivion to crash. Before running Oblivion: Press Ctr-Alt-Del to bring up the task manager. Go to the Processes Tab. Right click on any process starting with the letters HP and select End. Running Oblivion at this point may have this issue corrected. Note: The PC will need to be restarted to reinitialize printing or imaging.

-"FF" icons in the system tray
	Some users have reported having numerous "FF" icons in their taskbar during or after playing Oblivion. These icons are from a seperate video/audio decoder you may have installed in the past called "FFDShow." This program is processing the sound files for Oblivion, which some users have reported slows down the game, and can leave the icons in their system tray. Simply moving the mouse over those icons will get rid of them after you stop playing Oblivion. Uninstalling FFDShow can fix this, but it is NOT necessary. You can follow the steps below to tell FFDShow not to handle sound for Oblivion.

	Instructions for disabling the FFDShow for Oblivion without fully removing it:

	1. Click Start
	
	2. Click "All Programs" (or just Programs, depending on the version of Windows, whether they're using "classic," etc.)

	3. Go to the ffdshow folder.

	4. Click "Audio decoder configuration."

	5. In the left hand pane, click "Info & debug." This is the second entry in the list.

	6. In the right hand pane, near the bottom, find a check box labelled "Don't use ffdshow in:"

	7. Check that box, and in the text box underneath (it lights up when you check the check box), add "oblivion.exe" (don't include the quotes). If there is already something in that box, put a semi-colon ( ; ) after what's already there, and oblivion.exe after that. Do NOT use spaces, since ffdshow will think that's part of the filename. A valid entry would be "explorer.exe;oblivion.exe" (without quotes).

	8. Finally, click "Ok" and start Oblivion.

-Game Pad Functionality

Although the PC version of Oblivion handles best when played with a keyboard and mouse, it is possible to play the game with an assortment of game pads as well. Due to the variance in these game pads, it may be necessary to make a few changes to the Oblivion.ini file located in My Documents\My Games\Oblivion. Below is a list of the settings that can be changed to make a Xbox 360 controller attached to a PC, function better with Oblivion. It should be noted however, that because the PC version of the game was optimized to play with a keyboard and mouse, the experience will NOT be the same, as using a 360 controller on the Xbox 360 version of the game. Additionally, these settings can be applied to other game pads, but the values represented may need to be tweaked further. Finally, the mapping of the buttons will need to be determined when entering the game, and can be changed in Options - Controls, from the Main Menu - Do NOT map the directional controls (Forward, Backward, Left, Right), as this will overwrite certain changes made in the Oblivion.ini file.

These are the default settings in the Oblivion.ini:
;X = 1, Y = 2, Z = 3, XRot = 4, YRot = 5, ZRot = 6

iJoystickMoveFrontBack=2
iJoystickMoveLeftRight=1
fJoystickMoveFBMult=1.0000
fJoystickMoveLRMult=1.0000
iJoystickLookUpDown=6
iJoystickLookLeftRight=3
fJoystickLookUDMult=0.0020
fJoystickLookLRMult=0.0020

Change to these values to get better functionality from a 360 game pad connected to a PC.
;X = 1, Y = 2, Z = 3, XRot = 4, YRot = 5, ZRot = 6
iJoystickMoveFrontBack=2
iJoystickMoveLeftRight=1
fJoystickMoveFBMult=2.0000
fJoystickMoveLRMult=2.0000
iJoystickLookUpDown=5
iJoystickLookLeftRight=4
fJoystickLookUDMult=0.7500
fJoystickLookLRMult=0.7500

Make sure the settings are saved. Note, changes to the Oblivion.ini file will not be saved if Oblivion is running when the changes are made.

-Updated Oblivion Launcher
The updated launcher now includes options for changing your auto detect settings for Video Quality. The presents are Very Low, Low, Medium, High and Ultra High. If you select Reset to Defaults, it will restart the auto detect and offer the best settings for your system.


*****************************************
     2. Manual Errata and Addendum
*****************************************


-New Quick Keys. Press F1 - F4 to access your Journal and Stats menu

	F1 - Stats 

	F2 - Inventory Menu

	F3 - Magic Menu

	F4 - Maps and Quests

-Page 20 states the Governing Attribute for Block is Agility. It should be Endurance.


*****************************************
     3. Performance Tuning
*****************************************


There are several things you can do to increase game performance.

-Make sure you have no other programs running in the background.

-Lower the game resolution. The game runs faster at 640x480 and 800x600.

-Go to your Options menu and select Video. Try the following options to improve performance:
	-Set View Distance as low as possible. Your framerate and load times will improve but you will not be able to view as far.

	-Set Tree, Actor, Item and Object Fade as low as possible. This will cause certain objects in the world to fade away sooner.  This will increase your framerate but degrade visual quality.

	-Set Texture Size to Medium or Small. Textures on objects will not appear as sharp when this setting is reduced.  This will increase your framerate but degrade visual quality.

	-Set Grass slider as low as possible. This will cause less grass to be displayed around your character.  This will increase your framerate but you will see less grass displayed.

	-Set Distant LOD to OFF. This will reduce your view distance, but your framerate and load times will improve.

	-Set Distant Buildings to OFF. You will not see cities or the Imperial City in the distant landscape but your framerate and load times will improve.

	-Set Distant Trees to OFF. You will not see trees in the distant landscape but your framerate and load times will improve.

	-Set Interior Shadows as low as possible. This will decrease the number of characters that cast shadows while you are in interiors, improving your framerate.

	-Set Exterior Shadows as low as possible. This will decrease the number of characters that cast shadows while you are in exteriors, improving your framerate. 

	-Set Self Shadows to OFF. The Player and other characters will no longer cast shadows on themselves, but will still cast shadows on the environment.  This will improve your framerate.

	-Set Grass Shadows to OFF. Shadows will no longer display on grass. This will improve your framerate.

	-Set Tree Canopy Shadows to OFF. The forests will no longer cast shadows on the landscape, improving your framerate.

	-Set Shadow Filtering as low as possible or off.  This will reduce the amount of softening the shadows receive, but increase framerate.

	-Set Specular Light as low as possible. This will cause objects to lose their shininess at lower distances, improving your framerate.

	-Set HDR Lighting to OFF. This will increase your framerate but degrade visual quality.

	-Use Bloom lighting instead of HDR, or turn Bloom off.  Bloom is a less intensive version of HDR.  Turning it off will improve framerate but degrade visual quality.

	-Make sure Water Detail is set to Normal. High detail water will decrease your framerate.

	-Set Water Reflections and Ripples to OFF. This will increase your framerate while you are near water, but the water will not show reflections or react to objects interacting with it.

	-Set Window Reflections to Off.  This will remove the subtle reflections from windows but improve framerate.	

	-Set Blood Decals to Medium or Low. At Medium, decals do not get applied to characters, only landscape.  At Low, no decals get applied at all.  These will increase your framerate in combat situations.

	-Turn anti-aliasing down or off.  This will degrade overall visual quality but improve your framerate.

	-Turn off music
	The music is mp3 format and can slow the game down.

*****************************************
     4. System Requirements
*****************************************


-Minimum System Requirements:
* Windows XP
* 512MB System RAM
* 2 Ghz Intel Pentium 4 or equivalent processor
* 8x DVD-ROM Drive
* 4.6 GB free hard disk space
* DirectX 9.0c (included)
* 128MB Direct3D Compatible Video card and DirectX 9.0 compatible driver
* DirectX 8.1 Compatible Sound Card
* Keyboard, Mouse

-Recommended System Requirements:
* 3.0 Ghz Intel Pentium 4 or equivalent processor
* 1 GB System RAM
* ATI X800 series, Nvidia GeForce 6800 series, or higher video card

-Supported Video Card Chipsets:
ATI X1900 series
ATI X1800 series
ATI X1600 series
ATI X1300 series
ATI X850 series
ATI x800 series
ATI x700 series
ATI x600 series
ATI Radeon 9800 series
ATI Radeon 9700 series
ATI Radeon 9600 series
ATI Radeon 9500 series
NVIDIA Geforce 7800 series
NVIDIA GeForce 6800 series
NVIDIA GeForce 6600 series
NVIDIA GeForce 6200 series
NVIDIA GeForce FX series


VIDEO
-Regardless of your video card, make sure to download the latest drivers from your manufacturer.

INPUT
-ALT+TAB may cause some game instability with some hardware configurations and is not advised.


*****************************************
     5. Update 1.2.0416 Notes
*****************************************

Bug Fixes
*****************************************
Fixed a crash caused by bad form IDs

Fixes an issue where the game would try to use a form IDs that was either restricted or not available yet.

Fixed an issue where form IDs were not being marked as free properly, causing objects to disappear in game.





*****************************************
     6. Update 1.2.0214 Notes
*****************************************

Bug Fixes
*****************************************
Improved LOD visual quality for landscape.

Optimizations to file loading system.

Taking items from dead owned creatures is no longer a crime.

Fixed issue where lock/unlocked states on doors would occasionally be stored incorrectly in a save game.

NPCs no longer pop into view after player cancels out from the Wait menu.

Fixed memory leak with sitting in a chair multiple times.

The reflection from the environment map in windows now displays properly.

Fixed an issue where player is still in combat even though the creature is no longer present.

Player can no longer fast travel when paralyzed.

Fixed infinite dialogue loop when arrested by guards who have high disposition to you.

Fixed issue where guards would not properly report crime if they were pickpocketed.

Summoned creatures properly fade away when they are created from a leveled list.

Fixed issue where stolen items would lose their stolen status if the player character was female.

Fixed crash that would occur with NPCs loading in with arrows.

Pickup sound effects no longer play during the loading screen.

If you attack a creature owned by you, crime is no longer reported.

Fixed issue with LOD not loading in properly when entering/exiting worldspaces.

Fixed infinite soul gems exploit by dropping and picking up stacked soul gems.

Fixed a crash with summoning a creature and immediately exiting the cell.

Fixed a crash with stealing an object, exiting and immediately re-entering an interior.

Fixed issue where an NPC would occasionally not perform the proper idle animation.

Fixed an occasional crash when a creature loses detection on the player.

Fixed an occasional crash with NPCs who were not loaded going into combat.


Quest Fixes
*****************************************
In Light the Dragonfires, fixed issue where improper journal would appear if you closed an Oblivion gate.

In Till Death do They Part, fixed an issue where Melisande would not properly give you Cure Vampirism potion.


*****************************************
     7. Update 1.1 Notes
*****************************************


Bug Fixes
*****************************************

Fixed an issue with falling through collision in Fort Wooden Hand.

Fixed issue with remapping controls in French, German, Italian and Spanish versions.

Fixed issue with some shadows not lining up.

Going to jail while equipped with bound armor or weapons no longer crashes the game.

Fixed issue with bound weapons not dispelling properly after dismounting a horse.

Fixed issue with player shadow being delayed after fast travel.

Fixed infinite gold issue on some dead NPCs.

Fixed issue with disease resistences that made it impossible to contract vampirism under certain circumstances.

Fixed an issue where occasionally skills would not increase properly after you received an increase in a way other than skill uses like as a quest reward.

Fixed issue where spells, powers and lesser powers were being improperly resisted when the player cast them on themselves.

Fixed an issue where creatures and NPCs would not go into combat properly after being hit by a projectile.

Fixed an issue with duplicating items and unequiping the bow.

Fixed an exploit that allowed you to sell equipped items to a vendor more than once while on a horse.

Fixed an issue with items reappearing in dead bodies after saving and reloading.

Fixed crash when NPC with active light spell on them unloaded from memory.

New Very Low Quality graphic setting available under Launcher options with improved support for low end FX cards (5700 and lower). To use this setting, go to the Launcher, select Options and click Reset to Defaults to allow the auto detect to check your system.

Implemented SLI-mode optimizations on Nvidia cards, and Crossfire optimizations for ATI cards.

Fixed a crash issue where loading a save would crash if the player had extra data on them.

Fixed an issue for LOD art for city was not unloading quickly enough when exiting an interior.

Fixed an issue where Aylied doors would not open when activated in Miscarcand. 


Quest Fixes
*****************************************

If you are permanently expelled from Mages Guild, you can now go back into the Mages Guild buildings.

In The Siren's Deception, the door to Gweden farmhouse is prevented from locking too soon if player exits too quickly.

In the Light the Dragonfires quest, player controls are prevented from being locked if player accidentally hits Ocato during the final battle in the Imperial Palace.

In the Confront the King quest, fixed an issue where Mannimarco would occasionally stop fighting the player while the player's controls are locked.

In Corruption and Conscience, fixed an issue if player got to Llevana's house earlier than expected and she would initiate trespass behavior rather than move the quest forward.

In Theranis' Mistake, it is no longer possible to get multiple copies of Ahdarji's ring. Also, fixed an issue with player receiving Blood Price topic too early in the quest.

In the Leyawiin Recommendation quest, it is no longer possible to bypass Kalthar in Fort Blueblood.

In Revenge Served Cold, Corrick will now recognize when player had the jade amulet in their inventory if No Stone Unturned quest had been previously completed.

In Infiltration, player can no longer kill Blackwood Company members and stop progress in Fighter's Guild.

In Dark Brotherhood, if you kill fellow members and get kicked out of the guild, you can no longer continue to progress in the questline until you redeem yourself and get back in.

In The Master's Son, the player now properly receives their reward when completing the quest.

In Caught in the Hunt, fixed an issue where NPCs would not go into combat properly.

In the Cheydinhal Recommendation quest, fixed an issue where Vidkun's body would disappear if you left the well. 

Getting disqualified from the first Arena match no longer blocks you from further matches.

In Till Death Do They Part, the Count no longer rewards player with gold more than once. Fixed an issue with not receiving the Vampire Ashes topic if the player picked up vampire ashes before getting the quest. Fixed issue where Bloodgrass topic was not added if player finished the Main Quest before starting quest. Hal-Liurz will now follow player properly when asked about the cure.

In Mystery and Harlun's Watch, the dead body you are supposed to find will no longer disappear from Swampy Cave if you cleared out the dungeon before starting the quest.

In Blood of the Daedra, Martin will now recognize Spellbreaker as a Daedric artifact.

In When the Vow Breaks, additional instance of Rockshatter are now prevented from appearing on Bjalfi's dead corpse after saving and reloading.

In Paranoia, game no longer crashes when Bernadette Peneles exits the city while you are following her.

For Clavicus Vile quest, fixed crash with giving or refusing to give Umbra to Clavicus Vile.



Plugin Fixes
*****************************************

Fixed issue with saving your game while an actor is in a new interior cell created in a plugin, and re-loading the save game without the plugin.

Fixed issue with loading previous saves with plugin that contains new base objects that are containers, NPCs and creatures.

Fixed issue with linked pathpoints scripted to switch on/off that are modified by a plugin.

NPC's companions no longer disappear when they fast travel with player to an exterior cell that is modified by a plugin.

New scripted spell effects created in a plugin now work properly. 