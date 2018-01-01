---
title: Changelog | H-Ext
keywords: [changelog]
summary: "H-Ext changelog info"
sidebar: h-ext_sidebar
permalink: /h-ext/changelog.html
folder: h-ext
---

## October 20th, 2014 - November 10th, 2014

* Update to 0.5.2.4
* Fixed: UAC Virtualization cause issues with forced redirect directory without telling the application where it's really stored at.
* Changed: Changed the fresh setup method at load.

## May 30th, 2014 - September 20th, 2014

* Update to 0.5.2.3
* Task List: ticket 23 (See ticket for complete info)
* Added: isfloatA/W, isdoubleA/W functions added to util namespace. **NOTICE: This require an updated Add-on API.lib file for H-Ext 0.5.2.3 and newer.**
* Added: EXTOnPlayerUpdate hook
* Added: EXTOnMapReset hook, only supported for Halo PC & CE version. Halo Trial does not have this. **NOTICE: This does not hook to a "successfully reset" section, it only tells sv_map_reset has been executed.**
* Changed: EXTOnPlayerAttemptDropObject hook, was *EXTOnPlayerDropObject*
* Fixed: Rcon message for client console does not appear. (Added another detection if player is local or remote.)
* Changed: Timer ticks changed 60 ticks to 30 ticks per second (using map ticks instead of game ticks) and excluded the requirement of needed to include map ticks.
* Previous checking for halo, and Open Sauce, commands were not 100% accurately due to limitation on commands matched. Now it fully include every commands.
 * **NOTICE: You will need to manually re-fix your commands.ini file! Please remove ANY of the non-characters such as +, -, <, =, etc under "[Halo]" section!**
* Fixed: Halo's alias commands aren't 100% successful due to executing the alias instead of full command name.
* Fixed: Any non-characters excluding underline, dot, and numeric cause issue for iniFile class to insert fake section wrongful.
* Changed: Since noticeable for some hosting company could not restart due to quietly crash internally. By default it will not quietly crash. However, you can use a command to force quietly crash enable.
* Fixed: Login command through rcon cause crash.
* Fixed: First login success then cause second and on not to work due to overwriting other variables. **NOTICE: This is a serious affect of how H-Ext handle the players!**
* Fixed: Login through chat displayed the sensitive login info.
* Fixed: dynamicStack class of copying has one minor misused variable. **NOTICE: This has a serious affect of how H-Ext and addons operate the ICIniFile class!**

## January 10th, 2014 - May 29th, 2014

* Update to 0.5.2.2
* Updated to support Halo 1.0.10 (Only few signatures was not compatible with Halo 1.0.10)
* Task List: ticket 23 (See ticket for complete info)
* Added Timer class
* Fixed util::StrToTeam and IPlayer::StrToPlayerList for blue/red team always selected blue team.
* Fixed duplicated halo commands. **NOTICE: This only occur at initialize of H-Ext, any changes afterward will re-appear. Please unload and reload the H-Ext to resolve the duplicated halo commands.**
* Updated to Add-on 3.1.1
 * Fixed dynamicStack class
 * Fixed IObject class
 * Changed standard command parameters
 * Changed versioning method into more easier to setup.
* Added ? new hooks: (Cannot remember what was the new hooks for halo...)
* Released AdvObject Add-on

## December 3rd, 2013 - January 9th, 2014

* Update to 0.5.1.2
* Task List: ticket 23 (See ticket for complete info)
* Fixed major crashes for new setup and/or new users.
* Updated to Add-on 3.1
 * Big changes to the individual class functions export into one simple interface wrapper export to reduce the number of exports. (More easier to handle plus ability to support current and new additions.)
* Added 4 new hooks:
 * EXTOnEquipmentDropCurrent
 * EXTOnVehicleAIEntry
 * EXTOnMapLoad
 * EXTOnServerStatus (Only relative to dedicated server status repeats.)

## November 22nd - December 2nd, 2013

* Update to 0.5.0.2
* Fixed non-existed player as administrator cause crash.
* Fixed broken query for addding CD Hash into admins table.
* Fixed banlist query.
* Updated all database querys to work *as* expected to be.
* Verified to work with latest add-ons release (v1.0.0.1).

## November 8th - November 9th, 2013

* Update to 0.5.0.1
* Hotfix bug #26
* Hotfix dynamicStack from Add-on API's SDK.

## Feburary 24th 2013 - November 2nd, 2013

* Upgrade to 0.5.0.0
* Changed from standalone (secondary executable, EXE) into integration (module, DLL)
* Task List: ticket #19 (See ticket for complete info)
* Fixed bug #20
* ticket #21


## October 22nd - November 11th, 2012

* Updated to 0.4.2.2
* Some minor fixes overall relative to duplicate cd keys in server.
* Lost log for this update

## October 4th - October 21st, 2012

* Updated to 0.4.2.1
* Improved feature ticket #16
* Fixed bug #18
* Added working stats box (except for public detection)
* Added right-clicking support.
* Added tab key listener to search list of commands.
* Added missing "me" part of player_expression system.

## August 12 - October 3rd, 2012

* Updated to 0.4.1.1
* Add-on API updated to 2.1 .
* Added feature ticket #15
* Fixed unloading 2 or more loaded plugins.
* Compatible with Official Updater.

## April 26th - August 11th, 2012
* Upgraded to 0.4.0
* Add-on API updated to 2.0 .
* Major changes, see
 * ticket #3
 * ticket #4
 * ticket #5
 * ticket #6
 * ticket #7
 * ticket #9
* Added feature ticket #13
* Added/Improved feature ticket #8
* Fixed bug #1
* Fixed bug #2
* Fixed bug #10
* Fixed bug #11
* Fixed bug #12
* Fixed bug #14

## April 15th - April 25th, 2012
* Updated to 0.3.2.3
* Add-on API updated to 1.2 .
* Added Duplicated CD Key hash check disable/enable.
* Added GameSpy CD Key hash check disable/enable.
* Added Halo Client Version check disable/enable.
* Added Halo Server Version change disable/enable.
* Lost log for this update

## April 6th - April 14th, 2012
* Updated to 0.3.1.3
* Lost the log for this update

## March 16th - April 5th, 2012
* Updated to 0.3.1.2
* Lost the log for this update.

## January 27th - March 15th, 2012
* Updated to 0.3.1.1
* Add-on API updated to 1.1 .
* Updated biped.h, message.h, player.h, servercontrol.h, vehicle.h, weapon.h headers.
* Added machine.h header.
* Fixed Windows XP's UTF-8 format incompatibility. **(NOTICE: you must manually set the console's to Lucida Console by default for best viewing! This will be replaced in 0.4.0 and higher with GUI window(s).)**
* Fixed Windows XP's bug with empty parameter(s).
* Added UpdateObject function for force sync to clients.
* Added grenade commands for players.
* Re-modified the console's command executed and detect rcon players.
* Added ability to change unlimited level for admins instead of always 21.
* Added support to response back to rcon player.
* Added names, ips, and ports into new history system for logging per CD hash. (Limited per command is 20,000 which is total of 60,0000 per CD Hash.)
* Updated powerups, vehicles, weapons, and warthog to spawn directly to whom executed the command.
* Added /c command from original devicator's usage back to life. **(NOTICE: This is official beta command!)**
* Renamed "It's quite bit too quiet in here tbh..." to "It's too quiet in here tbh..." for killall function.
* Updated ammo, empty ammp, give ammo, take ammo, health, shield, shieldmax, healthmax, invinc, uninvinc, speed, freeze commands to display onto individual clients.
* Added list of alias commands for full function name.
* Added Upgrade system detection for database. (Required for new history system migrate into older database automatically.)

## December ?, 2011 - January 26th 2012
* Upgraded to 0.3.0 (major re-written, better standardize, add plugin support, and more C native language interaction level)
* Re-named the functions to formal command names and better understanding.
* Added plugin support. NOTICE: We do NOT post plugin updates here!  We have not determined where to have them posted yet.
* Added Add-on API 1.0 .
* Added Database API.
* Added default team when join. (MIGHT be already included in 0.2.2, unsure...)
* Added enable/disable team change (globally for now). (MIGHT be already included in 0.2.2, unsure...)
* Rewritten and improved database stability to 95 percentage.
* Fixed player's index from quit event due to offset is off by one from sync.
* Fixed map check loop due to case sensitive name check up.
* Fixed sv_ban and improved little bit.
* Fixed sv_password and more improved compatibilities usage.
* Added few additional features.
* Plus other improvements/fixes forgotten.

## November ? - November ?, 2011
* Updated to 0.2.2
* Added me command similar to xfire and minecraft's, could be more game servers using me commands.
* Added whisper to player support.
* Lost information except there are major additional features and improvements into it.

## October 18th - November 4th, 2011
* Updated to 0.2.1
* Fixed map detection for sv_map command.
* Fixed administrator restriction system.
* Added new administrator system and continue support using this new system.
* Added console display chat without required to log.
* Added shield command by request (Buggy and not effective due to unable sync to client for some reason.)
* Added support to hold up to 5 commands to holding list.
* Plus other improvements/fixes forgotten

## August 1st - October 15th, 2011
* Upgraded to 0.2.0 (major transfer from .dll to most focused .exe and required most changes/fixes compatibility for .exe support)
* Renamed from DZS SAPP to DZS Server Extension.
* Added working chatblock/chatban system.
* support chat command from global to vehicle chat.
* First time add AdminBot system **NEW FEATURE**
* log support for extension console.
* Added Vehicle Protection **NEW FEATURE**
* Added Internal Database support **NOTICE: Is compatible with Rec0's database but does not support administrator system**
* Removed dirty file support
* Removed MySQL support for time being as it is considered as a plugin feature.
* Plus other improvements/fixes forgotten

## July 11th - 23th, 2011
* Updated to 0.1.4 Beta Release (major improvements than previous versions)
* Fixed to have ability unload safely without crash. **(NOT RECOMMENDED TO UNLOAD ANY OLDER VERSION OF 0.1.3 AND BELOW!)**
* Fixed identical unit_kill command from SAPP's commands with exception-proof.
* Fixed the reversed indexes since few has stayed and pointed out my errors along with exception-proof to maintain server running.
* Add more commands and enhancements.
* Plus possible other improvements/fixes forgotten.

## July 8th - 9th, 2011
* Update to 0.1.3 Beta Release
* Added support for player-in-vehicle teleport
* Support to flip player-in-vehicle
* Added AFK (in draft but is supported) and set re-spawn time
* Re-construct the reversed index of players compatible.

## July 4th - 7th, 2011
* Updated to 0.1.2 Beta Release
* Added cheat commands with shortcuts identical to Rec0's
* Possible fixed team switch and kill commands
* Cured the commands relative to server message from sapp to different location
* Plus couple other issues

## June 31st - July 3rd, 2011
* Update to 0.1.1 Beta Release
* Migrated options support for safe toggle, server message toggle, and limit length.
* Re-re-fixed database freezing the server (100% sure this time)
* May or may not able to remove the query's thread (not 100% confirmed yet and unable to test it out)

## June 27th - 30th, 2011
* Set as 0.1.0 Beta Release
* Updated to 0.0.11
* Re-fixed the database's query (which is the cause) to set the timeout to avoid any more freezing the server.

## June 26th, 2011
* updated 0.0.10
* fixed and improved vehicle eject and teleport with better message.
* fixed the "Error" popup coming from player events system by capture the error and re-execute it to resume.
* Forgot what else...
* Next release should fix the frozen connection between database and server.

## June 18th - 26th, 2011
* Updated 0.0.9 Alpha
* Added external database support for commands, locations, and players.
* Fixed vehicle ejection
* Fixed player list ID number
* Fixed kick, kill, etc. to correct player.

## June 12th - 14th, 2011
* Updated to 0.0.8
* Fixed the sv_map command OUTSIDE of the thread.
* Partial fixed the kill and team switch (possible in 0.0.9 version will fix it by then)
* Fixed most of the commands that cause an error(s) while game still running.
* Maybe some others forgotten to be included here.

## June 8th - 11th, 2011
* Updated to 0.0.7 (third update of this version)
* Successfully detect the locations if is already on the list or not completely.
* Finally fixed the higher number on coordinates to complete number instead of scientific number.
* Set the decimal to 2 instead of randomly range from 0 - infinity inside decimal field.
* Added player's location teleportation system to teleport's function. (Make it easier to teleport players to one specific player.)
* Possible remove the exception from using the kill command from both kill and team switch function.
* Same as above but does the same with other relative "unit" devmode function possible exception as well.

## June 5 - 7th, 2011
* Updated to 0.0.6 (Now proves to be no crashing at all)
* Now included message for lag and unlag a player.
* Major replacement to keep the execution much safer level. (This may be the possible issue solved)
* Added two additional exception capture for console/rcon and chat commands. (May also be another possible issue solved)
* Fixed the "/" and "\" without saying the admin isn't on admin level.
* Added unauthorized non-admin message if attempted to use chat command.

## May 29th - 30th, 2011
* Update to 0.0.5
* Appended the rcon AND console execution into a new stable thread along with chat commands (chat commands stability were fixed in 0.0.4)

## May 25th - 28th, 2011
* Updated to 0.0.4
* Temporary fixed the ammo crash when a player is in the vehicle. (Fixed in 0.0.3 RC2)
* Added more server message for almost all additional commands.
* Added support for command loop for player matched to player list without needing to crash the server when have more than 6-8 players.

## May 24th, 2011
* Update to 0.0.3 RC1
* Major fixed for teleport system
* Major fixed the player expression system to match from the list
* Added team into player expression system
* Possible to capture the exception before it crash the server (hopefully)

## May 22th, 2011
* Updated to version 0.0.2
* Added About
* Fixed wrong address position
* Teleporting works properly

## May 17th, 2011
* Initial version 0.0.1
* Currently support the latest 1.09CE version and still support 1.08CE version. (Previously only support on 1.08CE version)

## May 15th, 2011
* Fixed adding the teleport locations properly
* Added remove teleport location

## May 14th 2011
* Fixed Admin levels permission to recognize if allowed or deny to execute the command
* Added few additional features (will be display later)

## May 9th - 13th 2011
* Fixed major bugs
* Added some additional features (will be display later)

## May 8th 2011
* Start working on out-of-date open source sapp from the Internet.

{% include links.html %}
