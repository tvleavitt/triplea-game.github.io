---
layout: page
title: Release Notes
permalink: /release_notes/
---

<div class=".release-notes">

<h3>Changes for 1.8.0.11</h3>
<ul>

  <li>- Minimum Java version is now Java 1.8</li>

  <li>- Removing all "Grid" games (Chess, Checkers, Go, Kings Table) as well as inaccessible puzzle games (N-Puzzle and Tic-Tac-Toe). (veqryn)</li>

  <li>- Performance improvement for bot servers to reduce CPU usage when hosting games, PR#53. (lafayette)</li>

  <li>- Performance improvement that allows games to start more quickly, background map parsing is halted when a game is launched, PR#74 (lafayette)</li>

  <li>- PNG files made 17MB smaller with lossless compression 'optipng', PR#146 (lafayette)</li>

  <li>- Install4j now used to create installer packages, PR#218 (gaborbernat)</li>

  <li>- Installer packages automatically deployed to github whenever code is merged, PR#261 (lafayette)</li>

  <li>- Performance improvement to speed up map parsing time, read only the game XML data and do not read the entire Zip file from disk. This speeds up map parsing to be typically under 100ms when before it could be a few seconds for largers maps. (lafayette)</li>

  <li>- Add support for to play mp3 audio files in addition to wav files. PR#201 (lafayette)</li>

  <li>- Bugfix - 'delete corrupt map' game crash when the confirmation dialog window was shown. PR#304 (lafayette)</li>

  <li>- Map parsing performance improvement, some maps with long territory lists will now loader faster. PR#293 (lafayette)</li>

  <li>- Code improvement - Unit test runtime reduced from 31s to 21s. PR#115 (lafayette)</li>

  <li>- Map parsing improvement - map zip data is read more efficiently, map data is loaded 10x faster. PR #240 (lafayette)</li>

  <li>- Undo unit moves with 'u' key - PR#253</li>

  <li>- AI - Added check for whether factories can be placed to purchase  #270 (redrum)</li>

  <li>- AI - consider enemy turn order  #282 (redrum)</li>

  <li>- AI - consider multi-nation attacks  (redrum)</li>

  <li>- Github Map Downloads #286</li>

  <li>- Map parsing performance improvement #293</li>

  <li>- AI - Add capital value for amphib attacks  #316</li>

  <li>- Add a 'clear' button to the error console.  #332</li>

  <li>- Add performance debug console   #333, #335 </li>

  <li>- Updated canals to check if at least 1 is passable instead of all if  #343 (redrum)</li>

  <li>- New Install4j Installers  #372  (gaborbernat)</li>

  <li>- AI - Add new Fast AI player #379</li>

  <li>- Ai remove strong ai  #394</li>

  <li>- Add total units in territory count to TerritoryPanel  #399</li>

  <li>- Show Engine Version on the UI + Consolidate Engine Version and Game Configuration  #426</li>

  <li>- AI - Update casualty selection unit value calculation to consider  #447</li>

  <li>- Map Download Overhaul - Tabbed View with Progress Bars and additional features  #449</li>

  <li>- Improve Planes Can Not Land Warning  #476</li>

  <li>- Remove Delay on the Startup Map and Engine Version Checks - #470</li>

  <li>- Default Politics Action is No - #497</li>


</ul>

<h3>Changes for 1.8.0.9</h3><ul>
  <li>- Bug fix, retreat from naval combat was not possible, now fixed. (redrum)</li>

  <li>- Fixed possible infinite loop bug when a corrupt map exists in the map downloads, PR#76. (lafayette)</li>

  <li>- Increase scroll speed when using arrow keys. Holding down control speeds up arrow key scroll. (lafayette)</li>

  <li>- Placing cursor next to the very edge of the map increases scroll speed. (lafayette)</li>

  <li>- Hard AI - Fixed calculating defenses on maps with air/naval bases to properly calculate enemy range. (redrum)</li>

  <li>- Hard AI - Fixed bug around not defending against enemy units that were transported the previous turn as they were being marked as already transported when potential enemy attacks were calculated. (redrum)</li>



</ul><h3>Changes for 1.8.0.7</h3><ul>
  <li>- Hard AI - Improved performance on large maps. (redrum)</li>

  <li>- Hard AI - Added support for valuing exposed units when attacking. (redrum)</li>

  <li>- Hard AI - Improved air units landing safely. (redrum)</li>

  <li>- Hard AI - Added scrambling support. (redrum)</li>

  <li>- Hard AI - Improved transport movement and defense. (redrum)</li>

  <li>- Hard AI - Added support for purchasing and landing on carriers. (redrum)</li>

  <li>- Hard AI - Improved naval non-combat move and avoid sea units getting stuck. (redrum)</li>

  <li>- Hard AI - Improved casualty selection to consider unit cost. (redrum)</li>

  <li>- Hard AI - Added unit support attachment consideration for purchasing and movement. (redrum)</li>

  <li>- Hard AI - Added politics support for 2 team maps such as Global 1940. (redrum)</li>

  <li>- Hard AI - Improved capital defense. (redrum)</li>

  <li>- Hard AI - Added support for WW2v1 non-limit placing of units. (redrum)</li>

  <li>- Hard AI - Added support for territory effects. (redrum)</li>

  <li>- Hard AI - Added support for China on WW2v3. (redrum)</li>

  <li>- Hard AI - Added support for unit placement limits. (redrum)</li>

  <li>- Hard AI - Fixed sorting bug causing error: Comparison method violates its general contract. (redrum)</li>

  <li>- Hard AI - Improved carrier/fighter casualty sorting to avoid leaving fighters stranded. (redrum)</li>

  <li>- Hard AI - Units of the same type are now moved all at once rather than one at a time. (redrum)</li>

  <li>- Hard AI - Fixed several rare NullPointerException errors. (redrum)</li>

  <li>- Hard AI - Added support for nations without capitals. (redrum)</li>

  <li>- Source code migrated to github - http://github.com/triplea-game/triplea (veqryn)</li>

  <li>- Fixed maxBuilt to include unplaced units, PR#62. (LaFayette)</li>

  <li>- Added a convenience button to undo all moves during a phase, PR#61. (LaFayette)</li>

  <li>- Removed obsolete Dynamix (land-only) AI. (veqryn)</li>

  <li>- Fixed issue with TripleA logging users out of axisandallies.org when posting turns. (redrum)</li>

  <li>- Fixed bug with movement validation for fighters launching from a carrier and flying into enemy land territory then returning. (veqryn)</li>

  <li>- Bug fixes on unit casualty sorters, and switching approximate method in as the default. (veqryn)</li>

  <li>- Created a new prototype unit sorter for quicker approximate sorting, including support attachments. (redrum)</li>


</ul><h3>Changes for 1.8.0.5</h3><ul>
  <li>- Created a prototype unit sorter for sorting units with support attachments (still in beta) and added it as an option in engine preferences. (veqryn & redrum)</li>

  <li>- Updating Substance/Insubstantial look and feel UI to version 7.3. (veqryn)</li>

  <li>- Fixed bug with how AA casualties are taken for multiple-hitpoint airplanes. (veqryn)</li>

  <li>- Fixed null pointer error in Classic (WW2v1) rockets. (veqryn)</li>

  <li>- Speeding up battle calculator by reducing possibilities of thread contention over locks. (veqryn) </li>

  <li>- Fixed bugs in Fuel cost for units, including around loading and unloading, and moving air with carriers. (veqryn)</li>

  <li>- More stability improvements for server games. (veqryn)</li>

  <li>- Fixed a thread deadlock that occurs when a game ends while the battle calc is still open, resulting in triplea not returning to the host screen. (veqryn)</li>

  <li>- Prevented battle calc's calculate button from being enabled until data has finished being copied. Also added a tool tip on the button to let the user know how much memory they have left. (veqryn)</li>

  <li>- Fixed display issue with repairs not being recorded properly in history panel. (veqryn)</li>

  <li>- Fixed memory leak in battle calc and game data, causing an exponential number of units to be added to saves. (veqryn)</li>

  <li>- Fixed bug in bid placement where you could not play British units in UK Pacific territories in Global 1940/1942. (veqryn)</li>

  <li>- Changing default host waiting time to 900 seconds (15 minutes) so that large games do not time out on people who don't know how to change the setting. (veqryn)</li>

  <li>- Massive improvements to the new Hard AI. (redrum)</li>

  <li>- Fixed lag and synchronization issues in the multi-threaded battle calc. Also added methods to time how long it takes to copy the game data, and use fewer threads if this takes more than 5 seconds. (veqryn)</li>

  <li>- Fixed possible deserialization error in resource collections. (veqryn)</li>

  <li>- Fixed bug in movement performer, which under certain rare circumstances would take all movement away from air units going from sea to land. (veqryn)</li>

  <li>- Further work on ProAI (called Hard AI in game menu), including new methods to determine retreats in battles. (redrum)</li>

  <li>- Fixed bug in username muting, which caused it to not work at all. (veqryn)</li>

  <li>- Fixed issue with the game waiting on a player to click all 'OK' messages before a battle would continue. (veqryn)</li>

  <li>- Fixed MapCreator so that it will properly send the map folder to the utility programs. (veqryn)</li>

  <li>- Adding options to engine preferences to change how long your game host waits for clients on game startup and for observers joining. (veqryn)</li>

  <li>- Allowing host to wait up to 100 seconds when starting a game for all clients to report in as good, and wait up to 30 seconds for observers joining after game has started. (veqryn) </li>

  <li>- Fixing two memory leaks that allowed AI's and GameData to stay in memory after exiting back to main screen. (veqryn)</li>

  <li>- Creating a threaded version of the BattleCalculator, to speed up results. (redrum & veqryn)</li>

  <li>- Creating a logging window for ProAI so that players can watch the log. (redrum)</li>


</ul><h3>Changes for 1.8.0.3</h3><ul>
  <li>- Created new step property option, "repairPlayers", which will allow a player to repair the units owned by a different player. (veqryn)</li>

  <li>- Fixed issue where your move phase was skipped if the only unit you owned was a land unit in a transport. (veqryn)</li>

  <li>- Allowing land units to receive repairing and bonus movement from neighboring sea zone sea units. (veqryn)</li>

  <li>- Units on transports no longer are able to repair other units, allow scrambling, or give movement to other units. (veqryn)</li>

  <li>- Fixed issue where a unit that dies from rockets, still participates in subsequent strategic bombing battle. (veqryn)</li>

  <li>- Fixed issue with allied land units in friendly transports and allied air on friendly carriers losing their movement when their transport/carrier moved. (veqryn)</li>

  <li>- Fixing issue with allied land units starting game loaded on friendly transports, could not offload until at least one non-combat phase had passed. (veqryn)</li>

  <li>- Deleted global game option property, "Allied Air Dependents", and replaced with its inverse, "Allied Air Independent". (veqryn)</li>

  <li>- Added menu option under 'Export" menu, called "Export Unit Charts", which will create an html document showing all units in the game and their properties and cost. (veqryn)</li>

  <li>- Created an new menu option under the 'Help' menu called "Unit Help", which will display a table of all units, by player, including all unit properties. (veqryn)</li>

  <li>- Fixed bug in relationship attachment property change by trigger. (veqryn)</li>

  <li>- Deleting phase step property option, "resetUnitState", and replacing with "resetUnitStateAtEnd" and "resetUnitStateAtStart". (frogg)</li>

  <li>- Making createsUnitsList ability choose a random territory when producing to a neighboring territory. (veqryn)</li>

  <li>- Fixing bugs in AI's where factories were on water zones that had no territory attachment. (veqryn)</li>

  <li>- Fixed bug where a stalemate battle with carriers that can be damaged and when damaged don't let planes land, were not letting defending planes move to land. (veqryn)</li>

  <li>- Deleting game option property "Unescorted Transport Dies", as it no longer does anything. (veqryn)</li>

  <li>- Cleanup of HeadlessGameServer classes. (veqryn)</li>

  <li>- Fixed bugs in Placement, which were allowing infinite placement of sea units which were constructions. (veqryn)</li>

  <li>- Some updates for 'Great War' world war 1 map, and Pact of Steel 2. (veqryn)</li>

  <li>- Possible fix for "Could not stop delegate execution" bug. (veqryn)</li>

  <li>- Fixed possible bug where a corrupted game save had the initialization delegate get called more than once. (veqryn)</li>

  <li>- Adding a new AI called "Hard AI". Also renamed AI's: EZ Fodder -> Easy AI, Moore N Able -> Medium AI, Dynamix -> Land Only AI. (redrum)</li>

  <li>- Fix for infinite crash-reload loop on loading a corrupt autosave on a host bot. (veqryn)</li>

  <li>- Fixed issue with Victory trigger not being able to use html properly. (veqryn)</li>

  <li>- Fixed illegal state exception error in landing paratroopers during a battle. (veqryn)</li>

  <li>- Possibly final fix for a game hang / frozen bot on game launch. (veqryn)</li>


</ul><h3>Changes for 1.8.0.1</h3><ul>
  <li>- Adding new sci-fi sound for "future" era. (pulicat, cernel, veqryn)</li>

  <li>- Allowing "NONE" as a valid option value in sounds.properties file. (veqryn)</li>

  <li>- Fixed null pointer exception in Moore AI for water based factories. (veqryn)</li>

  <li>- Fixed bid delegate so that it will still run even if the player has no resources other than the bid amount. (veqryn)</li>

  <li>- Fixed possible null pointer exception in Triggered Victory which is triggered from outside of the end round delegate. (veqryn)</li>

  <li>- Making TransportTracker a static implementation to clean up the engine a little bit. (veqryn)</li>

  <li>- Fixing various bugs in Global 1940, ww2v3, v4, v5, and v6. (veqryn)</li>

  <li>- Created new Player Rule Attachment, "immuneToBlockade", which will prevent blockade production loss for that player. (veqryn)</li>

  <li>- Allowed 1940's paratroopers tech (ariborne combat) to move to / attack territories that have been blitz or already conquered this turn. (veqryn)</li>

  <li>- Allowed 1940's paratroopers tech (airborne combat) to move from allied bases, and to allow travel over water. (veqryn)</li>

  <li>- Created new step properties for special move delegates, "airborneMove", which controls if it is an Airborne Combat move phase. (veqyrn)</li>

  <li>- Adding some more pre-industrial sounds. (pulicat)</li>

  <li>- Allowed muting of custom aa gun sounds and custom notification, victory, and defeat sounds. (veqryn)</li>

  <li>- Created resource image factory for making images and icons of resources. (veqryn)</li>

  <li>- Fixed user interface to allow purchasing resources. (veqryn)</li>

  <li>- Fixing engine to allow purchase rules for purchasing resources. (veqryn)</li>

  <li>- Fixed memory leak in repair rules for repairing factories. (veqryn)</li>

  <li>- Creating a menu option in the "File" menu called "Post PBEM/PBF Gamesave...", which will for pbem games post/email the savegame to the forum, without having to wait for the end turn phase. (veqryn)</li>

  <li>- Changing trigger "notification" to use "players". (veqryn)</li>

  <li>- Changing unit attachment property, "repairsUnits", to allow multiple and to have repair values associated with each unit, thereby allowing units to be repaired by X amount each turn. (veqryn)</li>

  <li>- Created new unitPlacement attribute, "unitDamage", which will let a unit start with bombing factory damage. (veqryn)</li>

  <li>- Created new unitPlacement attribute, "hitsTaken", which will let a unit start damaged. (veqryn)</li>

  <li>- Deleting game option property, "SBR Affects Unit Production", and simplifying the engine to only use direct unit damage. (veqryn)</li>

  <li>- Getting units with different bombing unit damage to not stack. (veqryn)</li>

  <li>- Allowing selection of casualties for multiple hit units to allow damage points past one. (veqryn)</li>

  <li>- Getting "hitPoints" to work in the graphical user interface. (veqryn)</li>

  <li>- Getting "hitPoints" to work on the back end inside the engine. (veqryn)</li>

  <li>- Created new unit attachment property, "hitPoints", which sets the number of hitpoints a unit has, and also deleted property "isTwoHit". (veqryn)</li>

  <li>- Allowing sounds to be played by trigger, by putting "_sounds" after a duplicate of the Notification message key, with the value equal to "notification_" or "victory_" or "defeat_" + the sound key found in the sounds.properties file. (veqryn)</li>

  <li>- Added logfile "dump" command for host bots, that will from the command line print out all status, connection, memory, and thread information to the log. (veqryn)</li>

  <li>- Created ability for lobby admins to mute and/or boot players in a host bot, remotely. (veqryn)</li>

  <li>- Created ability for lobby admins to see the player connections in any host game. (veqryn)</li>

  <li>- Created ability for lobby admins to see chatlog of a host bot remotely. (veqryn)</li>

  <li>- Adding a new autosave, 'autosave2', which will take turns being saved to with 'autosave'. (veqyrn)</li>

  <li>- Changing movement validation to disallow moving from a contested battle territory into an enemy territory. (veqryn)</li>

  <li>- Fixed bug with a territory owned by one player but having enemy units in it, if the owned reconquers the territory it is no longer marked as newly-conquered. (veqryn)</li>

  <li>- Fixed bug preventing sounds inside a zipped map from playing if the zipped map file path had any spaces or special characters in it. (veqryn)</li>

  <li>- Fixed bug preventing phase sounds from playing more than once in a non-pbem game. (veqryn)</li>

  <li>- Creating an option to select local players and AI's for PBEM games. AI's will not post/email the turn summary and savegame at the ends of their turns however. (veqryn)</li>

  <li>- Fixing bug with host bots where disabling players, quitting, then reloading and disabling even more players, resulted in game crash. (veqryn)</li>

  <li>- Disallowing previously disabled players from being re-enabled after a game has started. (veqryn)</li>

  <li>- Fixed bug with moderator lobby unbanning utility. (veqryn)</li>

  <li>- Created ability for lobby admins to ban players inside a host bot, remotely. (veqryn)</li>

  <li>- Created ability for lobby admins to stop game on a host bot remotely. (veqryn)</li>

  <li>- Created ability for lobby admins to shut down a host bot remotely. (veqryn)</li>

  <li>- Created new option for host bots, "triplea.lobby.game.supportPassword", which when set will allow remote actions on the host bot from the lobby admins. (veqryn)</li>

  <li>- Created new option for host bots, "triplea.lobby.game.reconnection", which will set the time between lobby reconnection refreshes, with the minimum and default being 6 hours. (veqryn)</li>

  <li>- Created new game option property, "Disabled Players Assets Deleted", which will delete all units and resources from a disabled unused player during game startup. (veqryn)</li>

  <li>- Allowing clients to disable and enable players for host bots, but not normal hosts. (veqryn)</li>

  <li>- Forcing random start to not allow disabled players to select territories, and also letting savegames keep disabled state, and disabled players switched to an AI. (veqryn)</li>

  <li>- Creating new playerlist option for players, "canBeDisabled", which if set to true will force the game to delete all delegates for that player, thereby allowing more customized multiplayer games. (veqryn)</li>

  <li>- Forcing hosts and hosting bots to always use Secure Random source when playing online, even when the host is not playing. (veqryn)</li>

  <li>- Updating TripleA to require at least Java 6 or greater. (veqryn)</li>

  <li>- Updating included jar libraries to latest versions. (veqryn)</li>

  <li>- Updating embedded JRE to Java 7 update 51 for x86. (veqryn)</li>

  <li>- Updated Substance UI to version 7.2.1, and included approximately 14 new Look and Feel skins. (veqryn)</li>

  <li>- Created a menu option called "User Notifications..." which lets you turn off notifications you would receive from End Turn Reports, Triggered Notifications, Chance rolls that are successful or failed. (veqryn)</li>

  <li>- Fixing Comment Log so that it updates in real time. (veqryn)</li>

  <li>- Changed automated hosting bots so that they show up as having 1 less player (ie: the bot itself doesn't count), which means zero players if noone else has joined. (veqryn)</li>

  <li>- Changed unit resource creation so that positive resources will be created before negative resources. (veqryn)</li>

  <li>- Fixing bug in destroyedTUV condition for allRounds that prevented it from working at all. (veqryn)</li>

  <li>- Added an updated engine jar for 1.7.0.5 so that the new engine can play old 1.7.0.x savegames. (veqryn)</li>

  <li>- Changed game setup screen so that the buttons for "Choose Game", "Load Saved Game", and "Game Options", will no longer be greyed out for Clients who have connected to an automated hosting bot. Those buttons will perform the same as if the client used the "Network" menu instead. (veqryn)</li>

  <li>- Adding a menu option to change an automated hosting bot's game options, and creating backend to process this request. (veqryn)</li>

  <li>- Forcing automated hosting bots have have a "support email address", so that when a bot has hung or stopped responding, a moderator in the lobby can email the bot's owner to notify them of the situation. (veqryn)</li>

  <li>- Forcing automated hosting bots to have no password, to start with the string "Bot", and have "automated_host" somewhere in comments. (veqryn)</li>

  <li>- Adding a column to the lobby called "B" for "Bots", which will show which hosts are automated hosting bots. They will also show up as italics. (veqryn)</li>

  <li>- Fixed order of firing in ww2v3 and Global 1940, so that defending subs that are not sneak attacking will fire after all attackers have fired. (veqryn)</li>

  <li>- Fixing a bug where attacking with a carrier loaded with allied fighters, then retreating, would prevent those fighters from being able to participate in battles for the rest of the game. (veqryn)</li>

  <li>- Allowed TripleA clip player to access sound files within a zipped map. (veqryn)</li>

  <li>- Fixed bug that allowed fighters to be moved greater than their allowed movement if paired with a carrier. (veqryn)</li>

  <li>- Adding scroll bars to placement window. (veqryn)</li>

  <li>- Fixed another bug in getMaxUnitsToBePlaced, it will no longer stop the game if it frees up enough capacity to place but not equal to theoretical maximum. (veqryn)</li>

  <li>- Fixed bug where a strategic bombing unit receiving negative support and/or negative terrain modifier would be unable to bomb is its attack power decreased to zero. (veqryn)</li>

  <li>- Created new step properties for move delegates, "combinedTurns", which changes some validation for intermeshed player phases, such as allowing air to live if the ally could place a carrier under them. (veqyrn)</li>

  <li>- Created new step properties for purchase and place delegates, "bid", which controls if it is a bid phase. (veqyrn)</li>

  <li>- Created new step properties for move and end turn delegates, "repairUnits", which controls when units get repaired. (veqyrn)</li>

  <li>- Created new step properties for move and place delegates, "removeAirThatCanNotLand", which controls when air that can not land gets killed. (veqryn)</li>

  <li>- Created new step properties for move delegates, "resetUnitState", which controls when units get their movement and other stats reset. (veqryn)</li>

  <li>- Created new step properties for move delegates, "giveBonusMovement", which controls when bonus movement is given. (veqryn)</li>

  <li>- Created new step properties for move delegates, "fireRockets", which controls when rockets fire. (veqryn)</li>

  <li>- Created new step properties for move delegates, "combatMove" and "nonCombatMove", which control movement validation. (veqryn)</li>

  <li>- Prevented AA type units from firing on both start and end of movement, when option "Force AA Attacks For Last Step Of Fly Over" is turned on. (frogg)</li>

  <li>- Created new game property option "Abandoned Territories May Be Taken Over Immediately", which allows an abandoned territory to be taken over on the turn it was abandoned, rather than waiting for it to be attacked. (veqryn)</li>

  <li>- Created new game property option "Sea Battles May Be Ignored", which allows attackers to not create a battle in a contested sea zone. (frogg)</li>

  <li>- Created new game property option "Contested Territories Produce No Income", which will stop all production in territories that contain enemy units. (frogg)</li>

  <li>- Created new game property option "Retreating Units Remain In Place", which will allow retreats to only the same territory as the battle. (frogg & veqryn)</li>

  <li>- Allowed AxisAndAllies.org forum poster to maintain "notify me" settings. (Bruce Nielsen)</li>

  <li>- Changed trigger property "when" so that it can be set multiple times, allowing a trigger to fire multiple times per round. (frogg)</li>

  <li>- Changed game property option "Battle Rounds" to "Land Battle Rounds". (veqryn)</li>

  <li>- Added game property option "Sea Battle Rounds". (frogg)</li>

  <li>- Possible fix for host game hang, when host is launching and another player leaves or joins at start of launch. (veqryn)</li>

  <li>- Possible fix for game hang / game freeze during hosting, client start step should now wait for delegate bridge to finish updating. (veqryn)</li>

  <li>- Possible workaround for game hang / game freeze during hosting, if error occurs game should now drop back to waiting screen instead of just hanging or ghosting. (veqryn)</li>

  <li>- Adding much more logging to HeadlessServerGame in order to try to find cause of the CastClassExceptions in TripleAPlayer.start() and NullPointer/IllegalArgumentExceptions in RemoteName. (veqryn)</li>

  <li>- Fixed null pointer error in battle calculator when spamming the cancel button. (veqryn)</li>

  <li>- Rebalancing Great War world war 1 game. (veqryn)</li>

  <li>- Fixed bug where chanceIncrementOnFailure and chanceDecrementOnSuccess were not allowing any number of zero or less for chance. (veqryn)</li>

  <li>- Fixed error where games with a round offset where doubling what round the game started on each time it was saved via the history panel. (veqryn)</li>

  <li>- Creating a headless chat service, so that server can be created in a headless environment and still chat. (veqryn)</li>

  <li>- Fixed bug causing fatal errors in client-server games when client owned very last step/delegate of game (only applied to some grid based games). (veqryn)</li>

  <li>- Adding a log file for the headless server located at /log/headless-game-server-<servername>-log<#>.txt, to keep track of events. (veqryn)</li>

  <li>- Adding many more additional commands to headless game server console, including show connections, ban player, save game, and stop game. (veqryn)</li>

  <li>- Stopped headless game server from being able to load any savegame for a map to which it does not have the required map files for. (veqryn)</li>

  <li>- Possible fix another possible hang/freeze point causing a Could Not Block Delegate Execution error. (veqryn)</li>

  <li>- Fixed headless game server's connect to lobby so that resetting the connection does not erase info about the game. (veqryn)</li>

  <li>- Possible fixes two possible hang/freeze points in Server Game, one caused by a bogus ClassCastException in ClientGame, the other by a bogus NullPointerError/IllegalArgumentError in RemoteName from PlayerDelegateBridge. (veqryn)</li>

  <li>- Making sure sound system never loads sound clips for headless game server. (veqryn)</li>

  <li>- Added a console to automated headless game server host, which allows commands such as 'help', 'status', 'memory', 'threads', and 'quit'. (veqryn)</li>

  <li>- Created a headless UIContext for use with headless game server, so that it may run on a linux platform that has no configured graphics environment. (veqryn)</li>


</ul><h3>Changes for 1.7.0.3</h3><ul>
  <li>- Got headless game to show options to client's, for changing the game, changing to an autosave, sending a save to the server, and getting the savegame from the host. (veqryn)</li>

  <li>- Got headless game to restart its lobby connection once per 8 hours. (veqryn)</li>

  <li>- Got headless game server to be able to connect to lobby, and host games repeatedly without requiring any UI or swing event thread. Also got to immediately reload autosave when a player quits. (veqryn)</li>

  <li>- Got headless game server to be able to pick games, and have a mini-ui for hosting and for during the game. (veqryn)</li>

  <li>- Got headless game server to be able to host minimap, with the game screen headless. (veqryn)</li>

  <li>- First pass at setting up framework for a headless game server. (veqryn)</li>

  <li>- Preventing AA units with maxRoundsAA from getting removed early from battle. (veqryn)</li>

  <li>- Fixed bug causing Random Territory Start delegate to fail in online games due to requesting dice too quickly. (veqryn)</li>

  <li>- Updating Great War ww1 map and xml, to improve options and balance. (veqryn)</li>

  <li>- Updating packaged JRE to Java 7 update 21 for x86. (veqryn)</li>

  <li>- Made fuelCost no longer charge for allied air dependants, paratroopers, and owned air on owned fighters not making an attack. (veqryn)</li>

  <li>- Created new game option property, "Use Fuel Cost", which will control if we charge for fuel in our movement. (veqryn)</li>

  <li>- Added an option to turn off the end of turn report, into the game menu bar. (veqryn)</li>

  <li>- Changed engine preference for max memory into a "system.ini" file, that way a user can delete or reinstall TripleA if they screw up. (veqryn)</li>

  <li>- Created new engine preference option to set the maximum memory used for triplea, for joining, hosting, and also an option to have triplea always restart with higher memory maximum. (veqryn)</li>

  <li>- Created new option in engine preferences to show engine log console, and also had the console show current memory usage. (veqryn)</li>

  <li>- Reducing maximum memory to 896mb, down from 1024mb, in order to stop these errors from happening, and not allowing engine to add 20% to this when joining online games or hosting. (veqryn)</li>

  <li>- Figuring out some user's Java jvm's and/or the JRE included with triplea, only allow up to xmx 1024mb of memory maximum, and that the program completely fails when going over this limit, often causing the user to be unable to join or host games online. (veqryn & diaz)</li>

  <li>- Fixing some lock not held errors. (veqryn)</li>

  <li>- Fixed bug causing triggered notifications to not use local images when shown on a client computer. (veqryn)</li>

  <li>- Not allowing scrambling question when only and SBR raid is in a territory and scramble to SBR is turned off. (veqryn)</li>

  <li>- Fixed bug causing Territory Effects to not be applied at all, ever. Also fixed possible issue with 'choose best roll' in low luck. (veqryn)</li>

  <li>- Fixed bug causing national objectives which rewarded players on a per-territory basis using the "each" modifier to not work. (veqryn)</li>

  <li>- Fixed bug causing paratrooping land units who's air transports were hit by AA fire to not be removed from the battle. (veqryn)</li>

  <li>- Fixed possible null pointer in color chooser for color property, which occurred when chosing the color for map text. (veqryn)</li>


</ul><h3>Changes for 1.7.0.1</h3><ul>
  <li>- New attachment properties for Triggers, Politics, and User Actions: "chanceIncrementOnFailure" and "chanceDecrementOnSuccess" which will modify the "chance" value. (veqryn)</li>

  <li>- Fixing fuelCost to not be charged for units in transports. (veqryn)</li>

  <li>- Major changes to both the map and the placements and the rules for "Great War" world war one game. (veqryn)</li>

  <li>- Implemented all sounds through IDelegateBridge.getSoundChannelBroadcaster().playSoundForAll() or through DefaultSoundChannel.playSoundOnLocalMachine() for a few local sounds like slapping in chat. (veqryn)</li>

  <li>- Created new channel broadcaster for use with playing sounds on both server machine and client machines. (veqryn)</li>

  <li>- Created user interface element for RandomStartDelegate, so that players can pick which territory they want and what units they want in it. (veqryn)</li>

  <li>- Gave all AIs methods to pick territories, and they will attempt to focus on a single area of the board. (veqryn)</li>

  <li>- Created new game option property, "Territories Are Assigned Randomly", which determines if territories are randomly assigned or picked by players during RandomStartDelegate. (veqryn)</li>

  <li>- Created new delegate, "RandomStartDelegate", which will allow for randomly assigned territories or territories chosen in turn order. (veqryn)</li>

  <li>- Fixed problem where territory names that were parseable integers could not allow any territory based conditions. I still recommend territories have a non integer character in them though. (veqryn) </li>

  <li>- Fixed null pointer error in signalGameOver when called by a trigger for a game that has never reached the end round step. (veqryn)</li>

  <li>- Minor adjustment to retain capital produce number methods to allow a value of zero. (flaaargle)</li>

  <li>- Created user interface element for the User Action Delegate, based on the existing politics interface. (veqryn)</li>

  <li>- Created new delegate, "UserActionDelegate", which will allow nations to take any kind of condition/trigger based action. (veqryn)</li>

  <li>- Created new text file, "actionstext.properties", which contains action text for the user interface for taking user actions, similar to politicstext.properties. (veqryn)</li>

  <li>- Added new property, "activateTrigger", to UserActionAttachment, which will fire a trigger when the nation takes this action. (veqryn)</li>

  <li>- Added properties for conditions, conditionType, invert, chance, costPU, text, actionAccept, and attemptsPerTurn to the User Action Attachment. (veqryn)</li>

  <li>- Created new attachment, "UserActionAttachment", which holds actions that can be taken by a player, based on an abstraction of the political action attachment. (veqryn)</li>

  <li>- New Condition Attachment property option, "gameProperty", which can be set equal to the exact string of any boolean game property option, including custom made up ones. (veqryn)</li>

  <li>- Created new AI specially for multiplayer free-for-all games, "Does Nothing AI", which will buy units the first round then destroy all money all subsequent rounds, along with doing nothing else. (veqryn)</li>

  <li>- Abstracted methods to find the power and rolls of units into a single method. (veqryn)</li>

  <li>- Fixed issue with Marine amphibious attackers showing a bonus on the battle screen even when attacking via land. (veqryn)</li>

  <li>- Fixed null pointer error in Strong AI (Moore AI). (veqryn)</li>

  <li>- Getting the UnitSupportAttachment faction option to handle both allied and enemy, thereby allowing giving positive or negative support to enemy units. (veqryn)</li>

  <li>- Getting the UnitSupportAttachment dice option to handle both strength and roll, thereby allowing giving extra rolls to units. (veqryn)</li>

  <li>- Changing defending submarines to fire after all attacking units under classic rules, where property Defending Subs Sneak Attack is false. (veqryn) </li>

  <li>- Created new button, "Order of Losses", in the battle calculator, which will all you to put in a text script of which casualties to select in what order. (veqryn)</li>

  <li>- Added option to retreat in battle calculator when we are losing, which is approximated by seeing if our 'meta-power' is lower than the opponent's. (veqryn)</li>

  <li>- Created new image utility, TileImageReconstructor, which will recreate an image based on base tiles or relief tiles and/or draw a polygons file onto an image. (veqryn)</li>

  <li>- Adding a visual log to AutoPlacementFinder and TileImageBreaker, and getting the AutoPlacementFinder to cut out at a max of about 50 placements per territory. (veqryn)</li>

  <li>- Changed unit attachment "isMarine" to allow for integers instead of boolean. (veqryn)</li>

  <li>- Updated default casualty selection to take territory effects into consideration. (veqryn)</li>

  <li>- Updating web poster to keep track of many entered websites, and save them all to the local cache but not to the savegame. (veqryn)</li>

  <li>- Created new unit attachment property, "canAirBattle", which determines if a unit participates in a normal battle's air battle. (veqryn)</li>

  <li>- Allowing defense to ground their planes before an air battle (preceding a normal battle) if withdrawing is turned on, however if the territory is lost they die. (veqryn)</li>

  <li>- Fixed battle screen null pointer errors caused by maps with artillery units but no supportable units. Also fixed bug where maps without notes could not be closed. (veqryn)</li>

  <li>- Allowed AA Gun type units to fire back in same round if killed by other AA Gun type units. (veqryn)</li>

  <li>- Added new steps to must fight battle so that offensive aa guns will work correctly. (veqryn)</li>

  <li>- Created new unit attachment properties, "offensiveAttackAA" and "offensiveAttackAAmaxDieSides", which will be used by offensive aa guns. (veqryn)</li>

  <li>- Created new unit attachment property, "maxRoundsAA", which sets the number of rounds an AA gun may fire in, with 1 being default. Only normal battles are affected, while flyover and strategic bombing are not affected. (veqryn)</li>

  <li>- Created new game option property, "Battle Rounds", which sets the maximum number of rounds of combat for normal battles, with -1 being infinite which is default. (veqryn)</li>

  <li>- Created new game option property, "Can Scramble Into Air Battles", which will allow a player to scramble air to neighboring territories in order to defend against air raids and air battles. (veqryn)</li>

  <li>- Set up battle delegate and tracker to allow air battles to be created for normal battles. (veqryn)</li>

  <li>- Created new game option property, "Battles May Be Preceeded By Air Battles", which will allow normal battles to have air battles first. (veqryn)</li>

  <li>- Created new game option properties, "Air Battle Attackers Can Retreat" and "Air Battle Defenders Can Retreat", which allow retreating from air battles. (veqryn)</li>

  <li>- Created new game option property, "Air Battle Rounds", which will allow setting the number of rounds of combat for air battles. (veqryn)</li>

  <li>- Abstracted StrategicBombingRaidPreBattle to become AirBattle, no longer extending StrategicBombingRaid. (veqryn)</li>

  <li>- Fixed bug that caused a rare skipping of a battle involving transports and air vs undefended transports. (veqryn)</li>

  <li>- Adding new PBEM feature, the ability to post to a custom triplea website. (weigo)</li>

  <li>- Adding scroll bar to chat panel for online game waiting host room before game launched. (veqryn)</li>

  <li>- Expanded Unit tool tips to include unit support attachments, and also to detail more info for other abilities. (veqryn)</li>

  <li>- Increasing maximum memory to 1gb (1024mb), up from 768mb. (veqryn)</li>

  <li>- Creating a new monthly check to see if all maps are up to date, and if not then asking the user to update their maps. (veqryn)</li>

  <li>- Allowed "men" in International Draughts to capture backwards, which appears as a game option in Checkers. (veqryn)</li>

  <li>- Created caching mechanism for the game notes, so that it is only in memory when the notes tab is open and otherwise can be cleared from memory if needed. (veqryn)</li>

  <li>- Created a new Unit Attachment option, "damageableAA", which allows this AA gun type unit to cause damage to a two hitpoint unit instead of outright killing it. (veqryn)</li>

  <li>- Fixed bug where AA shots on 2 hitpoint units with Choose AA Casualties on was resulting in no damage or killed unit. Also changed battle display to show "typeAA" for each AA Fire phase, instead of a generic identifier. (veqryn)</li>

  <li>- Allowing custom AA hit and miss sounds for irregular AA types, with the folder being located at "battle_<typeaa>_hit" and "battle_<typeaa>_miss" (folder must be lowercase though), where <typeaa> is the unit attachment "typeAA" of that unit. (veqryn)</li>

  <li>- Adding text labels to the Battle Calculator for the number of hitpoints and the total attack or defense power of each side. (veqryn) </li>

  <li>- Adding a new Hot Key "F" for 'Find Units', which will highlight all units you own that have movement left, but only during a movement phase. (frigoref)</li>

  <li>- Allowed Edit Mode to add land units to a sea zone if there are either transports already there or transports also being added at the same time. (veqryn)</li>

  <li>- Allowed Edit Mode to remove units owned by different players. (veqryn)</li>

  <li>- Changed territory attachment "victoryCity" to allow integers instead of boolean, thereby allowing victory cities with greater value, and also added a tooltip to tech purchase phase to show what techs are in each category. (eurofabio)</li>

  <li>- Allowed Edit Add Units to check if artwork exists for units not in a production frontier, and if so allow them to be created. (veqryn) </li>

  <li>- Added more info to Battle Calc including total TUV swing, and allowing retreat after losing all air units or having only x units left. (veqryn)</li>

  <li>- Fixed bug where having sea units begin the turn on top of an enemy sub, and then not moving them but also not attacking, caused them to lose their movement anyway. (veqryn)</li>

  <li>- Fixed bug where you could move a destroyer after it had killed a sub, during noncombat move. (veqryn)</li>

  <li>- Updating text xml's and adding TWW xml for new tests. (veqryn)</li>

  <li>- Fixing bug in air movement validation for complex movement cases. (veqryn)</li>

  <li>- Fixing several memory leaks related to game notes staying in memory multiple times. (veqryn)</li>

  <li>- Creating Edit Mode for Grid Based games like chess, checkers, and go. (veqryn)</li>

  <li>- Added feature to automatically parse HTML text in game notes and in notifications, and replace all image links with links to the map folder's "doc/images/" directory, thereby allowing local image files to be used. (veqryn)</li>

  <li>- Adding ability to specify when the attacker should retreat after how many rounds, to the battle calculator. (veqryn)</li>

  <li>- Added fields for average number of rounds, average attacking units left when attacker won, and average defending units left when defender won, to the battle calculator. (veqryn)</li>

  <li>- Added new Edit option to change political relationships between players. (veqryn)</li>

  <li>- Created option in game 'View' menu to change the font size and font colors of things like territory names, pu's, unit count, and factory damage count. (veqryn)</li>

  <li>- Fixed serious bug with process runner util that prevented a new classpath from being used, most notably preventing the 'old jars' from getting run. (veqryn)</li>

  <li>- Creating a method in IDisplay to send messages to all player's computers, but only once per computer. Also includes ability to send to certain players only. (veqryn)</li>

  <li>- Forced all non-returning void dialogs to run in a separate process as to not block the game from moving forward. </li>

  <li>- Forced all UI interactions to either go through a single thread, or wait for thread to finish, so as not to have multiple popups at same time. (veqryn)</li>

  <li>- Creating simple message dialog report for end of turn collection of PUs and national objectives and any blockade action. (veqryn)</li>

  <li>- Creating a mouse shadow image to go with the route image, showing how much movement you have left for any selected units, in blue font. (veqryn)</li>

  <li>- Possibly fixing bug where the game host process does not end, even though all windows close. (veqryn)</li>

  <li>- Allowing all Grid Games to use the play by email and forum posters. (veqryn)</li>

  <li>- Abstracted the Forum Poster to its own component and static methods. Added new checkboxes for including savegame and for reposting the turn if it failed the first time. (veqryn)</li>

  <li>- Creating victory conditions for Go, and creating a UI for players to negotiate which groups of stones are alive or dead. (veqryn)</li>

  <li>- Creating all game logic for Go. (veqryn)</li>

  <li>- Creating UI for Go. (veqryn)</li>

  <li>- Allowing Grid Games to change their width and height mid-game, like through game options. (veqryn)</li>

  <li>- Creating initial framework and loader for Go. (veqryn)</li>

  <li>- Creating simple AI for Checkers, and adding rules to enforce the forcing of jump capture moves when available. (veqryn)</li>

  <li>- Creating UI for Checkers. (veqryn)</li>

  <li>- Adding all game logic for Checkers. (veqryn)</li>

  <li>- Adding sound for joining a game chat room. (cpp-ose & jeparedes)</li>

  <li>- Creating framework and loader for Checkers. (veqryn)</li>

  <li>- Adding Chess to available games that come with TripleA, and cleaning up source and UI, and fixing various bugs in the grid games framework. (veqryn)</li>

  <li>- Getting Grid Games to use the History Panel, and adding the history panel and other options to their menu bar. (veqryn)</li>

  <li>- Getting GridMapPanel to scroll by having it extend ImageScrollerLargeView, and fixing up all grid based games to use this. (veqryn)</li>

  <li>- Getting Grid Games to allow having a chat panel in multiplayer and networked games. (veqryn) </li>

  <li>- Abstracting both Sliding Tiles (N-Puzzle) game and Tic Tac Toe game into Grid Game. (veqryn)</li>

  <li>- Created a min-max/alpha-beta type of AI, which takes a long time to think but actually makes OK moves. (veqryn)</li>

  <li>- Created a very very simple AI for Chess, based on random moves plus capturing pieces when available. (veqryn)</li>

  <li>- Finished checking for Check and Check Mate in Chess. (veqryn)</li>

  <li>- Finishing movement validation for Chess. (veqryn)</li>

  <li>- Adding a visual cue for which moves are legal for Chess and other Grid games. (veqryn)</li>

  <li>- Added movement validation logic for Chess. (veqryn)</li>

  <li>- Upgrading the graphics for Grid Games, and including a mouse shadow of selected units, and a highlight of which units on map are currently selected. (veqryn)</li>

  <li>- Major abstraction of both King's Table and Chess into a single framework for Grid based games. (veqryn)</li>

  <li>- Completing most of UI aspect of Chess game. (veqryn)</li>

  <li>- Creating framework for a Chess game. (veqryn)</li>

  <li>- Created a notification to the user when they start a version of TripleA for the first time, showing the new features of this version. (veqryn)</li>

  <li>- Created a notification to the user when they start TripleA that checks if their TripleA is the latest version, and if not asks them to update it. (veqryn)</li>

  <li>- Created a notification to the user when they click "list games" that will alert them to which maps they already have which may be out of date and need updating. (veqryn)</li>

  <li>- Added the default map downloader xml web link to the download maps feature, if the user does not already have any. (veqryn)</li>

  <li>- Fixed movement validation bug that prevent loading of land units onto a transport during noncombat if the transport was in an enemy 'owned' sea zone. (veqryn)</li>

  <li>- Fixed bug where units being transported or otherwise dependent were being counted towards unit presence and unit exclusion objectives. (veqryn)</li>

  <li>- Changing territory attachment "occupiedTerrOf" into "originalOwner". (veqryn)</li>

  <li>- Deleting game option property "Occupied Territories" since it does not do anything anymore. (veqryn)</li>

  <li>- Created new territory effect attachment option, "unitsNotAllowed", which is a list of units that will be prevented from moving into any territories with this effect. (crystalct) </li>

  <li>- Adding ability to specify which round the game starts on, through a round offset in gameplay section of xml. (veqryn)</li>

  <li>- Added ability to Right Click on any node in the History panel, and save a game at that point in history [could still be buggy, do not use for tournament games]. (veqryn)</li>

  <li>- Abstracted delegates so that the server can now determine if it needs to wait on the user for input for a delegate or not. (veqryn)</li>

  <li>- Fixed bug where having a tech token but not having enough money to buy a new one, would cause you to skip rolling for the existing token. (veqryn)</li>


</ul><h3>Changes for 1.6.1.4</h3><ul>
  <li>- Adding dotted lines to the LOTR Middle Earth map, to show connections over rivers. (veqryn)</li>

  <li>- Not showing tech in stats panel if game xml does not have any technologies. (veqryn)</li>

  <li>- Created new stepProperty, "turnSummaryPlayers", which holds a list of players for whom we will include their turn summary information in the forum/email post. (veqryn)</li>

  <li>- Created new stepProperty, "skipPosting", which when true will skip the forum posting for that EndTurn type step. (veqryn)</li>

  <li>- Created new xml option type "stepProperty" for a step (gamePlay - sequence), which can hold small options for modifying a delegate step. (veqryn)</li>

  <li>- Adding some more sounds for ancient/classical era. (veqryn)</li>

  <li>- Adding some more ww2 sounds and national anthems for main players. (hepster)</li>

  <li>- Allowing air movement over neutrals and enemy territories so long as movement over neutrals is allowed, and no nonparatrooping units are present. (veqryn)</li>

  <li>- Creating caching mechanism for sound clips, so that there are never more than 24 sound clips being held in memory. This should prevent errors in MacOS and Linux, which can not handle having large number of sound clips open at same time. This may however result in a delay before hearing clips, and still could result in errors if clips are really long. (veqryn)</li>

  <li>- Fixed null pointer error for a trigger based game property change of a field that starts out as null. (veqryn)</li>

  <li>- Fixed bug in strategic bombing that allowed strategic bombing of units that can be damaged, which were also being transported. (veqryn)</li>

  <li>- Adding scroll bars to notification messages window. (veqryn)</li>

  <li>- Increasing max memory from 640mb to 768mb, and up to 896mb for online games. (veqryn)</li>

  <li>- Moved all sounds to a specific "era" folder (ww2, preindustrial, classical, future) and changing how sounds are found again, so that there should no longer be any need for duplicate sound files. Now all sounds should come with TripleA, and you can use the "sounds.properties" file to cherry pick which sounds you want. (veqryn)</li>

  <li>- Created a "sounds.properties" file which allows you to specify which era of sounds (ww2, preindustrial, classical, future) you are using, and also set up custom sound choices for each sound location path. (veqryn)</li>

  <li>- Getting TripleA Map Panel to center on the capital of a player, whenever we switch to a new player's phase. (veqryn)</li>

  <li>- Changing getBoundingRect and createTerritoryImage and getTiles so that any polygons on the right or bottom will be translated to be on the negative left or top, hopefully solving issue where the mini territory image was not being displayed properly for territories on both sides of a map divide. (frigoref) </li>

  <li>- Abstracting the Stats panels into AbstractStatPanel so that extending Stats panel (and all of its overhead) is no longer necessary for the EconomyPanel, ObjectivePanel, TerritoryDetailPanel, and other panels. (veqryn)</li>

  <li>- Changing Tech Stats Panel to use small flag images for column headers instead of the first letter of nation names. (veqryn)</li>

  <li>- Fixing bugs with placing constructions in sea zones. Now constructions can only be "produced" by the territory they are going into. (veqryn)</li>

  <li>- Adding a lot more sounds to the engine (zim xero) and some sounds specific to napoleonic empires. (hepster & veqryn)</li>

  <li>- Added tutorial on how to make a map and/or map skin. (veqryn)</li>

  <li>- Allowing for Sea Factories, and Air Factories, to produce from owned sea zones. (veqryn)</li>

  <li>- Added UPnP support to TripleA, so that TripleA will now attempt to Forward Ports for the user.  This means users should no longer have to do port forwarding themselves to be able to host a game online. (veqryn)</li>

  <li>- Created framework for using UPnP library, and UI component for user. (veqryn)</li>

  <li>- Added java library for Universal Plug and Play (UPnP) to TripleA. (veqryn)</li>

  <li>- Created new HotKey, "N", which when pressed during a movement phase, will cycle through all units with available movement left, focusing the map on the unit. (veqryn)</li>

  <li>- Created new HotKey, "I", which when pressed will create a popup for 5 seconds showing all the info about the unit and/or territory your mouse is currently over. (veqryn)</li>

  <li>- Allowing the map to be scrolled by using the arrow keys and/or WASD. (veqryn)</li>

  <li>- Added original owner, whenCapturedByGoesTo, captureUnitOnEnteringBy, and changeUnitOwners to the Territory tooltip and territory tab info. (veqryn)</li>

  <li>- Fixing Move Panel and Place Panel so that Undoing a move or place will not result in scrolling back to the top, and will instead scroll to make sure that the move under the undoed move is still visible. (veqryn)</li>

  <li>- Allowing all sounds to have a player associated with them.  Just name the sound "<soundName>_<playerName>".  If the player sound does not exist, it will use the default non-player sound. (veqryn)</li>

  <li>- Added a ton more new sounds to the engine. (veqryn)</li>

  <li>- Changed Sounds so that instead of specific sound files, the engine will search for specific sound folder. The engine will then randomly select a sound in that folder and play it. This allows for randomized sounds. (veqryn)</li>

  <li>- Made sure any clicking or dragging gives focus to the main map panel area. Also ensuring that if focus goes to the tabs panel tabs, that the focus goes back to the map. (veqryn)</li>

  <li>- Created new game option property, "Submarines Defending May Submerge Or Retreat", which will allow defending submarines to submerge or retreat to a friendly neighboring sea zone. (veqryn)</li>

  <li>- Deleting game option property, "Hari-Kari Units", since it doesn't do anything at this point. (veqryn)</li>

  <li>- Deleting game option property, "Previous Units Fight", since it doesn't do anything at this point. (veqryn)</li>

  <li>- Allowing sea units to retreat back if the retreating to territory contains only ignored enemy units. (veqryn) </li>

  <li>- Disallowing rockets from firing over impassible territories by default. (veqryn)</li>

  <li>- Added message on how long a ban lasts for, when a user tries to reconnect to the lobby. (veqryn)</li>

  <li>- Created ui wrapper for properties, and allowed most to be editable. (veqryn)</li>

  <li>- Created new map utility, "MapPropertiesMaker", which will make the "map.properties" file. (veqryn)</li>

  <li>- Added an 'Is Amphibious' check box to the battle calculator, so that units like marines will correctly calculate for an amphibious battle. (veqryn)</li>

  <li>- Getting Decoration Placer to auto place all images nicely on the map if they match the territory names or if they are not decorations. Also including detailed instructions. (veqryn)</li>

  <li>- Got the Decoration Placer to work with placing PUs, decorations, name images, capitals, vc's, and all other image types and text files. (veqryn)</li>

  <li>- Creating new map utility, "Decoration Placer", which allows a map maker to put decorations and other images on a map, recording their points in a text file. (veqryn)</li>

  <li>- Fixed bug in Triggers that use "chance" and also have more than 1 action or event inside them, so that they will no longer test once for each action, and instead only one time total. (veqryn)</li>

  <li>- Created new tab, "Notes", which will just show the game notes, on the right side of the screen. (veqryn)</li>

  <li>- Getting the objective panel to not refresh more than every 10 seconds, and adding a "Refresh" button so that it can be manually refreshed. (veqryn)</li>

  <li>- Getting the objectives on the objective tab to show up in colors (red = true, blue = used up), and show more information: <#of uses left><T=true/F=false><#of objectives filled>. (veqryn)</li>

  <li>- Including on Objective tab whether condition is currently true or not, and getting it to update with the game. (veqryn)</li>

  <li>- Creating new text file, "objectives.properties", which will hold all the details about what objectives to show on the objective tab. (veqryn)</li>

  <li>- Creating new stats panel, "Objective" Tab, which will contain a list of all national objectives and any other conditions the map maker wants. (veqryn)</li>

  <li>- Created new "map.properties" variables: "map.cursor.hotspot.x", and "map.cursor.hotspot.y". (veqryn)</li>

  <li>- Allowing TripleA to use custom cursors located at "misc/cursor.gif". (veqryn)</li>

  <li>- Getting TripleA to use any sounds located in a folder named "sounds" in any map file, thereby allowing custom sounds for every map. (veqryn)</li>

  <li>- Renaming the "images" folder into "assets", and then moving the "sounds" folder to be inside of the "assets" folder, inside the triplea program directory. (veqryn)</li>

  <li>- Created new text file, "comments.txt", which will control where things like convoy route names and comments will go. (veqryn)</li>

  <li>- Deleted "map.properties" variable "map.showConvoyNames" and replaced with "map.showComments". (veqryn)</li>

  <li>- Created new folder, "territoryNames", which can be filled with .png images of each territory name. These will be displayed at the points in "name_place.txt". (veqryn)</li>

  <li>- Created new "map.properties" variables: "units.stack.size", "map.showSeaZoneNames", and "map.drawNamesFromTopLeft". (veqryn)</li>

  <li>- Deleting xml property, "Display Sea Names", and will replace it with a map.properties property "map.showSeaZoneNames", because display options should not be in the xml, only game logic should be. (veqryn)</li>

  <li>- Deleting xml property, "Display Units as Counters", and will replace it with a map.properties property "units.stack.size", because display options should not be in the xml, only game logic should be. (veqryn)</li>

  <li>- Created new "map.properties" variable "map.scrollWrapY", and got TripleA to successfully scroll in the Y direction, as well as both X and Y at the same time seamlessly. (veqryn & frigoref)</li>

  <li>- Created new "map.properties" variables: "map.showResources", and "screenshot.title.enabled". (veqryn)</li>

  <li>- Creating a ConnectionFinder for the 'map' part of the xml. (edwin van der wal)</li>

  <li>- Adding Mnemonics to menu options in game. (frigoref)</li>

  <li>- Improved performance of Polygon Grabber and added a auto-grab to it to will attempt to grab any polygon that does not contain other polygons, based on the centers file. (edwin & veqryn)</li>

  <li>- Set up UI for map creator, fixed it up to be able to run all utility files, including sending arguments to them. (veqryn)</li>

  <li>- Creating a new Map Creator / Map Maker that is accessible from the Engine Preferences section of TripleA. (veqryn)</li>

  <li>- Updating TileImageBreaker and PlacementPicker to include more notes on how to use them, as well as fixing some bugs and allowing arguments and remembering selections. (veqryn)</li>

  <li>- Updating CenterPicker and PolygonGrabber and AutoPlacementFinder to include more notes on how to use them, as well as allowing arguments and remembering selections. (veqryn)</li>

  <li>- Fixing Global 1940 to match 2nd Edition version. (veqryn)</li>

  <li>- Preventing fighters that used up all movement to get to a battle, from getting to retreat. (veqryn)</li>

  <li>- Allowing PlacementPicker and AutoPlacementFinder to accept two arguments (when run by command line), the width and the height, of the placements. (veqryn)</li>

  <li>- Fixed issues preventing the smallMap from being updated after switching map skins. Also polishing up support for map skins that are totally different than the original map. (veqryn)</li>

  <li>- Creating new "map.properties" variables: "units.width", "units.height", "units.counter.offset.width" and "units.counter.offset.height", allowing maps to use non-standard sized unit images. (veqryn)</li>

  <li>- Fixing a bug in center picker, and fixing a bug where selecting a map skin didn't verify the map before changing the user preferences. (veqryn)</li>

  <li>- Fixed bug where rockets could attack a factory multiple times. (veqryn)</li>

  <li>- Deleting the game option "Rocket Attack Per Factory Restricted", and replacing it with its inverse, "Rocket Attacks Per Factory Infinite". (veqryn)</li>

  <li>- Fixed issue with not being Java 1.5 compatible. (veqryn)</li>

  <li>- Fixed null pointer error in getSkins method when user has installed triplea to the user folder. (veqryn)</li>

  <li>- Fixed issue with showing Turn Summary from right clicking on the player's node while in the History mode, which showed the current player's territory summary instead of the selected player. (veqryn)</li>

  <li>- Fixing movement validation bug that disallowed movement into a sea zone controlled by the enemy with subs, if the sea zone also had an owner, even if subs are being ignored. (veqryn)</li>

  <li>- Adding new AI, "Moore N Able (2)", with ability to read a script file from map folder. (kmoore)</li>

  <li>- Fixing Concurrent Modification error with getIsAmphibiousMarine method in battle display. (veqryn)</li>

  <li>- Fixing comparison method in Easy AI (weak ai) so that adheres to the comparison contract. Also cleaned up a lot of code, fixed a lot of warnings. (veqryn)</li>

  <li>- Fixing bug history panel bug caused by loading a savegame at the end of the last player's turn, causing a "Can not add event, not in step" error to be thrown. (veqryn)</li>

  <li>- Adding new menu option "Focus On Own Casualties", which when selected will cause the default casualty selection to focused, allowing the user to hit spacebar to accept it. (hakon)</li>

  <li>- Changed order of steps so that in games where Submarines may submerge before battle, the attacker is asked first, then the defender is asked. (hakon)</li>

  <li>- Showed convoy blockade dice rolls in History Panel even if the blockade damage is zero. (veqryn)</li>


</ul><h3>Changes for 1.6.1.2</h3><ul>
  <li>- Fixed bug in Paratroopers code, causing paratrooper attacks in coast territories on maps with scrambling to never actually take the territory. (veqryn)</li>

  <li>- Creating a simple Ping method inside of the Chat Controller, that will ping all computers once every minute, hopefully improving everyone's connections. (Sean Bridges & veqryn)</li>

  <li>- Allowing people to hold SHIFT down while their mouse is over a territory in order to keep that territory in the Territory Panel, no matter where they move their mouse afterwards. (frigoref)</li>

  <li>- Changed EndTurnDelegate so that Units Changing Ownership, and Hitpoint Repair, will still happen even if you have lost your capital. (veqryn)</li>

  <li>- Getting MooreAI to submerge subs if only enemy air is left. (hakon)</li>

  <li>- Fixing "Edit Unit Bombing Damage" for maps that use territory based damage, such as ww2v3. (veqryn)</li>

  <li>- Allowing new option for the Play By Email / Play By Forum poster, to "Include Overall Dice Statistics" in the post/email. (veqryn)</li>

  <li>- Improving the menu "GAME -> SHOW DICE STATS" to give information per player, as well as totals. (veqryn)</li>

  <li>- Getting engine to record if the dice thrown is in Combat or not, for the dice statistics. (veqryn)</li>

  <li>- Getting engine to record which player is rolling dice for the dice statistics. (veqryn)</li>

  <li>- Adding scroll bars to edit place unit panel and non-tabbed purchase unit panel. (veqryn)</li>

  <li>- Fixing non-serialization error when attempting to save the game after a successful aa gun roll, but before selecting casualties. (veqryn)</li>

  <li>- Improved bombing result display to show ignored dice if there are any, and improving history panel to show the rolls for each target unit. (veqryn)</li>

  <li>- Fixed integer array error in Strategy Bombing with Heavy Bombers, causing the second half of all rolls to not be rolled, thereby defaulting to one each. (veqryn)</li>

  <li>- Fixed null pointer for undoing a placement made by UK in global 1940 maps, caused by the new no-air-checking delegate [players will need to update their 1940 maps though]. (veqryn)</li>

  <li>- Creating framework for TripleA to use proxies to connect to the internet. Allowing map downloading, PBEM/PBF, and dice servers to use a proxy. (veqryn)</li>

  <li>- Improving "Draw Territory Borders On Top" so that it will automatically switch to "medium" if you are on "low/default" and are zooming, and switch back once you stop zooming out. (veqryn)</li>

  <li>- Changing lobby moderator ban/mute options to make more sense, by only giving 3 options: name only, everything, or cancel. (veqryn) </li>

  <li>- Adding a backup lobby properties location on the tripleawarclub, in addition to the one on sourceforge. (veqryn)</li>

  <li>- Fixed null pointer error in MovePanel.selectEndPoint when clicking to move a unit to a territory with no connections. (veqryn)</li>


</ul><h3>Changes for 1.6.1.1</h3><ul>
  <li>- Fixing in loading old engine jars caused by odd pathnames. (veqryn)</li>

  <li>- Made AA Guns appear in battle, then disappear after firing if they could not participate any further. (veqryn)</li>

  <li>- Fixed bug causing stacked aa guns to all fire with the attack power of the most powerful aa gun in the group. (veqryn)</li>

  <li>- Fixed some math bugs in low luck picking of aa casualties for maps with non-standard aa guns. (veqryn)</li>

  <li>- Made massive updates to 1.5.2.1 and 1.6 so that they can work as 'old' jars and be run from 1.6.1.1 or future versions. (veqryn)</li>

  <li>- Disallowing starting of games if game data is null. (veqryn)</li>

  <li>- Allowing hosts to load an old savegame, causing old engine to join lobby and host directly, if they have the jar to run it. (veqryn)</li>

  <li>- Allowing members in online lobby to join games hosted by older versions of triplea, if they have the jar to run it. (veqryn)</li>

  <li>- Adding game version (GV), and engine version (EV), columns to lobby. (veqryn)</li>

  <li>- Fixing many bugs in the handling of command line arguments. (veqryn)</li>

  <li>- Adding Passworded (PW) column to lobby. (veqryn)</li>

  <li>- Making game notes non-modal (doesn't stop all action til closed) and making it always on top so that you can read it while you play. (veqryn)</li>

  <li>- Fixing movement validation to allow submarines that are transports to carry land units through other ships. (veqryn)</li>

  <li>- Forcing default map selection when TripleA starts to avoid the last file path uri used if it is not within the user's triplea folder or the program's folder. (veqryn)</li>

  <li>- Fixing bug with connections being lost during end of Air Battles, resulting in a game that can not continue. (veqryn)</li>

  <li>- Made xml exporter also add original territory owner as occupiedTerrOf until such a time as we can just use originalOwner. (veqryn)</li>

  <li>- Fixed bug causing land units carried by air units (paratroopers tech) to blitz unoccupied enemy territories on route if going behind enemy lines. (veqryn)</li>

  <li>- Fixing bug preventing renamed hardcoded techs from working properly. (veqryn)</li>

  <li>- Fixing some errors with Sliding Tiles game, Tic Tac Toe, and Kings Table. (veqryn)</li>

  <li>- Cleanup and abstraction of some AI classes and constructors and superclasses. (veqryn)</li>

  <li>- Fixed string index out of bounds error with notifications, and also forced them to shorten for the history event record, to 150 characters if needed by removing all html code then truncating the string. (veqryn)</li>

  <li>- Fixed issue with moving of old fighters to a new carrier by making sure it only used the producer territory. (veqryn)</li>

  <li>- Updating build to include old jars. Updating framework to ignore micro version numbers, so that 1.5.2.1 will also load 1.5.2.0 savegames, etc. (veqryn)</li>

  <li>- Created dialog to ask user if they want to load an old savegame.  Fixed framework so that it can load any old savegame if it can find an old engine to match. And added 1.6.0.0 jar engine. (veqryn)</li>

  <li>- Including old 1.5.2.1 jar file with slight modifications, so that 1.6.1.1 can play 1.5.2.1 savegames by simply running them with 1.5.2.1, but as a separate application. (veqryn)</li>

  <li>- Creating framework for loading older savegames using older included jar files. (veqryn)</li>

  <li>- Fixing some errors with command line options, and abstracting some game running utilities. (veqryn)</li>

  <li>- Fixing display error in old paratroopers tech that caused the land unit to appear to die with the air unit even after it has landed and survived any aa fire. (veqryn)</li>

  <li>- Making sure technology still has an effect even if it is not in a player's tech frontier. (veqryn)</li>

  <li>- Make sure the game chooser menu is cleared from memory after closed. (veqryn)</li>

  <li>- Created method to maintain savegame compatibility between 1.6.1 and 1.6.1.1 with regards to techs. (veqryn)</li>

  <li>- Removing static instances of all hardcoded Technologies. Everything now done with locally created instances per game data. (veqryn)</li>

  <li>- Changed choose how "best dice roll" / "LHTR heavy bombers" works with Low Luck on, so that it will add a bonus equal to the number of dice sides divided by 6. (veqryn)</li>

  <li>- Fixing scrambling again, so that even an amphibious assault on an undefended (blitzable) land territory, from an undefended sea zone, will still trigger scrambling. (veqryn)</li>

  <li>- Removed game stopping message about unlimited purchases, whenever a unit or item cost so little that you can buy more than 10000 of it. (veqryn)</li>

  <li>- Fixed errors in build.xml for java included version and mac version. (veqryn)</li>

  <li>- Fixed null pointer error in Dynamix AI. (veqryn)</li>

  <li>- Fixed bug in freePlacementCapacity when placing land units in a territory that previously placed sea units in a sea zone bordering more than one land producer. (veqryn)</li>

  <li>- Increasing max memory from 512mb to 640mb, and up to 768mb for online games. (veqryn)</li>


</ul><h3>Changes for 1.6.1</h3><ul>
  <li>- Rewriting build file and including META-INF, hopefully fixing issue with Gmail play-by-email emailer on linux machines. (rain)</li>

  <li>- Changing trigger property changes to use "-reset-" instead of clear. Can now be used with any attachment option. (veqryn)</li>

  <li>- Creating a reset method for every single attachment property. These can now be used to return a property to its default value. (veqryn)</li>

  <li>- Fixing some bugs introduced into AI with the factory switch. (veqryn)</li>

  <li>- Fixing null pointer error in Easy AI purchasing algorithm for getting costs of units. (veqryn)</li>

  <li>- Changing maxDamage to default to 2 instead of -1. This is for bombing type damage, and it acts as either a multiplier of territory value or as a hard set number depending on canProduceXUnits. (veqryn)</li>

  <li>- Fixing AIs to no longer use isFactory, and instead use things like canProduceUnits, etc. (veqryn)</li>

  <li>- Abstracting isFactory setting and matches to use the component parts. (veqryn)</li>

  <li>- Deleting unit attachment, "isFactory", but keeping the setter so that old xml's will not break. </li>
    setting isFactory now just sets: canBeDamaged, isInfrastructure, canProduceUnits, isConstruction, constructionType = "factory", maxConstructionsPerTypePerTerr = 1, constructionsPerTerrPerTypePerTurn = 1. (veqryn)

  <li>- Created new game option, "Submarines Prevent Unescorted Amphibious Assaults", that prevent unescorted transports from conducting amphibious assaults. (veqryn)</li>

  <li>- Created new game option, "Kamikaze Suicide Attacks Only Where Battles Are", and implemented it. (veqryn)</li>

  <li>- Fixed bug where land units would disappear when conquering a sea zone. (veqryn)</li>

  <li>- Making kamikaze and interceptor dialogs non-modal so user can move around map while choosing. Again, saving during the dialog then reloading might have odd effects. (veqryn)</li>

  <li>- Making scramble dialog non-modal so that the user can move the map around before choosing what to scramble. Note that saving the game while in the middle of scrambling can result in weird effects, so it is not recommended. (veqryn)</li>

  <li>- Undoing update to java Substance 7.1, in order to maintain compatibility with Java 5. (veqryn)</li>

  <li>- Created edit option to change the amount of unit bombing damage on any and all units which can be damaged by bombing. (veqryn)</li>

  <li>- Created edit option to change the amount of unit hitpoint damage on any and all units which can take more than 1 point of hit damage. (veqryn)</li>

  <li>- Created edit option to remove technology from a player, except that shipyards and industrial technology can never be removed, and any technology that uses triggers is pointless to remove and removing will not undo their effect. (veqryn)</li>

  <li>- Created edit option to add technology to a player. (veqryn)</li>

  <li>- Adding methods to ensure that any power sharing technology (like British to UK Pacific) will still roll for war bonds even if its capital is taken, so long as the shared power is not able to have the warbonds technologies. (veqryn)</li>

  <li>- Allowing additional nations to share the cost of technology, and creating a good user interface that dynamically adjusts to show how much is being paid by each nation. (veqryn)</li>

  <li>- Created an option in Play-By-Forum and Play-By-Email to send the move summary after the combat move phase, in addition to the summary at the end of the turn. This is to help with OOL and scrambling orders. (veqryn)</li>

  <li>- Abstracted EndTurnPanel into AbstractForumPosterPanel, then created MoveForumPosterPanel. (veqryn)</li>

  <li>- Created new game option, "Remove All Tech Tokens At End Of Turn", which will remove tech tokens after each tech roll. (veqryn)</li>

  <li>- Make savegames for long games, games with many players, and games with many battles, much smaller. (veqryn)</li>

  <li>- Changing how Battle Records get added and removed from game data through the Change Factory to be more memory efficient. (veqryn)</li>

  <li>- Adding an option for "None" to the list of territory effects. (veqryn)</li>

  <li>- Added List to Battle Calc so that you can manually select one or more territory effects, hold down shift to select more than one. List will automatically fill with starting territory's effects. (veqryn)</li>

  <li>- Fixed battle calc to make it try to use the territory that we select. (veqryn)</li>

  <li>- Fixing bug in Battle Calculator where damaged units got turned into healthy units before each battle was calculated. (veqryn)</li>

  <li>- Fixed null pointer error in triggerSupportChange caused by having a hashmap of an attachment class, inside of another attachment class, then deserializing this (loading a savegame), resulting in the hashmap being resolved before all its keys are, giving the wrong hashcodes to those keys. (veqryn)</li>

  <li>- Updating java Substance to 7.1, and adding 14 more skins. (veqryn)</li>

  <li>- Updated embedded Java JRE for windows executable version to Java 6 update 33. (veqryn)</li>

  <li>- Added a drawing method and menu option to have territory borders drawn a second time on top of the map. (veqryn)</li>

  <li>- Changing IDrawable calls to use highest level of graphics rendering available. (veqryn)</li>

  <li>- Fixing game selector model to no longer return to default game if we have trouble loading the uri of previous xml, and will instead try to pick by name first. (veqryn)</li>

  <li>- Added new sounds for air, sea, and land battles, rockets, politics, and tech. (veqryn)</li>

  <li>- Fixed issue where fighters moving alone were not asked if they want to escort. (veqryn)</li>

  <li>- Made DefaultAttachment extend GameDataComponent. (veqryn)</li>


</ul><h3>Changes for 1.6</h3><ul>
  <li>- Fixing Global 1940 bugs, and getting it to use Technology completely. (veqryn)</li>

  <li>- Allowed downloading of multiple maps/games in one go, by holding down CTRL while selecting maps in the "Download Games" dialog screen, and out of date maps will show up in bold, and maps up-to-date will show in italics. (ddurham)</li>

  <li>- Created new rules attachment option, "switch", which allows either "true" or "false", thereby giving all conditions a memory function. (veqryn)</li>

  <li>- Fixed bug where dependents of an air transport were not dying when the air transport was hit by AA fire, in the case where the air transports could fly deep into enemy territory and flew over an AA gun. (veqryn)</li>

  <li>- Fixed parsing error in player attachment options: placementLimit, movementLimit, attackingLimit. (veqryn)</li>

  <li>- Fixed fatal error in HistoryLog, caused by clearing an array that potentially gets accessed later at a specific index number, from doing an edit during a movement phase then doing an undo later. (veqryn)</li>

  <li>- Created new game option, "Subs Can End NonCombat Move With Enemies", which allows submarines to end their noncombat movement in a sea zone containing any enemy units. (veqryn)</li>

  <li>- Added information on which units are doing the bomber to the question about what should each bomber bomb. (veqryn)</li>

  <li>- Fixed error from trying to undo a battle move created using another player's units, using edit mode. (veqryn)</li>

  <li>- Fixed null pointer exception when not selecting the target for a bomber after an air battle is finished. (veqryn)</li>

  <li>- Allowed interceptors and escorts to benefit from attackRolls and defenseRolls and their bonuses. (veqryn)</li>

  <li>- Created new delegate, NoAirCheckPlaceDelegate, which does everything the normal "PlaceDelegate" does, but does not kill any aircraft at the end of the phase. (veqryn)</li>

  <li>- Fixed issue with not being able to blitz through units owned by a power to which you were neutral with. (veqryn)</li>

  <li>- Allowed loading of transports in Sea Zones where all enemies just became hostile this turn due to politics. (veqryn)</li>

  <li>- Fixed issue with loading transports in the same sea zone where a transport was previously unload in a previous phase. (veqryn)</li>

  <li>- Fixed issue with having multiple support attachment affecting the same group of units. The order of preference is now: highest bonus support first, then lowest number of supported types to highest number of types. (veqryn)</li>

  <li>- Created new techAbilityAttachment option, "bombingBonus", which will add additional damage after all dice are rolled, per unit. (veqryn)</li>

  <li>- Created new techAbilityAttachment option, "defenseRollsBonus", which adds additional defense rolls. (veqryn)</li>

  <li>- Created new techAbilityAttachment option, "attackRollsBonus", which adds additional attack rolls. (veqryn)</li>

  <li>- Created new UnitAttachment option, "chooseBestRoll", which controls whether we select the best dice or use all the dice rolled, when there is more than one die rolled. (veqryn)</li>

  <li>- Created new UnitAttachment option, "defenseRolls", which controls the number of defense rolls a unit has, so long as their defense is greater than zero. (veqryn)</li>

  <li>- Created new UnitAttachment option, "attackRolls", which controls the number of attack rolls a unit has, so long as their attack is greater than zero. (veqryn)</li>

  <li>- Abstracted Heavy Bombers technology. (veqryn)</li>

  <li>- Changed History Writer setRenderData to be part of a new event, instead of being a separate method. Also fixed some display issues with event and child messages. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "airborneTargettedByAA", which is set by the attacker, controlling which airborne units are subject to AA gun fire and by what AA gun types. (veqryn)</li>

  <li>- Fixing error message for when a game xml is not correctly formed. Also preventing errors from being thrown until we check the version number. (veqryn)</li>

  <li>- Deleted "GivesPUsDelegate". (veqryn)</li>

  <li>- Finished airborne movement delegate, and technology. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "airborneBases", which turns on the new airborne tech. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "airborneDistance", which turns on the new airborne tech. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "airborneTypes", which turns on the new airborne tech. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "airborneCapacity", which turns on the new airborne tech. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "airborneForces", which turns on the new airborne tech. (veqryn)</li>

  <li>- Created new game option, "Airborne Attacks Only In Enemy Territories", to help control different behavior for airborne tech. (veqryn)</li>

  <li>- Created new game option, "Airborne Attacks Only In Existing Battles", to help control different behavior for airborne tech. (veqryn)</li>

  <li>- Created Validation for Airborne movement. (veqryn)</li>

  <li>- Created AbstractMoveDelegate and abstracted MoveDelegate into it.  Created SpecialMoveDelegate to extend it, for use with new Paratroopers/Airborne tech. (veqryn)</li>

  <li>- Fixed error preventing AI Flat Income Bonus from happening unless the Percentage Bonus was also set. (veqryn)</li>

  <li>- Fixed repair panel to correctly set the max for each unit. (veqryn)</li>

  <li>- Fixed error with displaying discounts for repairing. Also fixed that you may not be able to repair with all your money if you had a discount. (veqryn)</li>

  <li>- Fixed null pointer error from having Edit Mode on while AA guns fire. (veqryn)</li>

  <li>- Started coding for new paratrooper tech, to be called Airborne Forces. (veqryn)</li>

  <li>- Fixed blockade zones so that they never do more damage than the combined total of their neighboring territories, even if there are multiple sea zones blockading a single or set of territories. (veqryn)</li>

  <li>- Allowed createsResourcesList to have negative values as well as positive values. (veqryn)</li>

  <li>- Created new Unit Attachment option, "bombingTargets", which allows the unit to only target specific other units for rockets and strategic bombing. (veqryn)</li>

  <li>- Disallowed Bombardment from any sea zone that had a kamikaze suicide attack. (veqryn)</li>

  <li>- Fixed failing unit tests. (veqryn)</li>

  <li>- Expanded Tech delegate UI element to use helpPayTechCost. (veqryn)</li>

  <li>- Created new PlayerAttachment option, "helpPayTechCost", which will allow other players to help pay the cost of technology. (veqryn)</li>

  <li>- Created new PlayerAttachment option, "shareTechnology", which will automatically give all technology to other players during tech activation phase. (veqryn)</li>

  <li>- Changed priority of AA casualty choosing system to: chooseAACasualties -> isRollAAIndividually -> isRandomAACasualties. This means that "choose aa" overrides all, while "roll aa individually" will only override "random aa". (veqryn)</li>

  <li>- Allowed "unitAbilitiesGained" to give "canBlitz" and "canBombard". (veqryn)</li>

  <li>- Created new techAbilityAttachment, "unitAbilitiesGained", which allows units to gain abilities when technology is discovered. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "rocketNumberPerTerritory", which controls the maximum number of dice to be rolled per territory. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "rocketDistance", which controls the maximum distance rockets can travel. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "rocketDiceNumber", which controls the number of dice each rocket rolls. (veqryn)</li>

  <li>- Created new RelationshipTypeAttachment option, "rocketsCanFlyOver", which allows rockets to fly over by default. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "warBondDiceNumber", which controls how many dice get rolled for war bonds. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "warBondDiceSides", which controls how large the dice are which are rolled to determine the war bonds bonus. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "repairDiscount", which controls the discount to repairing given by any technology. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "minimumTerritoryValueForProductionBonus", which controls the minimum value of a territory that a factory units must be in to receive the production bonus. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "productionBonus", which controls the bonus given to production by any technology. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "airDefenseBonus", which controls the bonus given to interceptors defense by any technology. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "airAttackBonus", which controls the bonus given to escorts attack by any technology. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "radarBonus", which controls the bonus to radar AA attack given by any technology. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "defenseBonus", which controls the defense bonus given by any technology. (veqryn)</li>

  <li>- Created new techAbilityAttachment, "attackBonus", which controls the attack bonus given by any technology. (veqryn)</li>

  <li>- Fixed error with "Should not be adding battle record for player ...", which was caused by creating a battle using edit mode for a player who's turn has passed already. (veqryn)</li>

  <li>- Fixed error with Low Luck AA guns when the dice side is different than 6. Was trying to roll zero random dice. (veqryn)</li>

  <li>- Fixed issue with not being able to move through submarines during noncombat if they were on top of convoy zones. (veqryn)</li>

  <li>- Created new game option, "Convoy Blockades Roll Dice For Cost", which will now allow dice to be thrown for all blockade damage. (veqryn)</li>

  <li>- Allowed multiple airbases in a single territory to stack for their max scrambling number total. (veqryn)</li>

  <li>- Allowed defenseless attackers to be able to retreat if they can, instead of being forced to die. (veqryn)</li>

  <li>- Possible fix for "Record Battle Statistics" occuring multiple times. (veqryn)</li>

  <li>- Allowed all defending or attacking units to die, when there are none left who are capable of throwing dice. (veqryn)</li>

  <li>- Fixed issue with maxScrambleCount not keeping track of scrambles for different sea zones by the same land territory. (veqryn)</li>

  <li>- Semi-Fixed issue with not being able to retreat from a scrambled air defense. You can now retreat anywhere that does not have enemies. User should know where they came from and make legal move. (veqryn) </li>

  <li>- Fixed issue with unloaded ground units not dying or being removed, even if their transports die from a scrambled air defense. (veqryn)</li>

  <li>- Disallowed any unloading of ground units to a friendly territory, during combat move, if we have scrambling or kamikazes turned on. (veqryn)</li>

  <li>- Fixed issue with "Scramble To Any Amphibious Assault" not working at all. (veqryn)</li>

  <li>- Created new game option, "Use Bombing Max Dice Sides And Bonus", which will control the unit attachment options: "bombingMaxDieSides" and "bombingBonus". (veqryn)</li>

  <li>- Stopped "Low Luck for Bombing and Territory Damage" from controlling "bombingMaxDieSides" and "bombingBonus", and made it create a Low Luck situation on top of whatever dice sides and bonus the map uses. (veqryn)</li>

  <li>- Fixing comparison method in weak ai. (veqryn)</li>

  <li>- Allowed users to download maps even if they come with triplea. (veqryn) </li>

  <li>- Fixed Null pointer errors in Turn Summary Poster, and also fixed up Politics to display better in the turn summary with indents. Also stopped the poster from showing certain things like: game loaded, recording battle statistics, and giving bonus movement. (veqryn)</li>

  <li>- Fixed a ton of lock not held errors that had resulted from new technology code. (veqryn)</li>

  <li>- Fixed Economy panel so that it would change when you click back through history. (tao nie)</li>

  <li>- Created new techAbilityAttachment, "movementBonus", which controls the bonus to movement that is received from any technology. Also created default attachment for Long Range Air, which will now be set to give +2 movement to all air units, that are air units at the start of the game. (veqryn)</li>

  <li>- Created framework for interpreting TechAbilityAttachment's, and also setting of default attachments for hardcoded technologies. (veqryn) </li>

  <li>- Created new type of attachment, TechAbilityAttachment, which will control how all technologies work. (veqryn)</li>

  <li>- Refactored TechAdvance and GenericTechAdvance to extend NamedAttachable, that way they can eventually have attachments. (veqryn)</li>

  <li>- Fixed bug where a NonFighting battle was attempting to add the result as a child in the history panel, without creating the event first. (veqryn)</li>

  <li>- Fixed bug preventing Moore AI from placing Transport type sea units whenever it did not buy non-transport sea units. (veqryn)</li>

  <li>- Clearing all cached data for AIs once a game has been left. (veqryn)</li>

  <li>- Clearing cached data for Dynamix AI once a game has been left. (frigoref)</li>

  <li>- Fixed issue with battles showing who won twice in the history panel. (veqryn)</li>

  <li>- Moved BattleRecord to its own class, and having BattleRecord, BattleRecords, and BattleResults all extend GameDataComponent. (veqryn)</li>

  <li>- Possibly fixed the problems with Edit Mode, by fixing a previous refactoring that switched two variables up. (veqryn)</li>

  <li>- Possibly fixed the problems with Edit Mode, by abstracting BasePersistentDelegate and separating EditDelegate from BaseDelegate. (veqryn)</li>

  <li>- Generating Serial IDs for all classes that may need them. (veqryn)</li>


</ul><h3>Changes for 1.5.2.1</h3><ul>
  <li>- Updated 1940 test xml to allow Axis powers to declare war on Americans separately, and for Americans to declare war on each Axis power separately. (veqryn)</li>

  <li>- Fixed null pointer error in Dynamix AI's determining of where to put a factory. (veqryn)</li>

  <li>- Having the default loaded game be loaded separately from the game chooser list, and putting the loading of the list into a separate thread. (veqryn & frigoref)</li>

  <li>- Removing game chooser list from memory when we start a game, or join a game, or join the lobby. (veqryn & frigoref)</li>

  <li>- Removed restriction of not being able to land in land territories with pending battles (there is still a restriction of course on who owns the territory, and whether it was conquered this turn or not). (veqryn) </li>

  <li>- Fixing possible error with using overriden placement delegates that were not triplea placement delegates, like using twoIfBySea place delegates. (frigoref)</li>

  <li>- Fixing bug where a territory that was taken without a fight, could still trigger a scrambling, with the wrong player selecting who scrambles. (veqryn)</li>

  <li>- Allowing air to end their movement over sea zones containing enemy units, if you own or will place a carrier there. (veqryn)</li>

  <li>- Disallowing new usernames for lobby if they match case insensitive an existing user, instead of checking only case sensitive. (veqryn)</li>

  <li>- Speeding up lobby login process. (frigoref & veqryn)</li>

  <li>- More fixes for sea placement and requiresUnits placement. (veqryn)</li>

  <li>- Prevented units with "requiresUnits" from being placed by territories not containing the required units, and also prevented them from being moved around by the "free-up-space" methods. (veqryn)</li>

  <li>- Fixed many small rare bugs in AbstractPlaceDelegate. (veqryn)</li>

  <li>- Changing look of main screen, and adding tool tips for all buttons. (veqryn)</li>

  <li>- Fixed possible Null Pointer error for maps with a production frontier of null rules. (veqryn)</li>

  <li>- Fixed possible IllegalStateException in Air Battles. (veqryn)</li>

  <li>- Allowed "Edit Moving" of units not owned by you, to create a battle by the unit's owner. (veqryn)</li>

  <li>- Fixed 'uses' for 'when' based triggers to be used up right after they are used, while triggers without when set get 'used up' at the end of each round that they are used in. (veqryn)</li>

  <li>- Fixed Air Battle to only allow aircraft capable of intercepting into the battle, instead of also allowing infrastructure too. (veqryn)</li>


</ul><h3>Changes for 1.5.2</h3><ul>
  <li>- Fixed infinite loop in getAllProducers for a sea placement. (veqryn)</li>

  <li>- Removing BattleResults from BattleRecord until we figure out the problem (probably non Serializable) with it always causing the BattleRecordsList to be null. (veqryn) </li>

  <li>- Moved all AI related code to new package. (veqryn)</li>

  <li>- Fixing the bugs introduced into the engine, and the failing unit tests due to changes in how battles were abstracted, and how they are now recorded when finished. (veqryn)</li>

  <li>- Created new type of battle, FinishedBattle (scripted), to handle blitzed and conquered territories. (veqryn)</li>

  <li>- Created new Rules Attachment and Condition Attachment option, "battle", which can be used to test for the presence of battles. (veqryn)</li>

  <li>- Major abstraction and cleanup of all battle related classes. (veqryn)</li>

  <li>- Fixing bad comparisons, and fixing missing hashCode methods. (veqryn)</li>

  <li>- Forced user preferences for individual sound muting choices to be saved by each local vm. (veqryn)</li>

  <li>- Allowed individual sounds to be muted, and separated simple Messenging from Slapping with different sounds for each. (frigoref)</li>

  <li>- Rewrote the framework for how sounds are loaded and played, in order to allow more flexible expansion of sound options. Moved sound files to separate user visible folder. (frigoref)</li>

  <li>- Temporary hack fix for bug where client computer can not use paratroopers at all, but hosts can. (veqryn)</li>

  <li>- Finalizing Alpha rules for test xml. (veqryn)</li>

  <li>- Improving in-game Help -> Movement/Selecting Help menu tips. (veqryn)</li>

  <li>- Holding down ALT key while selecting or deselecting units will now add/remove 10 units at a time. (veqryn)</li>

  <li>- Possible fix for battle window disappearing after closing, with battle panel not becoming visible again. (frigoref)</li>

  <li>- Abstraction of ClientGame and ServerGame into AbstractGame. (frigoref)</li>

  <li>- Deleting duplicate m_bridge variables that were hiding the real m_bridge variables of the extended classes. (veqryn)</li>

  <li>- Maintaining compatibility with Java 5. (veqryn)</li>

  <li>- Abstraction of Launcher code to an abstract class. (frigoref)</li>

  <li>- Fixed bug where sea placement could be done in territories captured this turn. (veqryn)</li>

  <li>- Fixed bug with bid placement of sea units, which was previously not allowing them to be placed anywhere at all. (veqryn)</li>

  <li>- Changed Battle Calculator to only count units that can die in combat, in the unit totals. No longer counts AA Guns or other units like Factories, in the unit totals, even if they are present. (veqryn)</li>

  <li>- Fixed infinite loop in Dynamix combat calculation routine, resulting from thinking battles that were lost were really won, then increasing the number of defenders to try to reach a "losing" battle, except that no losing battle ever came. (veqryn)</li>

  <li>- Preventing Dyanmix AI from purchasing any infrastructure or maxBuiltPerPlayer units. (veqryn)</li>

  <li>- Reduced calls to find map resource paths to a single time, when the map is first loaded. Should speed things up a little. (veqryn)</li>

  <li>- Fixed TripleA to ignore if the user has multiple folders with the same name in both of the "maps" directories that it reads from. TripleA will pick first from the user's maps folder, and pick second from the program's folder. (veqryn)</li>

  <li>- Fixed failing unit tests. (veqryn)</li>

  <li>- Fixed bug where if a defender wins a battle in a seazone, but has aircraft that can not land anymore, the aircraft had to choose right away where they wanted to land, forbidding landing in a territory with a pending battle. </li>
  Now fixed so that all these air wait til end of battle phase to ask where to move. (veqryn) 

  <li>- Fixed bug where aircraft + destroyer attacking a submarine, if the submarine kills the destroyer, the submarine may not yet submerge but should be allowed to submerge. (veqryn)</li>

  <li>- Fixed bug where if the defender only has subs left, and submerges them, the attacker can still retreat, but should not be able to. (veqryn)</li>

  <li>- Fixed bug where units unloaded from a sea zone with enemy units, to a friendly territory, would not die when the sea transports died. Fixed by making such moves illegal, forcing user to wait til after combat is resolved to offload. (veqryn)</li>

  <li>- Fixed bug in new Sea Placement code that incorrectly validated how many could be placed, and incorrectly switched placements to the wrong territory. (veqryn)</li>

  <li>- Fixing "Not in an event, but trying to add child" error for placing a carrier and moving fighters to be on it. (veqryn)</li>

  <li>- Fixing email/forum turn summary poster to use <pre> and </pre> tags, instead of &nbsp. (veqryn)</li>

  <li>- Fixed null pointer error in BattleRecordsList getTUVdamageCausedByPlayer. (veqryn)</li>


</ul><h3>Changes for 1.5.1</h3><ul>
  <li>- A second possible fix for ConcurrentModificationException in BattleModel.refresh -> DiceRoll.isAmphibiousMarine -> BattleTracker.getPendingBattleSites. (veqryn)</li>

  <li>- Changed Sea Placements to use all production for all surrounding Factories, if multiple factories touch that sea zone. Will now dynamically shift the production of other sea units away to other legal factories in order to allow the maximum production possible. (frigoref & veqryn)</li>

  <li>- Fixed null pointer error in trying to place a construction to a sea zone. (veqryn)</li>

  <li>- Locking the map when user's mouse is over the history panel, and then unlocking for each click on a history node. (frigoref) [edit: this is undone/rolled-back for now, pending finding a better way to lock/unlock a user's interface without writing to the cache/registry each time] </li>

  <li>- Fixed bug where Rounds would not appear in a Client game. (veqryn)</li>

  <li>- Creating a NullModeratorController class for locally hosted games. (veqryn)</li>

  <li>- Fixed bug where steps appear out of order in a client game's history panel. (frigoref)</li>

  <li>- Created new Trigger Attachment option, changeOwnership, which will allow a map to have the owner of a territory change by trigger. (veqryn)</li>

  <li>- For Trigger Attachment option "removeUnits", now allowing the use of "all" in place of the territory name, and also "all" in place of the unit type. Can be used to remove all units from some or all territories. (veqryn)</li>

  <li>- Correcting politics for Alpha xml. (veqryn)</li>

  <li>- Changing game property, Selectable Tech Roll, to also work with WW2V3 Tech Model, allowing the user to select which tech they want after a successful roll. Also fixed the dice chooser to let you set the sides. (veqryn)</li>

  <li>- Fixing bugs in new air movement validation, and improving speed and efficiency. (veqryn)</li>

  <li>- Completely rewrote the validation of air unit movement, and moved it to a new class, AirMovementValidator.java (veqryn)</li>

  <li>- More work on rewriting MoveValidation of air units. (veqryn)</li>

  <li>- Allowed for the use of the Arrow Keys for navigating around the map. (frigoref)</li>

  <li>- Adding [Mod] tags onto the names of any Admins in the online lobby. (veqryn)</li>

  <li>- Possibly correcting some hidden bugs in MoveValidator. (veqryn)</li>

  <li>- Created new CanalAttachment option, excludedUnits, which allows the specifying of specific units which will not be validated for. (veqryn)</li>

  <li>- Created new RelationshipTypeAttachment option, canMoveThroughCanals, which allows a player to move through a canal owned by the other player. (veqryn)</li>

  <li>- Removed restrictions that had canals only checked for Sea Movement. They now check for all movement, and therefore there can now be 'land' canals that require sea zones, or land requiring other land, or sea requiring sea, etc. (veqryn)</li>

  <li>- Creating a better error message for when users do not have a map, but try to join the game anyway. (frigoref)</li>

  <li>- Getting history panel to stop closing clicked on expanded paths every time a there is a new event or change, when your mouse is over the history panel. (frigoref)</li>

  <li>- Correcting bad history log messages for Edit mode. (veqryn)</li>

  <li>- Refactored Trigger Attachment class again to allow triggers to fire other triggers with certain options and properties. (veqryn)</li>

  <li>- Created new Trigger Attachment option, activateTrigger, which will allow a trigger to fire other triggers. (veqryn)</li>

  <li>- Preliminary work on ability to fire triggers from other triggers. (veqryn)</li>

  <li>- Fixing NoSuchElementException in Kamikaze attack ui. (veqryn)</li>

  <li>- Created new RelationshipTypeAttachment option, canMoveIntoDuringCombatMove, which stops combat-phase movement, but allows non-combat-phase movement. (veqryn)</li>

  <li>- Fixing Chat Panel player name area to be correct size to hold all player names and national flags. (frigoref)</li>

  <li>- Adding Alpha+3 National Objectives to xml. (veqryn)</li>

  <li>- Added "originalNoWater" as an option for conditions that test territories. (veqryn)</li>

  <li>- Fixed bug where paratroopers could not move over enemy sea zones or captured sea zones. (veqryn)</li>

  <li>- Fixed bug with moving sea units through sea units belonging to a power not yet at war with. Also possibly fixed bug with Easy AI's comparison method contract. (veqryn)</li>

  <li>- Adding Global 1940 alpha 3 as test xml. (veqryn)</li>

  <li>- Fixing bug where the neutral (null) player might be asked if it wants to scramble, which gives an error. (veqryn)</li>

  <li>- Adding Play-By-Forum method for TripleA War Club, http://www.tripleawarclub.org/  so that people can also play there. (qwertgold)</li>

  <li>- Fixing Battle Calc to not include units that are irrelevant to combat. (veqryn)</li>

  <li>- Made sure all m_variable types in attachments exactly match the new instance type that is used. This, combined with the previous 2 changes, should fix the history panel bugs that are being caused by not being able to find the correct setter. (veqryn)</li>

  <li>- Changing the way the ChangeFactory uses PropertyUtil for getting the old value of properties. Previously relied on the "get" method for getting the old value. Now it will directly access and store the "m_" object. getRawProperty no longer used. (veqryn)</li>

  <li>- Allowed changes to all attachments to be undone and redone in the history panel, by ensuring each setter has an additional setter for an object of the field's type. (veqryn)</li>

  <li>- Preventing history panel from updating if moused over, and allowing it to scroll down if not. (frigoref & veqryn)</li>

  <li>- Allowing route to recalculate if only air can make it. (frigoref)</li>

  <li>- More optimizations of getBestRoute. Also changing "Parse Selected" to be default parsing strategy of maps. (veqryn)</li>

  <li>- Changing getBestRoute to not use territories for which the owner's relationship with us does not allow us to pass. (veqryn)</li>

  <li>- Fixing getBestRoute to never use impassible and restricted territories. (veqryn)</li>

  <li>- Adding Global 1940 as test xml. (veqryn)</li>

  <li>- Fixing weird tech attachment getters to use booleans rather than strings. (veqryn)</li>

  <li>- Making sure that all attachment variables that start out as Null, can return to being null again through their setter. (veqryn)</li>

  <li>- Fixing various errors introduced into casualty selection. (veqryn)</li>

  <li>- Fixed null pointer error for players who have damaged units but no repair frontier. (veqryn)</li>

  <li>- Adding Europe 1940 as test xml. (veqryn)</li>

  <li>- Fixed more "Lock not held" errors, and a potential null pointer in the battle calculator. (veqryn)</li>

  <li>- Possible fix for ConcurrentModificationException in BattleModel.refresh -> DiceRoll.isAmphibiousMarine -> BattleTracker.getPendingBattleSites. (veqryn)</li>

  <li>- Fixing bug with displaying up total resources when more than one unit creates resources. (veqryn)</li>

  <li>- Allowed users to use Edit Mode to create new units for normal players, based on both their production frontier and any units they have on the board. (veqryn)</li>

  <li>- Allowing users to use Edit Mode to create and place new "Neutral" (null player) units, but only selecting from ones on the board. (veqryn)</li>

  <li>- Allowing users to Battle Calc against any "Neutral" (null player) units that are still on the board. (veqryn)</li>

  <li>- Fixing casting error bug introduced into battle calc. (veqryn)</li>

  <li>- Changing airfields and harbours to stop being operational at 3 damage, instead of 4. (veqryn)</li>

  <li>- Fixed bug where you were not allowed zero (0) for the unitPresence count. (veqryn)</li>

  <li>- Making the check to see if you can do the purchase phase, the same for both humans and AIs. (veqryn)</li>

  <li>- Fixed null pointer error for when a player runs low on resources. (veqryn)</li>

  <li>- Fixing a couple "Lock not held" errors. (veqryn)</li>

  <li>- Fixed the Battle Calculator not displaying combat units with 'AA' abilities. (veqryn)</li>

  <li>- Fixed the "Cant add an event, not a step" bug for adding AddBattleRecordsChange. (veqryn)</li>

  <li>- Fixed bug with Air Battles where there were more hits than aircraft. (veqryn)</li>


</ul><h3>Changes for 1.5</h3><ul>
  <li>- Adding new Game-Play manual. (victor, veqryn, hepster)</li>

  <li>- Fixing build xml to export new docs. (veqryn)</li>

  <li>- Fixed major bug with new Delayed parsing method, it will now correctly handle maps with errors in them by removing them from the game chooser list. (veqryn)</li>

  <li>- Creating better error messages for setting attachment options in xmls. (veqryn)</li>

  <li>- Fixing bug where suicide attack units could target units in transports. (veqryn)</li>

  <li>- Some major bug fixes to movement with paratroopers, including not allowing units with multiple movement to move through all enemies once you get paratroopers. (veqryn)</li>

  <li>- Created new game option, "Paratroopers Can Attack Deep Into Enemy Territory", which will allow movement for air transports during combat move over enemy territories. (veqryn)</li>

  <li>- Deleted Player Attachment stackingLimit and replaced with movementLimit, attackingLimit, and placementLimit. (veqryn)</li>

  <li>- Deleted Unit Attachment stackingLimit and replaced with movementLimit, attackingLimit, and placementLimit. (veqryn)</li>

  <li>- Fixing potential bugs with new .equals for all attachments. (veqryn)</li>

  <li>- Disabled political action button when taking actions, to prevent taking multiple actions while waiting for confirmation of the first. (veqryn)</li>

  <li>- Fixed major error preventing politics from working over the network, due to the new way condition testing works. (veqryn)</li>

  <li>- Fixed Lock not held errors for politics. (veqryn)</li>

  <li>- Changed political panel to use a split panel, and added the one-touch-expandable feature to all main game screen panels: map panel, chat panel, and history panel. (veqryn)</li>

  <li>- Added scroll bars to main screen player selection area. (frigoref)</li>

  <li>- Created option to have TripleA not parse every single xml at startup, and only parse as each game is selected. (veqryn & frigoref)</li>

  <li>- Added new button to main screen, Engine Preferences, which lets a user select various properties specific to the the triplea engine, like setting the look and feel, etc. (veqryn)</li>

  <li>- Added scroll bars to both political overview and political action screens. (veqryn)</li>

  <li>- Fixed serious bug in DefaultAttachment.getRawProperty() and getFieldIncludingFromSuperClasses, and also updated attachment/annotation test to search super's fields. (veqryn) </li>

  <li>- Making some small fixes to attachment/annotation test, and renaming any methods with attach to attach. (veqryn)</li>

  <li>- Added wait window to TripleA's startup. (frigoref)</li>

  <li>- Changed name of Dynamix to be Land-Only AI, at least until someone decides to start working on the AI again. (veqryn)</li>

  <li>- Completely updated the game xml exporter to TripleA 1.5, except that attachments are just copies of what was parsed from the xml originally. (veqryn)</li>

  <li>- Fixed null pointer error in Bid Placement when undoing a placement. (veqryn)</li>

  <li>- Created new Player Attachment property, stackingLimit, which allows stacking limits to be enforced flexibly per player, with multiple rules allowed for owned, allied, and total units. (veqryn)</li>

  <li>- Created new Rules Attachment property, players, which can be used with directOwnershipTerritories, directExclusionTerritories, directPresenceTerritories, or any of the other territory lists, to customize which players are required to own/occupy the territories. (veqryn)</li>

  <li>- Fixing new attachment setter annotation tester, and renaming some isXX methods to getXX. (veqryn)</li>

  <li>- Fixing a unit test by removing static instances from messenger classes. (qwertgold)</li>

  <li>- Adding @InternalDoNotExport or @GameProperty onto all setter methods in all attachments, and also unit and tripleaunit. (veqryn)</li>

  <li>- Creating annotations to be used for tracking and marking various setters for attachments and other game data. (qwertgold & veqryn)</li>

  <li>- Changing how attachments are created by the game parser. (frigoref & veqryn)</li>

  <li>- Changing build.xml and editing a test suite to ignore certain tests for the time being.  Also setting svn to ignore 'classes.jar', 'fb.xml', and 'TEST-games.strategy.AllTests.txt/xml'. (qwertgold)</li>

  <li>- Adding findbugs folder for use with ANT. (qwertgold)</li>

  <li>- Creation of new xml entry, <triplea minimumVersion="1.5"/>, which should be used by ALL new maps. If an older TripleA tries to play a map built for a newer TripleA, then it will simply ignore the map instead of throwing tons of java errors at the user. (veqryn)</li>

  <li>- Complete rewrite of AxisAndAllies.org forum poster. Also added help html pages for the pbem / pbf system. (qwertgold)</li>

  <li>- Creating some unit tests for purchasing with multiple resources. (edwin van der wal)</li>

  <li>- Adding folders for future resources images, and filling with some general images. (veqryn, hepster, rofl)</li>

  <li>- Finished phase 5 of refactoring of aaGuns, separating isAAforFlyOverOnly from isAAforCombatOnly, and creation of an option to force attacks at the end of a movement, and allowing attacks to be filtered based on accompanying units, thereby finally reaching compatibility with silly pacific rules. (veqryn)</li>

  <li>- Created new game option, "Force AA Attacks For Last Step Of Fly Over", which will force isAAforFlyOver to shoot for the last step of a route, which it normally does not. (veqryn)</li>

  <li>- Created new Unit Attachment, "willNotFireIfPresent", which will be used to prevent an AA unit from firing at all if the enemy has any of a list of units in the battle. (veqryn)</li>

  <li>- Created new Unit Attachment, "isAAforFlyOverOnly", which will be used to determine if there are any AA shots for units passing through a territory. (veqryn)</li>

  <li>- Finished phase 4 of refactoring of aaGuns, by allowing aaGuns to stack, overstack, and getting maxAAattacks to work, thereby allowing aaGuns to shoot a limited number of times instead of infinite. (veqryn) </li>

  <li>- Created new Unit Attachment, "mayOverStackAA", which will be used to allow more AA shots than the total number of aircraft/targets. (veqryn)</li>

  <li>- Created new Unit Attachment, "maxAAattacks", which will determine the maximum number of times an AA gun will be allowed to fire per round. (veqryn)</li>

  <li>- Finished phase 3 of refactoring of aaGuns, by removing the artificial constraints placed on AA guns and allowing them to operate flexibly, targeting different kinds of units, and having multiple groups of aa guns firing separately. (veqryn)</li>

  <li>- Created new Unit Attachment, "targetsAA", which determines what units may be hit by the AA fire of a unit. Defaults to all air units. (veqryn)</li>

  <li>- Created new Unit Attachment, "typeAA", which determines which 'group' an AA unit belongs to.  Each group gets to fire once, and only 1 unit in each group may fire. (veqryn)</li>

  <li>- Fixed bug in Anti Aircraft low luck where engine ignored attackAAmaxDieSides completely. (veqryn)</li>

  <li>- Finished phase 2 of refactoring of aaGuns, by removing internal references and variables for isAA for rockets, capturing, and aa for bombing and for combat. (veqryn)</li>

  <li>- Finished phase 1 of refactoring of aaGuns, by removing isAAmovement and removing isAA from dealing with any aspect of movement validation and stacking limits in the engine. Both isAAmovement and isAA just call the two new methods below when they are created. (veqryn)</li>

  <li>- Created two new Unit Attachment options, "canNotMoveDuringCombatMove" and "stackingLimit", which will take the place of previous isAA and isAAmovement abilities while making them more flexible. (veqryn)</li>

  <li>- Allowed for Dice Skins, which can be placed in the "dice" folder of a map's directory. (crystalct & veqryn)</li>

  <li>- Created new player attachment, suicideAttackTargets, which lets you set which units can be targetted during a kamikaze suicide attack. Also fixed null pointer error for neutral owned kamikaze zones. (veqryn)</li>

  <li>- Created new game option, "Kamikaze Suicide Attacks Done By Current Territory Owner", which allows you to change from the default of the original owner, to the current owner. (veqryn)</li>

  <li>- Cleanup of new PBEM code, and some bug fixing. (qwertgold)</li>

  <li>- Added new Territory Effect Attachment option, noBlitz, which disallows certain units from blitzing in this effect, and also some general cleanup. (edwin & veqryn)</li>

  <li>- Redoing PBEM system to fix bugs and add features. (qwertgold)</li>

  <li>- Adding Pacific 1940 updated to use Kamikaze attacks to the test xml suite. (veqryn)</li>

  <li>- Fixing bug where changing attachment properties of abstracted attachments failed. (veqryn)</li>

  <li>- Created new ui for humans to select what they want to attack for these special attacks, and set the AI to just attack randomly. (veqryn)</li>

  <li>- Created framework for performing special attacks at the beginning of the battle phase, using resources instead of units. (veqryn)</li>

  <li>- New game option to enable kamikaze attacks, "Use Kamikaze Suicide Attacks". (veqryn)</li>

  <li>- Created new Player Attachment, suicideAttackResources, which is the resource and attack value we will use for Kamikaze Suicide Attacks. (veqryn)</li>

  <li>- Changed most iterator loops into enhanced for loops. (frigoref)</li>

  <li>- Changed most instances of Node to Element in the game parser. (edwin van der wal)</li>

  <li>- Created new unit attachment, fuelCost, which allows a unit to use up a resource for each point of movementCost they use. (edwin van der wal)</li>

  <li>- Update of Export Stats to include information on all resources costs, not just PUs. Also fixed production screen to show all resources except techTokens and VPs. (veqryn)</li>

  <li>- Creation of "Economy" tab, besides stats panel, which carries current information on all resources owned by the players. (edwin van der wal)</li>

  <li>- Allowed resizing of the right side panel. (edwin van der wal)</li>

  <li>- Created ability for Game Options to be saved as default options. (qwertgold)</li>

  <li>- Updated Napoleonic Empires FFA to use the new destroyedTUV instead of upkeep. (veqryn)</li>

  <li>- Created new RulesAttachment, destroyedTUV, which allows you to check if a player has destroyed at least X enemy non-neutral TUV this round or all rounds. (veqryn)</li>

  <li>- Created methods inside BattleRecord related classes in order to record the TUV lost during all battles, for the attackers and the defenders. (veqryn)</li>

  <li>- Created BattleRecordsList to keep track of all BattleRecords, and made it be updated after the BattleDelegate ends by use of the ChangeFactory. (veqryn)</li>

  <li>- Created new data object, BattleRecord, in order to record more information about the battles that take place, and BattleRecords to keep track of these inside the BattleTracker. (veqryn)</li>

  <li>- Completely re-wrote Convoy Routes to be flexible and work with any territories, not just sea zones. Can now be used to many any territory require any other group of territories in order to receive income.</li>
Syntax is changed so that that convoyRoute is needed by both territories, while convoyAttached is needed by only the territory that requires the other territories. (veqryn)

  <li>- Updated Territory tab, beside stats tab, to carry significantly more information about the territory your mouse is currently over. Also put scroll bars on the list of units. (veqryn)</li>

  <li>- Created new Territory attachment, "resources", which will allow territories to produce other resources besides PUs. (veqryn)</li>

  <li>- Fixed engine to allow multiple resources for purchasing of units and repairs. Added new panel on stats tab to show additional resources. (edwin van der wal)</li>

  <li>- Phase 4 of abstraction, RulesAttachment now abstracted into RulesAttachment, AbstractRulesAttachment, and AbstractPlayerRulesAttachment. (veqryn)</li>

  <li>- Created a new overlay for territory effect images, that is enabled in map.properties map.useTerritoryEffectMarkers=true, territory_effects.txt, and territoryEffects folder. (edwin van der wal)</li>

  <li>- Fixed bug where 'when' based triggers did not fire at all. (veqryn)</li>

  <li>- Fixed bug where default based triggers were firing multiple times for each default firing location. (veqryn)</li>

  <li>- Created new Trigger Attachment, removeUnits, which allows you to remove units from a territory for selected players. (veqryn)</li>

  <li>- Created new Trigger Attachment, chance, which allows you to have a certain chance for a trigger to activate (tested only after all conditions are true). (veqryn)</li>

  <li>- Phase 3 of abstraction of RulesAttachment and TriggerAttachment and PoliticalActionAttachment: the creation of an abstract class to hold all common cold related to conditions. (veqryn)</li>

  <li>- Created new rules attachment for conditions, chance, which allows you to have a certain chance for a condition to be true. (veqryn)</li>

  <li>- Temporary fix for the issues caused by only testing political conditions once.  Now we test them after each political action. (veqryn)</li>

  <li>- Updated political action attachments validation to only test once per politics phase for all the conditions for each action. (veqryn)</li>

  <li>- Created new relationship attachment, givesBackOriginalTerritories, which lets a player give back originally controlled territories to another player. (veqryn)</li>

  <li>- Changing PropertyUtil from using getClass().getDeclaredMethods() to using getClass().getMethods() for changing data inside game data objects, like units, players, attachments, etc. (veqryn & frigoref)</li>

  <li>- Extended Objective/Condition attachment count "each" to work with Triggers "resource", "purchase", and "placement". (veqryn)</li>

  <li>- Fixing null pointer errors and conceptual problems with my way of testing all conditions. (veqryn)</li>

  <li>- Phase 2 of abstraction and refactoring of TriggerAttachments: now all triggers get called through a single method, collectAndFireTriggers. (veqryn)</li>

  <li>- Created getAllConditionsRecursive and testAllConditions which will test get and test all ICondition, and now all RulesAttachments get tested through these. (veqryn)</li>

  <li>- Had RulesAttachment, TriggerAttachment, and PoliticalActionAttachment all implement ICondition. (veqryn)</li>

  <li>- Created ICondition, and interface for any Attachment that had conditions as a part of it. (veqryn)</li>

  <li>- Moved actions for victory trigger and notification trigger to be part of the trigger attachment so that they will return void, and therefore can abstract easier. (veqryn)</li>

  <li>- Deprecating TriggerAttachments "trigger", and changing name to "conditions" in order to match the other uses of condition attachments. (veqryn)</li>

  <li>- Phase 1 of abstraction of TriggerAttachments, creation of AbstractTriggerAttachment. (frigoref)</li>

  <li>- Fixed bug where I could move my tanks and all land units over water, so long as the end was land. (veqryn)</li>

  <li>- Allowed players with canTakeOverOwnedTerritory to take over during noncombat move. (veqryn)</li>

  <li>- Created new relationship type attachment, canTakeOverOwnedTerritory, which will allow taking over of an ally's territory. (veqryn) </li>

  <li>- Fixing gamenotes for Lord of the Rings Middle Earth. (veqryn)</li>

  <li>- Created new relationship type attachment, canLandAirUnitsOnOwnedLand, which decides if units can land in a player's territory or not. (veqryn) </li>

  <li>- New Map Skin for Napoleonic Empires, which can be enabled in the View menu. (pulicat)</li>

  <li>- Changed BattleModel to show air battle units with different stats then their normal attack/defense stats. (veqryn)</li>

  <li>- Made sure units participating in air battles did not participate in any other battles. (veqryn)</li>

  <li>- Created launching of interceptors component for air battles. (veqryn)</li>

  <li>- Created dice rolling component for Strategic Bombing Air Battles, including for Low Luck. (veqryn)</li>

  <li>- Moved 'Fire' out of MustFightBattle with the hopes of abstracting it and making it a general class one day. (veqryn)</li>

  <li>- Created battle steps and interfaces for Air Battle, but still not done actual combat. (veqryn)</li>

  <li>- Created ability for Air Battles to create Bombing Raids when they are finished if any bombers remain. (veqryn)</li>

  <li>- Created new unit attachments, "canIntercept", "canEscort", "airDefense", "airAttack", which can be combined with new game option, "Raids May Be Preceeded By Air Battles", to allow air battles. (veqryn)</li>

  <li>- Abstracted hashCode and equals methods from all battles and put into AbstractBattle class. (veqryn)</li>

  <li>- Created StrategicBombingRaidPreBattle class, which will handle air battles and other things that occur before bombing raids. (veqryn) </li>

  <li>- Changes to allow Strategic Bombing raids to have multiple targets, with units assigned to different targets. (veqryn)</li>

  <li>- Some further abstraction of AbstractBattle class. (veqryn)</li>

  <li>- Cleanup of some tests to use ChangePerformer to edit data directly, instead of Change.perform(). (frigoref)</li>

  <li>- Allowed scrambling to any territory, and allowed moving the units after scrambling is completed, to anywhere. (veqryn)</li>

  <li>- Allowed scrambling units to move to find new landing zones if their originating territory was taken or they are not forced to return to it. (veqryn)</li>

  <li>- Wrote new Scrambling ui dialog from scratch, and made it work over the network. (veqryn)</li>

  <li>- New game option, "AI Bonus Income Flat Rate", which gives a flat bonus every turn to all AIs. (veqryn)</li>

  <li>- Changed PlayerID.getData() to be deprecated, and removed all uses of it that I could. (veqryn)</li>

  <li>- Fixed various bugs in Scrambling, like not having dependent battles, not adding the units to existing battles, not removing units from old battles. (veqryn)</li>

  <li>- Completely re-wrote how scrambling works.  All scrambling now takes place before any battles begin.  (veqryn)</li>

  <li>- New game option, "Scramble To Any Amphibious Assault", allows bases not being attacked to scramble to defend bases that are being attacked amphibiously. (veqryn)</li>

  <li>- Allowed double clicking on a game in the lobby to equal joining that game. (veqryn)</li>

  <li>- Removing all scrambling code from the engine, in order to start over and code correctly. (veqryn)</li>

  <li>- Created new TripleAUnit variable for keeping track of bonus movement, and eliminated use of unit attachment getMovement.  In order to see a units movement, please use either getMaxMovementAllowed() or getMovementLeft(), both in TripleAUnit. (veqryn)</li>

  <li>- Complete cleanup of all code, adding final on to everything that can take it. (veqryn)</li>

  <li>- Redoing of movement validation to use movement costs, and completely rewriting the movement validation of carriers and aircraft for landing zones. (edwin van der wal)</li>

  <li>- Refactoring Route class to use movement costs, rather than number of steps. (edwin van der wal)</li>

  <li>- Changing the internal logic of scrambling to correctly test for the max scrambling length, and a new unit attachment, maxScrambleCount, which determines how many units can scramble. (bung)</li>

  <li>- Allowed "each" as a count number for National Objectives, which then multiplies the bonus by the number of territories in that list who have their conditions met. (veqryn)</li>

  <li>- Network menu option, "Show Who is Who", now shows players who are AI. (veqryn)</li>

  <li>- Players who have both no movable attacking land units units, and either no factories or no land, will no longer be able to do any political actions, and any political actions affecting only them can not be done. They will now auto-accept any action from another player in addition. (veqryn) </li>

  <li>- Allowed alliances to stop having war with each other. (veqryn)</li>

  <li>- Allowed players to leave an alliance completely, with all members. (veqryn)</li>

  <li>- Forced all alliance players to go out of war if one of them goes out of war, with a player. (veqryn)</li>

  <li>- Forced players to have their ally's agreement when going into or out of war, and letting new people into the alliance. (veqryn)</li>

  <li>- Created new relationshipTypeAttachment, isDefaultWarPosition and alliancesCanChainTogether, which handle if and when relationships will chain. (veqryn)</li>

  <li>- Created new game option, "Alliances Can Chain Together", which causes anyone who is allied with your ally, to become your ally, and any of your ally's enemies to become your enemy. (veqryn)</li>

  <li>- Created new game option, "Relationships Last Extra Rounds", which lets a player have relationships last additional or fewer rounds than default. (veqryn)</li>

  <li>- Added ability for TripleA to remember which type of player you selected when you reload the game. And fixed bug where hosted online games did not remember your selection. (veqryn)</li>

  <li>- Added methods for AI to cheat in all games, using new properties: "AI Bonus Income Percentage", "AI Bonus Attack", "AI Bonus Defense". (veqryn)</li>

  <li>- Fixed "not all units can blitz" bug. (veqryn)</li>

  <li>- Made the engine write who (ai/human/client) is playing each player, each time game is loaded, to the history panel. (veqryn)</li>

  <li>- Adding political map skin, and reconstructed basetiles, for Napoleonic Empires. (veqryn)</li>

  <li>- Stopped blitzing out of a combat into further combat, if you began in same territory. (veqryn)</li>

  <li>- Allowed less strict Edit Mode options. (veqryn)</li>

  <li>- Changed PlayerID to record if the player is Human or AI, and which type of AI. (veqryn)</li>

  <li>- Allowed territories with now hostile units to be redrawn, and have red markup, at the end of the politics delegate. (veqryn)</li>

  <li>- Fixed bug where you could capture territory from a power you were neutral or allied with, if you attacked an enemy on their territory. (veqryn)</li>

  <li>- Fixed multiple bugs surround territories suddenly made hostile. And created a new class, "RouteScripted", which allows for Routes that do not follow the normal rules. (veqryn)</li>

  <li>- Fixed bug where territories with no units, had enemy units in them from a previous turn, did not start any battle, and where therefore never taken over. (veqryn)</li>

  <li>- Fixed null pointer in Moore AI for when it owns a factory in a territory it does not control. (veqryn)</li>

  <li>- Created new unit attachment, "special", which currently allows for "canOnlyPlaceInOriginalTerritories". (veqryn)</li>

  <li>- Fixed zoom out and zoom in on the map with the Mouse Wheel, by holding down the "ALT" key. (veqryn)</li>

  <li>- Changing relationship type attachment, upkeepCost, to allow an integer percentage, which will effect all income gained during the end of turn step. (veqryn)</li>

  <li>- Re-allow booting (boot-slapping) of admins. (veqryn)</li>

  <li>- Allowed double clicking for selecting a game, and had the choose game list be cached, with a refresh button. (qwertgold)</li>

  <li>- Fixed bug in stats and xml exporter where the file name contained illegal characters, causing the file creation to fail. (veqryn)</li>

  <li>- Fixed bug where clicking cancel in order to look around the map, during casualty selection, generated an error. (frigoref)</li>

  <li>- Fixed bugs in alliance tracker related to players not being in an alliance. (veqryn)</li>

  <li>- Fixed bugs in 'example' maps: Tic Tac Toe, King's Table, and Sliding Tiles 8-number. (veqryn)</li>


</ul><h3>Changes for 1.4</h3><ul>
  <li>- Adding politicstext.properties for Napoleonic Empires. (veqryn)</li>

  <li>- Massive update to Napoleonic Empires: FFA, to allow it to use Politics. (veqryn)</li>

  <li>- Updating Pact of Steel 2 and Pacific test xmls. (veqryn)</li>

  <li>- Added scroll bars to select casualties dialog panel. (veqryn)</li>

  <li>- Sorted political actions based on player, type, and name. (veqryn)</li>

  <li>- Capped Politics ui actions, and added scroll bars to the bottom button part. (veqryn)</li>

  <li>- Fixed rendering issue where nations that were neutral to each other still caused red markup when in the same territory or sea zone. (frigoref)</li>

  <li>- Fixed bug where victory city victories happened in FFA maps according to the current alliance rather than the player's alliance tracker. (veqryn)</li>

  <li>- Added "upkeepCost" as an attachment for RelationshipTypeAttachment, which allows you to have a cost in order to maintain a relationship. (veqryn)</li>

  <li>- Changed "invert" in rules attachments, trigger attachments, and political attachments, to work as a real logical negation. Now correctly follows boolean math. (veqryn)</li>

  <li>- Added roundValue to relationshipInitialize, which is the beginning round a relationship starts out at. This should normally be "1", but if you have certain conditions set up, you may wish to change this to a negative or positive number to reflect what round you would like the condition to be true on. (veqryn)</li>

  <li>- Made AI behavior towards politics to be a bit more random, allowing it to take any political action so long as it has 10x the amount of PUs as the political action's cost. (veqryn)</li>

  <li>- Abstracting isMet logic for rules attachments into a single place, areConditionsMet, in RulesAttachment. (veqryn)</li>

  <li>- Changed unitPresence to allow inputting of multiple units on one line for an OR relationship between those units. (veqryn)</li>

  <li>- Fixed bug surrounding infinite loop caused by having nations A and B neutral with each other, but at war with C nation owning both subs and transports in a sea zone, attacked by the C nation. (frigoref & veqryn) </li>

  <li>- Fixing bug introduced into must fight battle, by the battle class abstraction. Also slightly updating the dev documentation. (frigoref)</li>

  <li>- Changed triggers "uses" to use up a single 'use' every round that they are used.  So a trigger with 4 action types will use up a single use (instead of 4), assuming those four actions were done in the same round. (veqryn)</li>

  <li>- Some code cleanup. (veqryn)</li>

  <li>- Fixed null pointer error in Moore AI's rank territories method, due to politics change. (veqryn)</li>

  <li>- Adding PoliticalActionAttachment to the list of attachments that triggers can change through players + playerAttachmentName + playerProperty. (veqryn)</li>

  <li>- Adding invert and conditionType to Political Action Attachments, also changing conditions to allow multiple conditions. (veqryn)</li>

  <li>- Changing Pact of Steel 2 to allow for politics, without greatly affecting the game. (veqryn)</li>

  <li>- Adding baseAI code for AIs to declare war on people. (edwin van der wal & veqryn)</li>

  <li>- Abstraction of various fighting battles into AbstractBattle, and renaming of Battle.java to IBattle. (frigoref)</li>

  <li>- Added ability for BaseDelegate to keep track of whether triggers have fired or not, and changed all delegates to record and load super's saveState data when saving and loading. (veqryn)</li>

  <li>- Some small ui fixes for politics. (edwin van der wal)</li>

  <li>- Removing @Overrides for implemented methods, in order to maintain Java 1.5 compatibility. Also removing unnecessary casting. (veqryn)</li>

  <li>- Adding web links to normal game menu bar, and also adding link for guides page on triplea homepage. (veqryn)</li>

  <li>- Created two new game options, "Use Politics" and "Units Can Be Changed On Capture". (veqryn)</li>

  <li>- Fixing bugs in last patch on politics. Deleted relationshipExistance and instead made it part of "relationship" setter. (veqryn)</li>

  <li>- Added Politics UI. (edwin van der wal)</li>

  <li>- Created relationshipExistance property in RulesAttachment, if this is set in combination with a relationship property, the relationshipExists property will indicate the number of complete rounds this relationship needs to have been in existance. (edwin van der wal)</li>

  <li>- Created new attachment, politicalActionAttachment, which sets which actions are allowed during the politics phase for a player. (edwin van der wal)</li>

  <li>- Removing trigger when notifications from TripleAPlayer (because no gamedata changing logic should ever be in TripleAPlayer), and moving them to basedelegate. (edwin van der wal & veqryn)</li>

  <li>- Fix for Casualty Reset Bug 1730391, where casualty screen clears after saving and reloading. (frigoref & veqryn)</li>

  <li>- Changed whenCapturedChangesInto to allow the transferring of combat damage and unit damage to the new units. (veqryn)</li>

  <li>- Changed whenCapturedChangesInto to allow creating multiple unit types and multiple of a unit. (veqryn)</li>

  <li>- Changed whenCapturedByGoesTo to not work when liberating an ally's territory. (veqryn)</li>

  <li>- Created new unit attachment, whenCapturedChangesInto, which allows you to have a unit change into a different unit type when it is captured. (veqryn)</li>

  <li>- Created new territory attachment, whenCapturedByGoesTo, which allows you to have a territory be given to another player when captured by a certain player. (veqryn)</li>

  <li>- Workaround fix to screenshot export bug. (edwin van der wal)</li>

  <li>- Code cleanup of needless casting. (veqryn)</li>

  <li>- Code cleanup of warnings. (veqryn)</li>

  <li>- Fixed bug in Increased Factory Production tech, where it discounted any units bought by half, so long as you bought only 1 type of unit this turn. (veqryn)</li>

  <li>- Allowing the map to be redrawn if territory attachments are changed mid-game. (veqryn)</li>

  <li>- Fixed null pointer error in Moore AI, and also an incorrect validation of warning the user when they have produced more than they can place. (veqryn)</li>

  <li>- Fixing some bugs based on FindBugs, and general code cleanup. (veqryn & edwin van der wal)</li>

  <li>- Fixed bug where memory for online and hosted games was set artificially low at 128, instead of being set to the max memory set by triplea run scripts and exe. (veqryn)</li>

  <li>- Removing one memory leak from battle calc, it was recording the units is created to game data, inflating the savegame size. (veqryn & frigoref)</li>

  <li>- Source code formatting on entire engine. (veqryn)</li>

  <li>- Using cleanup to add @Override to anything that overrides something. (veqryn)</li>

  <li>- Correcting problems with frig last patch to do with extended methods no longer overwriting super's methods. (veqryn)</li>

  <li>- Removing more needless gamedata passing. (frigoref)</li>

  <li>- Some general code cleanup, especially with iterators and rawtypes. (veqryn)</li>

  <li>- Removed needless gamedata passing, and added methods to get game data out of bridge. (frigoref)</li>

  <li>- Updated export stats to display far more information, about actual techs gained, and number of each unit type for each player, etc. (veqryn)</li>

  <li>- Updated game data to record the playerIDs of whoever wins the game. (veqryn)</li>

  <li>- Started making tests for all the features added in the last year. Made placeholder tests for everything revision 2800-3000. (veqryn)</li>

  <li>- Changing UIContext.m_mapDir static, so that is may be accessed anywhere. (frigoref)</li>

  <li>- Added information on productionRules and UnitTypes to the export stats function. (veqryn)</li>

  <li>- Changed some string comparing from == and != to .equals() and !.equals(). (veqryn)</li>

  <li>- Created new rules attachment, placementAnySeaZone, that allows placing sea units beside any land territory owned at the beginning of the turn. (veqryn)</li>

  <li>- Fixing bugs in old victory conditions and moving them to endRoundDelegate, and also fixing bugs surrounding strings in attachment property change triggers. (veqryn)</li>

  <li>- Adding PactOfSteel2 and Pac40 xmls to test xml suite. (veqryn)</li>

  <li>- Changed destroyedWhenCapturedBy to allow destroying when capturing from a player, not just by a player, by adding a prefix of "BY:" or "FROM:" and also created destroyedWhenCapturedFrom which calls destroyedWhenCapturedBy with a "FROM:" prefix. (veqryn)</li>

  <li>- Changed unitAttachment toString to be much more informative, and include all values. (veqryn)</li>

  <li>- Created new Relationship attachments for canMoveLandUnitsOverOwnedLand and canMoveAirUnitsOverOwnedLand, and set them to validate movement. (veqryn)</li>

  <li>- Allowed conditionType for both triggers and conditions (objectives) attachments to have integer values, in addition to other values,</li>
  conditionType now allowing: 'AND' or 'OR' or 'XOR' or 'y' or 'y-z' where Y and Z are valid positive integers and Z is greater than Y. (veqryn)

  <li>- Allowing html to be used for both triggered notifications and for triggered victory messages. (veqryn) </li>

  <li>- Added ability for the defender to capture units if it wins on defense and the attacker brought capturable infrastructure units to the battle. (veqryn)</li>

  <li>- Fixing bug in moving defending air to land when a carrier is damaged on defense. (veqryn)</li>

  <li>- Fixing bugs surrounding unitsMayNotLandOnCarrier and unitsMayNotLeaveAlliedCarrier interacting with each other. (veqryn)</li>

  <li>- Updated whenCombatDamaged to work with unitsMayNotLeaveAlliedCarrier. (veqryn)</li>

  <li>- Updated whenCombatDamaged to work with unitsMayNotLandOnCarrier. (veqryn)</li>

  <li>- Created new unit attachment ability to have a unit behave differently when damaged, using whenCombatDamaged. (veqryn)</li>

  <li>- Adding notes about all properties to Pact of Steel 2 xml, and some code cleanup. (veqryn)</li>

  <li>- Updated receivesAbilityWhenWith to work for "canBlitz". (veqryn)</li>

  <li>- Created new unit attachment ability to have a unit receive an ability when in the presence or on the same route with another unit, using "receivesAbilityWhenWith". (veqryn)</li>

  <li>- Created triggers for changing any attachment that is attached to a territoryEffect by using: territoryEffects, territoryEffectAttachmentName, and territoryEffectProperty. (veqryn)</li>

  <li>- Created triggers for changing any attachment that is attached to a relationshipType by using: relationshipTypes, relationshipTypeAttachmentName, and relationshipTypeProperty. (veqryn)</li>

  <li>- Created triggers for changing any attachment that is attached to a territory by using: territories, territoryAttachmentName, and territoryProperty. (veqryn)</li>

  <li>- Created triggers for changing any attachment that is attached to a unit by using: unitType, unitAttachmentName, and unitProperty. (veqryn)</li>

  <li>- Created triggers for changing any attachment that is attached to a player by using: players, playerAttachmentName, and playerProperty. (veqryn)</li>

  <li>- Completely re-wrote how raw changes were done, and deleted attachmentToBeChangedName and attachmentToBeChangedProperty. (veqryn)</li>

  <li>- Created new ability to set when a trigger fires, with "when", setting "before/after:stepName", that works with all triggers. Triggers still maintain a default step for firing. (veqryn)</li>

  <li>- Finished work on making triggers for rules and trigger attachments, using attachmentToBeChangedName and attachmentToBeChangedProperty. (veqryn)</li>

  <li>- Preliminary work on making new triggers for rules attachments, and fixing issue with clearing properties without setting. (veqryn)</li>

  <li>- Created new triggers for changing player attachments, using players and playerProperty. (veqryn)</li>

  <li>- Finished work on allowing triggers to clear data from properties that add rather than overwrite data, by adding "-clear-" to the beginning of the new property, in the triggered change. (veqryn)</li>

  <li>- Fixed issue where stats panel and exported stats relied on the first game steps it saw to determine turn order, which meant it considered the order of bids as representative of turn order, instead of looking at things like movement. (veqryn) </li>

  <li>- Preliminary work on allowing triggers to clear data from properties that allow multiple sets, in other words, properties that add data rather than overwriting. (veqryn)</li>

  <li>- Created new triggers for changing territory properties, using territoryName and territoryProperty. (veqryn)</li>

  <li>- Fixed unitProperty trigger change to accept properties with more than one colon. (veqryn)</li>

  <li>- Created ability to make conditions and rules attachments that include other conditions in them, and the ability to set the relationship of these conditions to AND, OR, XOR. (veqryn)</li>

  <li>- Fixed bug where getCosts in BattleCalculator was only returning the costs for the units that a nation could produce, instead of all units that nation could own. Changed to BattleCalculator.getCostsForTUV (veqryn)</li>

  <li>- Fixed bug where TUV in stats panel showed units that had multiple given per production, like NWO's artillery was buy 2 for 7 PUs, incorrectly show on the TUV panel as 7 PUs each. Now it shows up as the rounded up value. (veqryn)</li>

  <li>- Updating client game and server model to carry information on alliances and player order. (veqryn)</li>

  <li>- Allowed the exporting of stats based on the individual phases in a players turn. (veqryn)</li>

  <li>- Updating local player selection screen to show players in turn order, assuming xml was done properly, and to show their alliances. (veqryn)</li>

  <li>- Updating 'Export Game Stats...' to give more general information about the game. (veqryn)</li>

  <li>- Fixing bug where newly created battles now included duplicates of any units that were strategically bombing a territory. (veqryn)</li>

  <li>- Allowed for units that were in territories suddenly made hostile by a change in politics to create battles in those territories. (veqryn)</li>

  <li>- Fixed remaining unit tests. (veqryn)</li>

  <li>- Engine code cleanup. (frigoref)</li>

  <li>- Some small fixes for unit tests, and some small abstractions. (frigoref & veqryn)</li>

  <li>- Changed combat filters to allow infrastructure with support or combat abilities to take part in combat. (veqryn)</li>

  <li>- Fixing some unit tests, creating tests for Revised sub bug. (veqryn)</li>

  <li>- Fixed casualty selection hang bug, and also abstracted CasualtyDetails. (veqryn)</li>

  <li>- Fixing some unit tests. (veqryn & frigoref)</li>

  <li>- Updated all test xmls. (veqryn)</li>

  <li>- Fixed bug introduced into undoing moves, where undoing a sea placement generated an error. (frigoref)</li>

  <li>- Created new trigger ability to add and remove production rules from a production frontier. (veqryn)</li>

  <li>- Beginning work on territory effects, and some cleanup in the use of basedelegate. (edwin van der wal, with help from frigoref and veqryn)</li>

  <li>- Adding ability to trigger notification messages to the players. (edwin van der wal)</li>

  <li>- Some beginning work on Dynamix AI sea transportation methods. (wisconsin)</li>

  <li>- Fixing of some matches to use new relationships, and some general code cleanup. (veqryn)</li>

  <li>- Various code cleaning. (frigoref)</li>

  <li>- Some changes to how politics gets initialized. (edwin van der wal)</li>

  <li>- Cleaning up of relationships, have alliances auto-create relationships based on default war or allied, and creation of relationship interpreter class. (frigoref)</li>

  <li>- Allowed basic html to be used inside unit tool tips. (veqryn)</li>

  <li>- Created new unit attachment, createsResourcesList, which allows units to create resources like PUs and techTokens each turn for their owner. (veqryn)</li>

  <li>- Created framework and objects for having individual relationships between players, rather than set alliances and war as the only option. (edwin van der wal, with some help from frigoref and veqryn)</li>

  <li>- Created politics delegate, which will eventually be filled with the logic and ui elements to allow players to change their alliances and relationships with other players. (edwin van der wal)</li>
    <delegate name="politics" javaClass="games.strategy.triplea.delegate.PoliticsDelegate" display="Politics"/>

  <li>- Fixed inability to save games during placement phase. (frigoref)</li>

  <li>- Added ability to customize tooltips for units, using "tooltips.properties". (edwin van der wal)</li>

  <li>- Stop caching of production_tabs properties, will now read the file each time purchase screen is displayed. (edwin van der wal)</li>

  <li>- Small fixes to new production_tabs properties and display. User specified production tabs must include all units possible to be purchased by a player, or else an error will be thrown. (veqryn)</li>

  <li>- Added ability to customize production tabs for each map, using "production_tabs.properties" and "production_tabs.PlayerName.properties". (edwin van der wal)</li>

  <li>- Added matches for dependencies and transported by. (veqryn)</li>

  <li>- Fixed route finder to find better routes for units. Will stop finding sea routes for land units, and land routes for sea units. Will try to avoid enemies, AA guns, and neutrals. (veqryn)</li>

  <li>- Fixed bugs in canInvadeOnlyFrom. (veqryn)</li>

  <li>- Created new unit attachment, canInvadeOnlyFrom, which determines if a unit can conduct amphibious assaults or if it has to disembark in noncombat. (edwin van der wal)</li>

  <li>- Made placements appear as a list, just like moves do, and can now be undone individually. Abstracted undoable moves and placements. (frigoref)</li>


</ul><h3>Changes for 1.3.2.3</h3><ul>
  <li>- Fixed bug where casualty selection window was never shown and battles hanged, due to infinite loop inside default casualty sorting process under special conditions. (veqryn)</li>

  <li>- Fixed bug where units that had previously died to strat bombing, rockets, or scrambling, were still present in the battle if there was a conventional battle immediately afterwards in that territory. (veqryn)</li>

  <li>- Fixed bug in validation of non-combat movement of paratroopers. (veqryn)</li>

  <li>- Fixed error where allied air on defending carriers may not shoot at non-sub units under certain conditions. (veqryn)</li>

  <li>- Fixed error where after a player got paratroopers, ships no longer had their movement validated correctly. (veqryn)</li>

  <li>- Fixed error related to two-hit battleships in middle earth. (veqryn)</li>


</ul><h3>Changes for 1.3.2.2</h3><ul>
  <li>- Fixed infinite loops in purchasing methods for both Strong AI and Weak AI, for low cost units. (veqryn)</li>

  <li>- Fixed null pointer error in Strong AI landing of air units for players with impassible capitals. (veqryn)</li>

  <li>- Changed savegame-xml exporter to add occupiedTerrOf to any territory not owned by current owner. (veqryn)</li>

  <li>- Fixed bug in validation of air that can't land for mixed allied and owned air attempting to land where there already is a carrier and a new carrier will also be placed. (veqryn)</li>

  <li>- Fixed null pointer error in Strong AI sea movement. (veqryn)</li>


</ul><h3>Changes for 1.3.2.1</h3><ul>
  <li>- Added new button to main screen, "Rule Book...", which will open up the user's default web browser and go to the triplea sf page with our future rulebook. (veqryn [Mark Christopher Duncan])</li>

  <li>- Updated "unitProduction" so when used in conjunction with "Damage From Bombing Done To Units Instead Of Territories" it sets the allowed number of units to be produced in that territory, thereby finally un-associating the PU production of a territory from the Unit production of a territory.</li>
  Also, updated "production" to automatically set "unitProduction" to be equal. So if you want a different unitProduction value, you must set it after production when attaching to a territory. (veqryn [Mark Christopher Duncan])

  <li>- Fixed bug related to territory damage in history panel, as well as a null pointer error for factories on territories with no attachments, and also fixed a bug that was not allowing canProduceUnits units to have same max damage as factory units. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added information on number of units being purchased to production panel. Also changed all upgrade/consumes type units to have their names displayed in blue. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added tabs option to production panel. (edwin van der wal)</li>

  <li>- Fixed bug where upgrades of sea units could be placed same turn as the base unit. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed bug where air units may not participate in a battle if they had been on an allied carrier that was involved in a battle. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed bug where units with zero attack that were supportable never got to roll in combat. Also, re-wrote getRolls. (veqryn [Mark Christopher Duncan])</li>

  <li>- Balancing fixes for LOTR Middle Earth. (ajmdemen)</li>

  <li>- Small fixes to exporter classes. (edwin van der wal & veqryn [Mark Christopher Duncan])</li>

  <li>- Balancing fixes for Pact of Steel 2. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed issue with carriers that are also transports not allowing their land units to participate in battle when the sea unit has participated in battle. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added many new admin features to lobby server and client. (wisconsin)</li>

  <li>- Added ability to export a savegame to an xml, thereby allowing in game editing of maps. (edwin van der wal)</li>

  <li>- Added new game property, "Neutral Flyover Allowed", which like it says, will allow you to fly over neutrals. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed bug in movement validation that allowed paths over impassibles and restricted territories to be taken into account for landing zones. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed bug in movement validation that allowed both combat and noncombat flyover of neutrals. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed bug in movement validation for paratroopers and mechanized infantry techs when a unit has received bonus movement from an airfield or harbour. (veqryn [Mark Christopher Duncan])</li>

  <li>- Several small changes to Middle Earth, Big World v3 rules, and Pact of Steel 2. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed to allow old Mac OS X computers to connect to lobby, again. (veqryn [Mark Christopher Duncan])</li>

  <li>- Small fix to validation of user data for lobby. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed bug where allied fighters on carriers were not moving with the carriers under certain situations, like when there was an transport ship in the same sea zone, or a harbour or airfield had modified their movement. (veqryn [Mark Christopher Duncan])</li>


</ul><h3>Changes for 1.3.1.1</h3><ul>
  <li>- Allowing lobby to parse user data more effectively. (wisconsin & veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed major bug in low luck support attachments, where units got up to double the support they were supposed to get. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed Dynamix settings menu to use java 1.5 compatible coding, instead of java 1.6.  With this change, and the removal of string isEmpty calls, TripleA is once again compatible with java 1.5 and Mac OS computers. (wisconsin)</li>

  <li>- Updated then Added "Big World : v3 Rules" game, a mod of the original Big World mostly by Prussia, to triplea. (veqryn [Mark Christopher Duncan])</li>

  <li>- Removed String .isEmpty calls, as they are not supported under Java 1.5, also called java 5. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed fighters and air disappearing even if you bought a carrier, if there is another turn like china, between yours and the placement of the carrier. (veqryn [Mark Christopher Duncan]) </li>

  <li>- Fixed paratrooper loading creating multiple copies of units. Fixed bugs for deselection of paratroopers and air. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed minor bugs, including units having to roll to kill unescorted transports. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added more ways to get user info for connecting to the lobby on older max-os / unix machines. (veqryn [Mark Christopher Duncan])</li>

  <li>- Got lobby actions to correctly be logged, and fixed bug in banning system. (wisconsin)</li>

  <li>- Fixed all issues surrounding connecting to the lobby. (veqryn [Mark Christopher Duncan])</li>

  <li>- Updated packaged java JRE to java 6 update 25. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added ability to remove games from the lobby screen. (wisconsin)</li>

  <li>- Fixed error for old java versions that were unable to access online lobby. (wisconsin)</li>

  <li>- Created new unit attachment, createsUnitsList, which allows automatic creation of units by other units at end of turn. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed unitAttachment validation to allow factories to have maxDamage. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed build.xml to work for macRelease. (veqryn [Mark Christopher Duncan])</li>


</ul><h3>Changes for 1.3.1.0</h3><ul>
  <li>- Fixed "what should bomber bomb" AI error, in all AIs. Also fixed bug in easy ai where it would not place any units if some were bunkers. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed moore AI and easy AI to use new repairing method when trying to repair unit damage instead of territory damage. (veqryn [Mark Christopher Duncan])</li>

  <li>- Some updates for Dynamix AI, and fixed AI bug caused by more than one map was opened per TripleA instance, and Added a Resource Collection Increaser cheat. (wisconsin)</li>

  <li>- Finished making repair rules work for both damage done to units and damage done to territories. </li>
  A note to map makers: repair rules should mention the actual unit, not a _hit version of the unit.  This means all repair rules that mention "factory_hit" will need to be changed to mention "factory". (veqryn [Mark Christopher Duncan])

  <li>- Initial work on making repair rules work for damage done to units. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed null pointer in moore ai for games which don't have carriers. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added method to unit class to find territory unit is in. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed moore AI and easy AI to not purchase any unit which has consumesUnits. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed bug in scrambling code where user was not being asked if they want to scramble. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed infinite loop introduced into original factory owner check. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new unit attachment, canProduceUnits, which allows a unit to produce other units, without being a factory. Therefor we can now have combat factories, flying factories, or aa gun factories, or w/e. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added the developer forum and the war club to the lobby help menu. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added tool tips for units to battle calculator. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed null pointer caused by using .getOwner().getData()  and a word to anyone else who ever thinks about using this: don't, it causes null pointers if there are any neutrals, since neutral is a null player. (veqryn [Mark Christopher Duncan])</li>

  <li>- Created new unit attachment, requiresUnits, which allows units to be placed only when certain units are in the territory. (veqryn [Mark Christopher Duncan])</li>

  <li>- Changed it so that Territory production defaults to Zero instead of 2, and that unitProduction gets set to a territory's production, though you can still set unitProduction manually if you set it AFTER you set production. (veqryn [Mark Christopher Duncan])</li>

  <li>- Created new unit attachment, consumesUnits, which allows units to be upgraded or placed on top of other units. (veqryn [Mark Christopher Duncan])</li>

  <li>- Created new unit attachment, canOnlyBePlacedInTerritoryValuedAtX, which defaults to -1 meaning can be placed anywhere. (veqryn [Mark Christopher Duncan])</li>

  <li>- Expanded 'disabled' logic to include airbases, repairsUnits, givesMovement, and combat units. Disabled units will not provide their abilities, like scrambling, movement, or repairing, to other units.  Disabled combat units will not participate in combat, and will be destroyed if captured. (veqryn [Mark Christopher Duncan])</li>

  <li>- Created the placement logic for canProduceXUnits, which now works properly. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed display error where units with unit damage were not having their damage amount displayed. Still some bugs though for groups of units. (veqryn [Mark Christopher Duncan])</li>

  <li>- Created new unit attachment, canDieFromReachingMaxDamage, which will cause a unit to die if they reach max damage through strat bombing or rockets. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed bug in triggers that caused unit production damage to be done to a territory if a factory was placed via triggers. (veqryn [Mark Christopher Duncan])</li>

  <li>- Allowed rockets to also damage a unit, rather than a territory.  Further work on getting unit damage to work and display properly. (veqryn [Mark Christopher Duncan])</li>

  <li>- Made disabled units actually work. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed bugs introduced into Strategic Bombing. (veqryn [Mark Christopher Duncan])</li>

  <li>- Created new global property, "Damage From Bombing Done To Units Instead Of Territories", which when ON will have damage be done to units rather than territories, as territory damage was the old way of doing things. </li>
  In order for this to work, you must have "SBR Affects Unit Production" turned OFF, as that is the trigger for per territory damage. (veqryn [Mark Christopher Duncan])

  <li>- Created "canProduceXUnits" unit attachment. Set to "-1" if you want to produce the value of the territory the unit is in. Still working on the code for this. (veqryn [Mark Christopher Duncan])</li>

  <li>- Removed "isCombatInfrastructure" and "unitDamage" from unit attachments, and also removed m_maxOperationalDamage from TripleAUnits. Unit damage is per unit, not per unit type, so it should never be a unit attachment. (veqryn [Mark Christopher Duncan])</li>

  <li>- Stopped both Moore AI and Easy AI from buying any units that have maxBuildRestrictions. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added lobby rules web page to list of web pages available from the new help menu in the lobby screen. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed null pointer in unit drawer. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fix for Moore AI, it was choosing to never ever attack neutrals in some situations, even if they blocked the path towards the enemy. (veqryn [Mark Christopher Duncan])</li>

  <li>- Abstracting MovePanel class. (frigoref)</li>

  <li>- Removing constants that refer to specific units, as we should be using unit attachments instead.  Also minor updates to unit attachment's new toString. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added "Reset" button to Map Zoom. (veqryn [Mark Christopher Duncan])</li>

  <li>- Allowed for more information about units to be displayed as a tool tip on the territory panel. (veqryn [Mark Christopher Duncan])</li>

  <li>- Created new toString in unit attachment to only display important information that is different from a default unit with no attachments. (veqryn [Mark Christopher Duncan])</li>

  <li>- Allowed for more information about units to be displayed as a tool tip during production screen.  Allowed tool tip to be displayed when hovering over unit icon, in addition to small info stats. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixes for various null pointer errors. (veqryn [Mark Christopher Duncan])</li>

  <li>- New unit attachment setter, "unitPlacementOnlyAllowedIn", which is the direct inverse of "unitPlacementRestrictions". (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed issue [bug 3294118] where transports drop their ground units in the ocean when they engage in combat. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new global property, "On Entering Units Destroyed Instead Of Captured", which if true allows units normally captured on entering to be destroyed.  Does not affect non-combat units, only affects combat units with the canBeCapturedOnEnteringBy attachment. (veqryn [Mark Christopher Duncan])</li>


</ul><h3>Changes for 1.3.0.0</h3><ul>
  <li>- Added the new username banning system, which will help a lot on the lobby. Like to ban offensive usernames without necessarily banning the player. (wisconsin)</li>

  <li>- Another patch for Dynamix AI (wisconsin)</li>

  <li>- Added airfield_disabled.png and harbour_disabled.png for all nations (veqryn [Mark Christopher Duncan])</li>

  <li>- Flipped all unit graphics. All axis sea and air point left, while allies point right (except russian air points left).  All ground units for a country point same direction, left for japan and russia, right for everyone else. Non-combat units and aaGuns do not point any direction, or are same for all nations. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed Neutrals charge to work properly, without java errors, if the neutral is attacked and there is a battle. Will now display a message in history panel if there is not enough PUs to remove. (veqryn [Mark Christopher Duncan])</li>

  <li>- Determine if units are 'disabled' and display a unique icon for them (ComradeKev)</li>

  <li>- Initial work on Scrambling aircraft (ComradeKev)</li>

  <li>- Fixed bug in StrongAI/MooreAI where it would never attack a player if it lost too much TUV, and the TUV calc thought the enemy had zero TUV. Also fixed bug where it calced for the offensive value of walk in territories, instead of defensive value. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added a global property, "Capture Units On Entering Territory", which if true allows units to be captured instead of fighting. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new player attachment, captureUnitOnEnteringBy, which will allow this player to let some of the units be captured when a territory is taken over. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new territory attachment, captureUnitOnEnteringBy, which will allow units in the territory to be taken when the territory is captured. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new unit attachment, canBeCapturedOnEnteringBy, which will allow a unit to be taken when the territory is captured. (veqryn [Mark Christopher Duncan])</li>

  <li>- Changed Strategic Bombing to account for isSuicide units. Now isSuicide units will also die if they strategic bomb something. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed error unit display of unit graphics, where things that were _hit needed _it on the end instead of front, sometimes resulting in needing _it_hit_it, etc. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed null pointer in game data getNeighbors match. (veqryn [Mark Christopher Duncan])</li>

  <li>- Updating default maps to use latest properties. (veqryn [Mark Christopher Duncan])</li>

  <li>- Rewrote entire RulesAttachment.java so that territory conditions could use "count" with options like "original", "controlled", etc. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new rule property option, "map", for use with Presence and Exclusion conditions. If used, it will return the entire map's territories. (veqryn [Mark Christopher Duncan])</li>

  <li>- Made it so that jet power technology and super subs technology no longer affect units with zero attack and zero defense. (veqryn [Mark Christopher Duncan])</li>

  <li>- Completely re-wrote checkUnitExclusions and Made unitPresence work with directExcludedTerritories, alliedExclusionTerritories, enemyExclusionTerritories, enemySurfaceExclusionTerritories. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new rule property and condition/objective, "directExcludedTerritories", which applies to the attached player. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new rule property and condition/objective, "unitPresence", as well as "directPresenceTerritories", "alliedPresenceTerritories", and "enemyPresenceTerritories". </li>
  unitPresence is a unit and count for that unit, which must be used with a presence territories to determine if there are those units in those territories or not. (veqryn [Mark Christopher Duncan])

  <li>- Added new trigger option, "conditionType", which can be set to AND, OR, XOR. This option defines the relationship conditions in a trigger must have, when there is more than 1 condition in the trigger. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed bug in triggers where an inverted trigger would activate when it should not, when one condition was false but another true. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added the ability for any construction of type ending in "structure" not to be changed by setting global values for unlimited/more constructions. Also fixed issue with submarine suicide units able to attack aircraft. (veqryn [Mark Christopher Duncan])</li>

  <li>- Updating UnitImageFactory to not rely on hardcoded unit names. Now any unit with isAA unit attachment will require _r and _rockets and _rockets_r IF you have those technologies.  Same applied for new aa gun rules and factories. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new unit attachment, isRocket, which will turn the unit into a rocket when the player has the rocket technology, without the unit being an AA gun.  </li>
  If the unit is named exactly "aaGun" then it will require an image called "rockets".  If the unit is named anything else, then it will require an image with "_rockets" appended to its original name. (veqryn [Mark Christopher Duncan])

  <li>- Added new unit attachment, isAAmovement, which when true the unit will follow the rules specified for movement of an AA gun, even if it is not an AA gun, or is a special kind of AA gun. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed issue where battle calc calls with AA units was generating divide by zero. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed bug where battles never ended between units with zero attack/defense power. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new menu option during a game, "Roll Dice...", in the "Game" drop down menu. It allows a player to roll as many dice, with any dice sides, that they want, independant from playing the game. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new unit attachments, <option name="isAAforCombatOnly" value="true"/> and <option name="isAAforBombingThisUnitOnly" value="true"/>, allow units to be AA guns for only certain attack types. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new unit attachments, <option name="attackAAmaxDieSides" value="6"/> and <option name="attackAA" value="1"/>, which allow you to independently set the attack values and max dice sides for AA units. Radar Tech changed to add "1" to the attack values. </li>
  Attack values, including radar, may never go above half of the max dice sides. All attack values (with and without radar) should divide into diceSides without any remainder, otherwise the players will get errors during LowLuck. (veqryn [Mark Christopher Duncan])

  <li>- Fixed a bug where a player with both Mechanized Infantry and Paratroopers technology could no longer do any mechanized infantry movement because the validator was checking for paratroopers first. (veqryn [Mark Christopher Duncan])</li>

  <li>- Created Low Luck for Strategic Bombing and Rockets. New global property, "Low Luck for Bombing and Territory Damage", and new Unit Attachments, bombingMaxDieSides and bombingBonus. Can be used to set different values for strategic bombing and rocket attacks, separate from the rest of the game. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new unit attachment, <option name="givesMovement" value="1:fighter"/>, and global property, "Units May Give Bonus Movement", which allow units to give movement to other units. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed edit mode to allow changing ownership of sea territories, so long as it is not un-owned. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed convoy zone movement validation, and created new global property to manage it: "Naval Units May Not NonCombat Move Into Controlled Sea Zones". Previously was disallowing moves into convoy zones during non-combat, and was marking transported land units as having been in battle. (veqryn [Mark Christopher Duncan])</li>

  <li>- Updates to Pact of Steel 2, so that Japanese make use of isKamikaze and isSuicide. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new unit attachment, isKamikaze, which will allow an air unit to use up all of its movement to go to a battle, if it wants to. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fix for bug 3052260, Ww2v2 revised subs should now roll dice correctly, instead of dying prematurely in cases where the enemy has a destroyer. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed suicide units combat to take into account subs and destroyers. Follows relatively simple rules compared with normal combat. (veqryn [Mark Christopher Duncan])</li>

  <li>- Created new global property, "Defending Suicide and Munition Units Do Not Fire", which when true will stop defending suicide units from acting like suicide units: dying first round, shooting before everyone else. </li>
  So if true, defending suicide units act like normal units, however they still can not be taken casualty to attacks by other suicide units. (veqryn [Mark Christopher Duncan])

  <li>- Fixed various matches and places in the code to do with non-combat units, so that they will now also include isInfrastructure. (veqryn [Mark Christopher Duncan])</li>

  <li>- Finished work on isSuicide, and also created new game property, "Suicide and Munition Casualties Restricted", which stops casualties from returning fire if true. </li>
  Please be aware that the the code in MustFightBattle for these two new features needs to be double checked, especially for multiplayer games. (veqryn [Mark Christopher Duncan])

  <li>- Beginning work on unit attachment "isSuicide", which will allow a unit to die at the beginning of combat. (veqryn [Mark Christopher Duncan])</li>

  <li>- Changed "isInfrastructure" to NOT be bombable. Made it so that "canBeDamaged" is now the switch to make something bombable. (veqryn [Mark Christopher Duncan])</li>

  <li>- Changed "isInfrastructure" to be captured when taken.  isInfrastructure will now be used in place of the planned 'isNonCombat'. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new unit attachment, destroyedWhenCapturedBy, which is a list of players who would destroy a unit rather than capture it. New global property to activate it, "Units Can Be Destroyed Instead Of Captured". (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new unit attachment, maxBuiltPerPlayer, which limits the number of a unittype that can be built for each player. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added history entries for many triggers. (veqryn [Mark Christopher Duncan])</li>

  <li>- Updated ui and utilities to allow islands to be selectable if they are inside a sea zone that ends or begins with "Sea Zone". Previously only allowed water territories to end with, not begin with "Sea Zone". (veqryn [Mark Christopher Duncan])</li>

  <li>- Updated giveUnits and takeUnits to not throw Java errors for older maps. Not backwards compatible, just ignore it if true or false. (veqryn [Mark Christopher Duncan])</li>

  <li>- Dice change: now allows max dice sides to be set in the xml, <diceSides value="6"/>. Defaults to 6 if not present. Can be any number between 1 and 200. This will allow many new types of games to be made. (veqryn [Mark Christopher Duncan] and gansito)</li>

  <li>- Bug fix in Trigger Attachments Tech change, was disqualifying techs based on attached player instead of aPlayer. (veqryn [Mark Christopher Duncan])</li>

  <li>- Redid canBeGivenByTerritoryTo unit attachment to be a colon delimited list of players, who are the players this unit can be given to. Also added a missing toString. (veqryn [Mark Christopher Duncan])</li>

  <li>- Completely redid giveUnitControl to be flexible. giveUnitControl and changeUnitOwners are now lists of players to give to, and a new unit attachment, canBeGivenByTerritory, and a new global property, "Give Units By Territory".  </li>
  takeUnitControl is deleted since no longer needed. This will break compatibility with 2 maps, but I have already updated them, so users just have to update their maps after the next version comes out. (veqryn [Mark Christopher Duncan], with some inspiration from rolflarsson)

  <li>- New game property, "Triggered Victory", and new trigger option, "victory" value = victory message. Can be based on any condition. (veqryn [Mark Christopher Duncan])</li>

  <li>- Dynamix AI patch, various small improvements and logic fixes. (wisconsin)</li>

  <li>- New game property, "Low Luck for Technology", which will apply low luck rules to rolling for tech. (veqryn [Mark Christopher Duncan])</li>

  <li>- Dynamix AI logging patch, should make logs easier to read. (wisconsin)</li>

  <li>- Completely re-wrote NoPuDelegate, and re-wrote the Rules Attachment for productionPerXTerritories. Now looks like: <option name="productionPerXTerritories" value="infantry" count="2"/>, and you can have multiple instances of this. (veqryn [Mark Christopher Duncan])</li>

  <li>- Small bug fix for Support attachments (squiddaddy), and a bug fix for the new placement logic. (veqryn [Mark Christopher Duncan])</li>

  <li>- Dynamix AI patch, adding more features and improving some logic. (wisconsin)</li>

  <li>- New Repair options. New unit attachment: <option name="repairsUnits" value="battleship:bunker"/> will cause the attached unit to repair units in the list. New game properties: "Battleships repair at beginning of round" and "Two HitPoint Units Require Repair Facilities". (veqryn [Mark Christopher Duncan])</li>

  <li>- Created 2 new autosaves: autosave_round_even and autosave_round_odd, which will autosave at the beginning of each round. Provides only the last 2 rounds in order to keep file spam to a minimum. (veqryn [Mark Christopher Duncan])</li>

  <li>- New Carrier-Fighter interleaver for AI casualty selection.  Another patch for Dynamix AI. (wisconsin)</li>

  <li>- Fixed bug where the NoPuPurchase delegate was calling the normal Purchase delegate if the player had PUs left over, Resulting in the player getting multiple purchase screens. (veqryn [Mark Christopher Duncan])</li>

  <li>- New game property, "Unit Placement Restrictions", and new Unit Attachment option, <option name="unitPlacementRestrictions" value="territory1:territory2"/>, prevent a unit or units from being placed in any given territory. (veqryn [Mark Christopher Duncan])</li>

  <li>- Beginning work on Unit Placement Restrictions. (veqryn [Mark Christopher Duncan])</li>

  <li>- Moore AI's casualty picking fixed to work with all maps, not just ww2vX maps. (veqryn [Mark Christopher Duncan])</li>

  <li>- Caching of game data to speed up dynamix ai and multiple battle calcing in one turn.  And another patch for Dynamix AI. (wisconsin)</li>

  <li>- Added new method for Moore AI to move unused transports back to factories. (wisconsin)</li>

  <li>- Fix for Moore AI moving units towards capitals already conquered, and not letting units leave once they get there. (wisconsin)</li>

  <li>- Fix for Null Pointer error in Moore AI's factory movement. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fix for Null Pointer error in Moore AI's movePlanesHomeNonCom. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fix for Moore AI's horrible purchasing of transportable land units, which often resulted in the purchase of no land units. This also fixes the 'moore ai buying too many sea transports' issue. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new method for Moore AI to move landlocked units to coastal territories if amphibious (wisconsin), and fixed the purchasing of Transports to purchase land when needed and transports when needed, hopefully without over-purchasing either. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new option for alliedExclusionTerritories: "controlledNoWater", which will not count water or impassible territories. (veqryn [Mark Christopher Duncan])</li>

  <li>- Major patch for Dynamix AI. Updated battle calc to cache sorted casualty lists. (wisconsin)</li>

  <li>- Created a map skin for Middle Earth based on the alterate relief tiles. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added Middle Earth 12 player map, thanks to original creators: (flanagany & ajmdemen)</li>

  <li>- Balancing changes to Napoleonic Empires, removed a connection, added fortress to majorca, removed tower from catalonia, changed two fortresses in candia into chasseurs. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed battle calc to show correct results in battles where artillery and supportables had same attack power. (veqryn [Mark Christopher Duncan])</li>

  <li>- Changed default casualty picker to choose optimal casualties based on artillery and supportability. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added relief tiles to Pact of Steel. (conarymor)</li>

  <li>- Fixed a bug where Undo-ing the placement of a factory, to a territory that already had a factory, under ww2v3 isSBRAffectsUnitProduction rules, caused max damage to be done to the original factory. (veqryn [Mark Christopher Duncan])</li>

  <li>- Completely re-wrote isConstructions to be completely customizable. Factories now count as constructions when being placed, eliminating placement code specifically for factories. </li>
  New properties for isConstructions: "constructionType" is a string identifying what kind of construction it order to determine stacking, "constructionsPerTerrPerTypePerTurn" and "maxConstructionsPerTypePerTerr" to limit placement.  
  Created a new property called "More Constructions with Factory" as the counterpart to the without factory version.  isConstructions can be any unit, factory, aaGun, airfield, infantry, land unit, etc. (veqryn [Mark Christopher Duncan])

  <li>- Some work on completely rewriting isConstructions. (veqryn [Mark Christopher Duncan])</li>

  <li>- Another patch for Dynamix AI. (wisconsin)</li>

  <li>- Major patch for Dynamix AI, including new settings window to customize in-game certain variables the AI uses. (Wisconsin)</li>

  <li>- Fix for serializing and techs java error. (squid daddy)</li>

  <li>- Added Napoleonic Empires, a beautiful map created by veqryn [Mark Christopher Duncan] and Lssah. Updated to use triggers and combat transports. (veqryn [Mark Christopher Duncan] & lssah)</li>

  <li>- Fix for support/triggers/rules java error. (squid daddy)</li>

  <li>- New player attachments, "destroysPUs", which when set for a player means that player destroys their PUs rather than let them be captured. (veqryn [Mark Christopher Duncan])</li>

  <li>- New player attachments to deal with multiple capitals, "retainCapitalNumber" and "retainCapitalProduceNumber", which be set to the number of capitals need to lose money and gain/spend it respectively. (veqryn [Mark Christopher Duncan])</li>

  <li>- New player rule, "maxPlacePerTerritory", overrides both factory rules and infinite placement. Also fixed a bug in isCombatTransport that stopped the casualty picker from choosing it. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed bunker placement validation to work properly. No longer able to place infinite units by creative clicking orders. Also fixed a bug that allowed infinite placement. (veqryn [Mark Christopher Duncan])</li>

  <li>- Bunker rules allowed by new unit property, isConstruction, and new game properties for it (crystalct), heavily modified and bugs fixed, with updated NWO and POS2. (veqryn [Mark Christopher Duncan])</li>

  <li>- Updating Pact of Steel 2, to take advantage of latest technology list abilities. (veqryn [Mark Christopher Duncan])</li>

  <li>- Patch for technology lists, to allow creation of new technologies and renaming of old ones. Allows adding new technologies by trigger. (squid daddy)</li>

  <li>- Created two new properties for map.properties, "map.showConvoyNames=true" and "map.useNation_convoyFlags=true". If useNation_convoyFlags is true, the flags folder of a game must have "<nation_name>_convoy.png" for each nation with convoys. Convoy names can be moved in name_place.txt (veqryn [Mark Christopher Duncan])</li>

  <li>- Increasing Max Memory to 512mb for linux/mac/windows, and to 192mb for the server. (veqryn [Mark Christopher Duncan])</li>

  <li>- New Property, "Low Luck for AntiAircraft", will turn on Low Luck only for Anti Aircraft shots. (veqryn [Mark Christopher Duncan])</li>

  <li>- Allowed blockade and convoy images to be moved with 2 new txt files: "blockade.txt" and "convoy.txt". Also fixed bug where a convoy zone that was occupied territory displayed the wrong owner, and the bug where a convoy route was displayed as a convoy zone. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added images to be displayed for Blockades. Default image is "blockade.png" in the misc folder of a map. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new unit property, "isCombatTransport", which allows a transport to fight, be taken casualty, and not allow enemies to move through it, under ww2v3 rules. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added new property, "Multiply PUs", which will multiply all PUs gained or lost during a turn, but not yet multiply costs of units, repairs, or starting PUs. (squid daddy)</li>

  <li>- Added Technology Frontiers, and ability to customize which tech is available to which player. (squid daddy)</li>

  <li>- Changed Pact of Steel 2 to take advantage of new Tech choosing attachments. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added a new About... dialog box to main screen. Shows TripleA, engine version, authors, website, as well as a short how-to-play. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added a new AI, Dynamix AI, a scripted AI that seeks to be properly coded and easy to understand, as well as solving all problems in moore ai. (wisconsin)</li>

  <li>- Added some flags made by veqryn [Mark Christopher Duncan], and some by Pulicat. Added "airfield" and "harbour" unit images to all nations, thanks to Hepster. (veqryn [Mark Christopher Duncan])</li>

  <li>- Created Pact of Steel 2, a mod of pos that runs on ww2v3 rules but with drastic changes. Designed to show off every single feature TripleA has to offer on customizing maps. </li>
  Includes detailed notes on each any every property, option, attachment that exists in triplea. Can be used as an example by future map makers on what everything should look like when it works. (veqryn [Mark Christopher Duncan])

  <li>- Added Pact Of Steel map to triplea, thanks to makers: TripleElk and others.  Also fixed baseTiles, updated to current engine. (tripleelk, veqryn [Mark Christopher Duncan])</li>

  <li>- Added New World Order map to triplea, thanks to makers: Sieg, ErnieBommel, and others. Also updated to remove special characters from name and files, and updated to take advantage of Triggers. (sieg & erniebommel, veqryn [Mark Christopher Duncan])</li>

  <li>- Deleted unused uncoded game Properties. (veqryn [Mark Christopher Duncan])</li>

  <li>- Made "LHTR Carrier production rules" completely over-ride the other 4 carrier-fighter properties, that way it is finaly a single switch toggle for the rules-set. (veqryn [Mark Christopher Duncan])</li>

  <li>- Small bug in triggers, production changes were always occuring no matter what, missing brackets. (veqryn [Mark Christopher Duncan])</li>

  <li>- Further updates to Trigger Attachments and Support attachments, as well as creating a new property to turn triggers on and off, defaults to false: "Use Triggers". (squid daddy)</li>

  <li>- Bug fix in alliedOwnership and directOwnership NatObj's use of original and enemy, was returning a list of territories that did not exist. (veqryn [Mark Christopher Duncan])</li>

  <li>- Trigger Attachment and Rules Attachment updates. (squid daddy)</li>

  <li>- Added isLandTransport to support moving isInfantry land units using Mechanized Infantry tech, now separated from canBlitz and isMarine. (veqryn [Mark Christopher Duncan])</li>

  <li>- Minor Updates to Big World and Great War, updates for bugs in the xml as well as small balancing changes. (veqryn [Mark Christopher Duncan])</li>

  <li>- Added Purchases to the Trigger Attachment. (squid daddy)</li>

  <li>- Fixed giving technology to be actually random, as previously when the list was smaller than 6, some techs had a higher chance of getting picked than others. (squid daddy)</li>

  <li>- Changing LHTR Heavy Bombers with Low Luck to give strength+1 instead of 2*strength for attacks, maxing out at max_dice. (squid daddy)</li>

  <li>- Triggered Rule Changes patch added. (squid daddy)</li>

  <li>- Lobby Moderator Enhancement patch added. (wisconsin)</li>

  <li>- Moore AI fix to Rank Territories, was considering islands as being closer to enemy capitols than other territories with a land route. Also much improved the defense of transports and trasporting locations. (veqryn [Mark Christopher Duncan])</li>

  <li>- Moore AI improvement: created a new method so that the AI will attempt to defend the beginning and end of its transport chain. (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed a null pointer errors in Moore AI's rank territories method. (veqryn [Mark Christopher Duncan])</li>

  <li>- Combined isTerritoryEnemyAndNotNuetralWater AND isTerritoryEnemyAndNotNeutral INTO isTerritoryEnemyAndNotUnownedWaterOrImpassibleOrRestricted. (veqryn [Mark Christopher Duncan])</li>

  <li>- New Territory Attachment, blockadeZone, and Unit Attachment, blockade = value, will allow sea units to blockade territories. (squid daddy)</li>

  <li>- national objectives addition of 'uses' and 'atWarPlayers'. Still needs some work on atWar. (squid daddy)</li>

  <li>- directOwnershipTerritories National Objective added, ownership by an ally doesn't count. (astabada/franz)</li>

  <li>- Enhanced Combat Support attachments. (squid daddy)</li>

  <li>- Moore AI purchases tweaking and speeding up. Will no longer consider for purchasing units with zero movement, units with 3 or more attack than defense or defense than attack, </li>
  and units with zero defense, and sea units with 1 movement, if there are 2 movement sea units available. Also now records when it purchases transports in getDidPurchaseTransports(). (veqryn [Mark Christopher Duncan])

  <li>- Null Pointer Exception fix in StrongAI transporting. (veqryn [Mark Christopher Duncan])</li>

  <li>- Moore AI fixes for previous update. (veqryn [Mark Christopher Duncan])</li>

  <li>- Create new CompositeRouteFinder.java, which will find a route based on 3 territory composite matches. (wisconsin)</li>

  <li>- Moore AI fixed several of the reasons why ai can't seem to transport units intelligently or at all. Also made it buy more transports if it needs them. Added new matches and renamed findCertainShips to findTersWithUnitsMatching. (wisconsin)</li>

  <li>- Moore AI out of bounds exception fixed in SUtils.removeUnit(). (veqryn [Mark Christopher Duncan])</li>

  <li>- Moore AI speed fix, and added combined getNeighbors() to GameMap.java. Moore AI now as additional logging properties, comments, and several methods updated to work much faster. (squidbait)</li>

  <li>- New Unit Option: "isAirBase" allows units to scramble to combat (ComradeKev)</li>

  <li>- New Unit Option: "maxOperationalDamage" sets max damage to be sustained before unit is disabled (ComradeKev)</li>

  <li>- New Unit Option: "maxDamage" sets total max damage for a unit (ComradeKev)</li>

  <li>- New Unit Option: "isInfrastructure" infrastructure units can be bombed (ComradeKev)</li>

  <li>- New Unit Option: "isCombatInfrastructure" units can be bombed or taken as casualties in regular combat (ComradeKev)</li>

  <li>- New Property: "Display Units as Counters" (COUNTERS_DISPLAY), will make stacks out of units up to a certain amount. (Edwin van der Wal)</li>

  <li>- Moore AI SUtils fix, findNearest() and distanceToEnemy() completely re-written to be much faster. (squidbait)</li>

  <li>- Moore AI and Easy AI repair rules fix, will now repair intelligently, and never under repair at all, or over repair by more than a couple pu's. (veqryn [Mark Christopher Duncan])</li>

  <li>- Moore AI fixed a bug in SUtils.distanceToEnemy() so that it will return the minimum distance, rather than the first distance it finds. (squidbait)</li>

  <li>- Moore AI will now move factories if they can move them and there is more than 1 in a territory (veqryn [Mark Christopher Duncan]), and some non-combat fixes and logging (squidbait)</li>

  <li>- Moore AI will now bid single units to territories, and bid to all it territories before cycling over to bid to the first one again. Starts with territories touching the enemy. Also fixed a bug in SUtils.distanceToEnemy(). (veqryn [Mark Christopher Duncan])</li>

  <li>- MustFightBattle was removing all movement from all units (including air) that stopped to kill an undefended transport, and should not remove movement of air units. (veqryn [Mark Christopher Duncan])</li>

  <li>- Moore AI and Weak AI fixes, they were not repairing any factories when they had multiple damaged factories. Both will now repair correctly, and limit repairs to half of total PUs, and limit individual factories to a repair of one quarter total PUs. (veqryn [Mark Christopher Duncan])</li>

  <li>- Moore AI fixes, will now return immediately if it has nothing to do for moves and purchasing (wisconsin), and will now repair damaged factories correctly (veqryn [Mark Christopher Duncan]).</li>

  <li>- Moore AI major fix, was considering defender's attack values instead of defense values under some circumstances. Formula to remove casualty units was returning the list as is without properly sorting first, </li>
and was saying that anything with zero attack value has zero rolls in any battles, even if defending. Removed zero-movement units from combat-movement considerations. Also added a debug logger to moore ai properties. (veqryn [Mark Christopher Duncan])

  <li>- Moore AI major fix, was disqualifying all land units from attacking when those land units did not have artillery, isInfantry, or blitz. Much improved performance on 270BC. (veqryn [Mark Christopher Duncan])</li>

  <li>- Moore AI SUtils getExactNeighbors() fix, was returning incorrect data for any distance greater than 2. (veqryn [Mark Christopher Duncan])</li>

  <li>- Moore AI logic fix, calculations for taking enemy capitol with allied help included owned strength when looking at allied strength, also </li>
  getExactNeighbors was returning incorrect data by not fully removing previous iterations (getExactNeighbors still returns incorrect data if distance > 2). (squidbait)

  <li>- Easy AI major fix, was considering all water territories on the map in the list of territories to attack with land units. (veqryn [Mark Christopher Duncan])</li>

  <li>- Easy AI will now purchase units for bid, however it will only purchase land units, and only place them in the capitol. (veqryn [Mark Christopher Duncan])</li>

  <li>- Easy AI bug fix, was purchasing zero units when it had to repair a factory and also had at least 1 other factory with no repairs. Also fixed AI not using all of its money when it had enough left to buy one more unit.  (veqryn [Mark Christopher Duncan])</li>

  <li>- Fixed Moore AI not puchasing anything when it has placeanywhere rules and no factories, and fixed it placing everything inside a capitol which is impassable (bug 2965154), </li>
and fixed a list which was growing indefinitely each round with duplicates, the AI will no longer place in any impassible territory, the AI will not attempt to place factories in territories just conquered, 
and also made further tweaks to the AI (veqryn [Mark Christopher Duncan]).

  <li>- More work on Moore AI's purchasing and placing. Will now sort territories into a list which represents both production ability and closeness to enemy.</li>
AI is now discouraged from buying submarines. And AI will now attempt to buy a factory if it has no factories. (veqryn [Mark Christopher Duncan])

  <li>- Added a swap sides button to the battle calculator, corrected a misspelled class, and reduced default calcs from 5000 to 3000 (dav_eagle)</li>

  <li>- Moore AI purchase fixes. AI was buying factories then trying to place them in water. When rich it was purchasing only the cheapest unit (bug 2989178), </li>
and even when it was supposed to it was not buying any factories. Tried to purchase all air way too often. Was attempting to place factories it did not have. 
Was purchasing specialty units like walls, bunkers, and mortars, way too often. Was not buying factories if the enemy had any units within 3 territories of potential factory territory.
And lots of small tweaks to purchasing algorithm to allow moore ai to work for more maps other than ww2v3, especially bigger maps. (veqryn [Mark Christopher Duncan])

  <li>- Moore AI logic fix, will now attack alone transports correctly, and some small tweaks (veqryn [Mark Christopher Duncan] & wisconsin)</li>

  <li>- Moore AI logic fixes, including amphibious attacks, and clearing of data in loops (squidbait)</li>

  <li>- Small balancing change to minimap.  Russians -6 PUs, Italians +9 PUs. (veqryn [Mark Christopher Duncan])</li>

  <li>- MoveValidator fix, was returning true if route contained subs/trans in part of route, and surface warships in another part of route. (squidbait)</li>

  <li>- logic bug fix for easy ai: it was checking for the att value for def units in territories to walk into. (veqryn [Mark Christopher Duncan])</li>

  <li>- logic bug fix for the weak/easy ai, so that it will not try to move zero movement units. (daral)</li>

  <li>- logic bug fix for the moore ai, which tries to move units out of range. (wisconsin)</li>

  <li>- Adding a browser launcher utility that works with java 5 and 6. (veqryn [Mark Christopher Duncan])</li>

  <li>- Adding buttons to the map download dialog, as well as the lobby menu, that when clicked open a web browser to the </li>
  triplea sourceforge web page for threads on how to download maps, how to host games, and how to report bugs. (veqryn [Mark Christopher Duncan] & bung)

  <li>- Allowing any country name which begins in "AI" to be automatically set to be AI (in addition to "Neutral"). (veqryn [Mark Christopher Duncan])</li>

  <li>- Added a few new properties to start to support next gen engine (ComradeKev)</li>

  <li>- limit status message length and remove combining characters (sgb [Sean Bridges])</li>
 
  <li>- better server side INode validation (sgb [Sean Bridges])</li>

  <li>- fix null pointer when selecting various air transport loads (ComradeKev)</li>

  <li>- Added Great War reliefs (Pulicat)</li>

  <li>- Updated BigWorld game (veqryn [Mark Christopher Duncan], Uboat, Pulicat, and others)</li>

  <li>- fix part of bug 3012752 - unitSupportCount not working (ComradeKev)</li>

  <li>- fix bug 3081799 air units capable of landing on land included in carrier landing calculations (ComradeKev)</li>

  <li>- add SELECTABLE_ZERO_MOVEMENT_UNITS property support (veqryn [Mark Christopher Duncan])</li>

  <li>- fix bug 3043828 pending sea battles with transports causes crash (ComradeKev)</li>

  <li>- set attacking units' movement to 0 when they stop to kill undefended units (ComradeKev)</li>

  <li>- fix bug 3007142 Carriers that are also transports (ComradeKev)</li>

  <li>- fix bug 3028106 fighter landing bug (ComradeKev)</li>

  <li>- another fix for 2998846 & 3012752 Kamikaze fighters and unloaded troop edit-removal (ComradeKev)</li>

  <li>- fix bug 2998846 kamikaze aircraft not working (ComradeKev)</li>

  <li>- add isAirTransport(able) to support air dropping units, now separated from isStrategicBomber (ComradeKev)</li>

  <li>- fix bug 2994004 air landing on newly produced carrier in multi-national SZ disappears (ComradeKev)</li>
 
  <li>- feature request (2799840) add tech tokens to status tab (ComradeKev)</li>

  <li>- update .ico and .png icons (veqryn [Mark Christopher Duncan])</li>

  <li>- feature request add dialog showing results of War Bonds (ComradeKev)</li>

  <li>- fixed load of PacificTest.java (ComradeKev)</li>

  <li>- fix bug 2987400 remove ww2v2 from isNavalBombardCasualtiesReturnFire calculations (ComradeKev)</li>

  <li>- fix bug 2981507 isNeutralsImpassable not considered for air non-combat movement (ComradeKev)</li>

  <li>- fix bug 2975757 paratroops walking on water with movement >1 (ComradeKev)</li>

  <li>- fix bug 2986683 add bombard property to control bombarding attack power (ComradeKev)</li>

  <li>- feature 2802942 artillery supporting >1 inf, defaults to 1 (ComradeKev)</li>

  <li>- feature 2969513 configurable tech roll cost by player, defaults to 5 (ComradeKev)</li>

  <li>- fix bug 2979946 AA Always On only recording last territory casualties (ComradeKev)</li>

  <li>- fix bug 2983390 continued battles (subs) not fought when transport bridge used (ComradeKev)</li>

  <li>- fix bug 2981407 Can't edit-remove transported units (ComradeKev)</li>

  <li>- fix bug 2827064 unload/load trn bug (ComradeKev)</li>

  <li>- fix type in battle screen (Bung)</li>

  <li>- update cruiser and Italian infantry  (veqryn [Mark Christopher Duncan], crystalct)</li>


</ul><h3>Changes for 1.2.5.5 stable</h3><ul>

  <li>- better server side INode validation (sgb)</li>

</ul><h3>Changes for 1.2.5.4 stable</h3><ul>

  <li>- ask users to restart after downloading a map as workaround to 2981890 (sgb)</li>

  <li>- replace japanese_fade gif with png (veqryn [Mark Christopher Duncan])</li>

  <li>- new free french flags (veqryn [Mark Christopher Duncan], crystalct)</li>

  <li>- fix bug 2981512 game hangs during purchase units phase with mooreAI (sgb)</li>

</ul><h3>Changes for 1.2.5.3</h3><ul>

  <li>- fix bug 2979108 Multiplayer LL AA guns Java Error (sgb)</li>

</ul><h3>Changes for 1.2.5.2</h3><ul>

  <li>- fix bug 2977842 Black sea zone movement bug (sgb)</li>

  <li>- fixed bug ConcurrentModificationException (sgb)</li>

  <li>- low luck air now works according the to the veqryn [Mark Christopher Duncan] rules (sgb)</li>

  <li>- validate zip file on map download (sgb)</li>

</ul><h3>Changes for 1.2.5.1</h3><ul>

  <li>- fix bug 2973990 repair rules bug plus new lock not held bug (sgb)</li>

  <li>- fix bug 2969991 lock not held bug, 1.2.5.0 (sgb)</li>

  <li>- fix bug 2970332 low luck aa casualties don't work when movement varies (sgb)</li>

  <li>- fix bug 2971204 moore AI out of bounds exception when no transport rules (sgb)</li>

  <li>- partial fix for bug (2971193) to-hit of 6 causes dump- need to revisit when moving to Dx (ComradeKev)</li>

  <li>- Re-fix bug (2965453) convoy centers/routes with original owners (ComradeKev)</li>

</ul><h3>Changes for 1.2.5</h3><ul>

  <li>- Re-added Japanese_fade.png flag file for use as kamikaze markers in Pacific (ComradeKev)</li>

  <li>- Fix bug (2965453) occupiedTerritoryOf doesn't work with Convoy Centers (ComradeKev)</li>

  <li>- Add new isTransportAndNotDestroyer match so DDs that can transport don't fall into normal transport rules (ComradeKev)</li>

  <li>- Fix bug(2961038) Can transport armor or more than transportCapacity on bomber with paratroops (ComradeKev)</li>

  <li>- fix bug stack overflow in NWO 1.7.7 on Hard AI (sgb)</li>

  <li>- updated german, italian and neutral flags (veqryn [Mark Christopher Duncan])</li>

  <li>- better packaged windows icon file (veqryn [Mark Christopher Duncan])</li>

  <li>- fix bug 2964947, minimap AI error (sgb)</li>

  <li>- allow choosing aa casualty option to work with low luck (sgb)</li>

  <li>- fix crash where unloading attacking transports to allied nations when a defending transport was present and the allied transport dies in the battle (sgb)</li>

  <li>- fix crash with unloading units to multiple allied territories and multiple transports die (sgb)</li>

  <li>- fix low luck aa casualty selection when different plane types are present (sgb)</li>

</ul><h3>Changes for 1.2.4</h3><ul>

  <li>- fix bug (2960696) Strategic Bombing Crash in 1.2.3.0 (sgb)</li>

  <li>- fix bug 2961673 crash in strong ai (sgb)</li>

  <li>- fix bug 2943370, lock not held (sgb)</li>

  <li>- fix exception with casualty selection in low luck (sgb)</li>

  <li>- fix bug in strong ai when there are no transport production rules (sgb)</li>

  <li>- fix null pointer in strong ai (sgb)</li>

</ul><h3>Changes for 1.2.3</h3><ul>

  <li>- fix downloaded map skins (sgb)</li>

  <li>- Add default AI setting for 'Neutral' players in remote games (ComradeKev)</li>

  <li>- remove nwo map in default install, this allows it to be updated independently (sgb)</li>

  <li>- update xml for big world,great war, update misc images for great war, update flags for great war, update italian cruiser image, update chineese and american aa gun,</li>
 add various flags, add various missing units (veqryn [Mark Christopher Duncan], ubernaut, EB (OnanTheBrBr), and U-boat)

  <li>- add optional version number to map listing xml file.  This version number will be saved when the game is downloaded.  When the user is asked to delete</li>
an already downloaded map, the dialog will have the old and new versions in the overwrite message.  Version numbers are 2-4 numbers separated by a '.', eg 1.2, 12.23, 1.2.3, 1.2.3.4  (sgb)

  <li>- Tweaked version error message and aircraft landing on CV validation (ComradeKev)</li>
 
  <li>- Patch bug () Dump in EasyAI non-combat movement (ComradeKev)</li>

  <li>- Patch bug (2953997) Dump in StrongAI non-combat movement (ComradeKev)</li>

  <li>- Fix bug (2955224) Low Luck casualties not being taken (ComradeKev)</li>

  <li>- Fix bug (2951839) reporting that non-blitzed neutrals are charging fee, causing dumps (ComradeKev)</li>

  <li>- Fix bug (2951882) amphib units being ignored (ComradeKev)</li>

  <li>- increase max java memory to 256m (sgb)</li>

  <li>- new icon for triplea.exe (ubernaut)</li>

</ul><h3>Changes for 1.2.2</h3><ul>

  <li>- update flag images in the base flags folder (u-boat,veqryn [Mark Christopher Duncan])</li>

  <li>- allow flag images to be gif or png, gif's will be preferred if both are available to prevent new images in the base folder from overriding images in mods (sgb)</li>

  <li>- Fix null pointer in new AA dice rolling code (ComradeKev)</li>

  <li>- Add default AI setting for 'Neutral' players (ComradeKev)</li>
 
  <li>- Fix bug related to paratroops and blitzing tank movement (ComradeKev)</li>

  <li>- Fix bug (2947241) combined land/amphib blitz with associated sea battle throws exception (ComradeKev)</li>
 
  <li>- Add additional unit png files to most base/images/units folders (ComradeKev)</li>

  <li>- Fix bug (2945150) 'Neutrals Are Impassable' only valid for aircraft (ComradeKev)</li>

  <li>- Fix bug (2943002) AA firing rules with and without low luck (ComradeKev)</li>

  <li>- Fix bug (294300) Victory Conditions tweaked (ComradeKev)</li>

  <li>- Check 'Allied Air Dependents' property to see if allied air can participate in attack (ComradeKev)</li>

  <li>- Fix bug (2936271) Bombers allowed to continue to more battles after dropping (blitzing) paratroops (ComradeKev)</li>
 
  <li>- Fix bug (2939602) Allied fighters on attacking carriers (ComradeKev)</li>

  <li>- Fix bug (2939915) by tweaking route finding logic (ComradeKev)</li>

  <li>- Fix bug (2938275) AA on trns firing at passing aircraft (ComradeKev)</li>

  <li>- Change 'No Economic Victory' game property to 'Economic Victory' (ComradeKev)</li>

  <li>- Fix displayed Victory City victory message (ComradeKev)</li>

  <li>- Fix null pointer if trying to select factory in edit mode (ComradeKev)</li>

  <li>- Update NWO map to version 1.7.2 (OnanTheBrBr)</li>

  <li>- Fix bug (2933998) null pointer in MoreNAble IA Non Combat movement through sea zones (ComradeKev)</li>

  <li>- Fix bug (2933797) Battle Calc in Edit Mode- removed unnecessary checks for edit mode (ComradeKev)</li>

  <li>- Allow submersible subs to travel under enemy ships in combat and non-combat (except DDs) (ComradeKev)</li>

  <li>- Update options panel height to 15 items to fit on smaller screens (ComradeKev)</li>

  <li>- Fix bug (2933341) Exception if paratroop transport cost > bomber capacity (ComradeKev)</li>
 
  <li>- Fix bug (2932947) paratroop checking code allowing naval ships to move through enemy SZ (ComradeKev)</li>

</ul><h3>Changes for 1.2.1</h3><ul>

  <li>- Update game icons (ubernaut)</li>

  <li>- Fix subs being able to move through enemy fleets in noncombat for WW2v2 (ComradeKev)</li>

  <li>- Fix broken code around pacific test cases for new properties (ComradeKev)</li>

  <li>- Remove the hardcoded productionRules for non-sea units during Shipyard initialization (ComradeKev)</li>

  <li>- Fix bug 2925146 options panel overflows screen in a single column (ComradeKev)</li>

  <li>- Fix GameParser to correctly read optional flag for players in the xml playerList (ComradeKev)</li>
  
  <li>- Fix bug 2926226 fighter movement with owned carriers (ComradeKev)</li>

  <li>- Update NWO xml to use the new figher/carrier properties (ComradeKev)</li>

  <li>- Break up Fighter/Carrier production rules into atomic components and added several new game properties for them (ComradeKev)</li>
	Produce fighters on carriers - New fighters can be placed on New carriers
	Produce new fighters on old carriers - New fighters can be placed on Old carriers
	Move existing fighters to new carriers - An existing fighter may be moved to a New carrier from an adjacent territory
	Land existing fighters on new carriers - Existing fighters can end their movement where a new carrier will be placed
  <li>- Add game property support for configurable Victory City thresholds 'xxx Total Victory VCs', 'xxx Honorable Victory VCs', & 'xxx Projection of Power VCs' with xxx being alliance name (ComradeKev)</li>

  <li>- Add support for game property to define economic victory conditions in the form of 'xxx Victory' with xxx being alliance name (ComradeKev)</li>

  <li>- Abstract victory conditions to read teams/players from XML rather than hardcoded values (ComradeKev)</li>

  <li>- Add negateDominatingFirstRoundAttack option for RulesAttachment- negates dominatingFirstRoundAttack for player (ComradeKev)</li>
 
  <li>- Add dominatingFirstRoundAttack option for RulesAttachment- defenders roll at 1 (ComradeKev)</li>

  <li>- Add placementInCapitalRestricted option for RulesAttachment- restricts unit placement to capital (ComradeKev)</li>

  <li>- Add unlimitedProduction option for RulesAttachment- bypasses limitation of unit placement to factory production (ComradeKev)</li>

  <li>- Add 'Neutrals Are Blitzable' property with value of TRUE to NWO (ComradeKev)</li>

  <li>- Fix bug 2919694 non blitzing units allowed to incrementally make 2nd move (ComradeKev)</li>

  <li>- Fix bug (partial) 2860602 Allied air on carriers group together when carriers move through one another (ComradeKev)</li>

  <li>- Fix bug 2922798 transports with mechanized infantry aboard can move 3 spaces (ComradeKev)</li>

  <li>- Fix bug 2921117 can't blitz neutrals- added Neutrals Are Blitzable property (ComradeKev)</li>

  <li>- rename nwo map to new_world_order_eb, this is all lowercase which works on linux, and matches the other map names (sgb)</li>

  <li>- rounded neutral flags (veqryn [Mark Christopher Duncan])</li>

  <li>- Fix bug 2919513 units with 0 attack not getting artillery support (ComradeKev)</li>

</ul><h3>Changes for 1.2</h3><ul>

  <li>- Fix display of factory damage when unit name is "Factory" rather than "factory" (ComradeKev)</li>

  <li>- Add more test cases (ComradeKev)</li>

  <li>- update to Great War 3.0 (Jason Clark)</li>

  <li>- Fix bug 2915452 Shouldn't be able to blitz with non-blitzing units by incrementally moving (ComradeKev)</li>

  <li>- Fix bug 2915057 Bombers shouldn't be able to move then pick up paratroops (ComradeKev)</li>

</ul><h3>Changes for 1.1.2</h3><ul>

  <li>- Add more test cases (ComradeKev)</li>

  <li>- Upgrade NWO to NWO EB (OnanTheBrBr)</li>

  <li>- Fix bug 2909898 2-move units allowed to move 'through' enemy forces (ComradeKev)</li>

  <li>- Fix test cases for LHTR rules revisions below (ComradeKev)</li>

  <li>- Fix bug 2905542 LHTR HB not adding +1 to SBR rolls (ComradeKev)</li>

  <li>- Fix bug 2908897 occupiedTerrOf not working when liberating allied capital (ComradeKev)</li>

  <li>- fix null pointer in move with Twilight Imperium (sgb)</li>

  <li>- Create/use Properties for various entries in Constants for consistency (ComradeKev)</li>

  <li>- Fix invalid property used in isTransportUnloadRestricted of TransportTracker (ComradeKev)</li>

  <li>- Fix bug 2907042 Revised submerged subs don't fight in subsequent defending battles (ComradeKev) </li>

  <li>- increase download map panel size (sgb)</li>

  <li>- if a url in the download games xml starts with !, ignore it and disable download button.  this allows better formatting  (sgb)</li>

  <li>- game engine prevents ai from repairing a territory more than the number of times it was hit (sgb)</li>

  <li>- fix bug 2899005, Long air range icon works only with "fighter" and "bomber" (sgb)</li>

  <li>- fix bug 2905298, Wrong message Cant place sea unit on land (sgb)</li>

  <li>- fix bug 2905986, occupiedTerrOf don't work with capital (sgb)</li>

  <li>- skins can be downloaded/read from the users map folder (sgb)</li>

</ul><h3>Changes for 1.1.1</h3><ul>

  <li>- new neutral flag images (veqryn [Mark Christopher Duncan])</li>

  <li>- allow users the option to replace downloaded maps when downloading (sgb)</li>

  <li>- don't allow downloading a map with the same name as one that comes with the default TripleA install (sgb)</li>

  <li>- fix bug 2893890, fighters with no movement left can hover in sea zones where carriers can be placed (sgb)</li>

  <li>- fix bug 2887488, Add "Display Sea Names" property to display sea zone names (ComradeKev)</li>
 
  <li>- Add 'Multiple AA Per Territory' property (ComradeKev)</li>
 
  <li>- Fix nonCombat movement into enemy SZ 2 zones away (ComradeKev)</li>

  <li>- Remove Economic Victory from NWO, Great War, and Big World (ComradeKev)</li>

  <li>- Add French Rocket to NWO units (ComradeKev)</li>

  <li>- Fix WW2V3_Tech_Model constant (ComradeKev)</li>

  <li>- Fix buyCruiserIndustrialTechnology unit for Big_World (ComradeKev)</li>

  <li>- Various map utility fixes (Stephen Wicklund)</li>

  <li>- Right clicking on center picker removes the dot (Stephen Wicklund)</li>

  <li>- Center picker displays the name of the center next to the dot (Stephen Wicklund)</li>

  <li>- Fix bug in getStrengthOfPotentialAttackers for planes. Reduced frequency of tech purchase. (Kevin Moore)</li>

  <li>- fix bug 2831083, WW2V3: Retreat from undefended transports (sgb)</li>

  <li>- fix bug 2892836, aa radar in low luck (sgb)</li>

  <li>- fix bug 2893144, null pointer on startup (sgb)</li>

  <li>- fix bug 2898135, where unloaded infantry could move as mechanized infantry (sgb)</li>

  <li>- various paratrooper fixes (sgb)</li>

  <li>- fix bug 2892469, paratroops in first enemy territory (sgb)</li>

  <li>- StrongAi, Cleaned out unused code. Minor tweak to getStrengthOfPotentialAttackers. (Kevin Moore)</li>

  <li>- Fix bug in zip url parsing (Stephen Gallagher)</li>

  <li>- StrongAi, Fix bug in ship movement. Modify territory selection for non-combat transports (Kevin Moore)</li>

  <li>- fix bug where paratroops could walk on water, bug 2867358 (sgb)</li>

  <li>- remove isParatroop UnitAttachmant property. (sgb) </li>

  <li>- fix Allied fighter on AC bug, bug 2890919 (sgb)</li>

  <li>- fix infinite loop in odds calculator, bug  2853353 (sgb)</li>

  <li>- better logic for determining which odds calculator player should be used if no units are in the territory (sgb)</li>

  <li>- better isolation of units in odd calculator from units in the game (bug 2820761) (sgb)</li>

  <li>- download file notes shows top of notes by default now, rather than scrolling to the middle (sgb)</li>

</ul><h3>Changes for 1.1.0</h3><ul>

  <li>- update StrongAI files for PUs (ComradeKev)</li>

  <li>- update to substance 5.3 (sgb)</li>

  <li>- remove troublesome maps (sgb)</li>

  <li>- Add code to allow downloading and installing games from the network.  An Exampe site is here, </li>
  http://sites.google.com/site/tripleadownloadexamples/    (sgb)

  <li>- add utility for updating game.xml files (sgb)</li>

  <li>- Strong AI Changes  (Kevin Moore)</li>
  -Handles Neutrals correctly.
  -Switched all decision making to a territory ranking system which is consistent throughout the AI
  -Eliminated expectations that movement will be under revised/AA50 limits.
  -Cleaned up handling of units around a threatened capital
  -Improved blitzing and transport invading


  <li>- Scrub Production Units (PUs)(ComradeKev)</li>

  <li>- Fix bug 2827014 Air forces route through impassables if length = valid sea route (ComradeKev)</li>

  <li>- Fix bug 2829876 BB bombards when only air attacking from SZ (ComradeKev)</li>

  <li>- Fix bug 2827394 renamed Neutral.GIF to Neutral.gif (ComradeKev)</li>

  <li>- Fix  bug 2820547 faulty mechanized inf and paratroop capacity (ComradeKev)</li>

  <li>- Scrub xml and source (ComradeKev)</li>

  <li>- fix bug 2818614 include substance jar in build.xml (Seidelin)</li>

  <li>- fix bug 2818578 partial amphib attack with air asked to retreat twice (Seidelin) </li>

  <li>- fix bug 2820382 Undoing/redoing amphibious attack can allow too many bombard (Seidelin)</li>

  <li>- Don't allow aa guns in blitzed territories to fire rockets (sgb)</li>

  <li>- Improved land and sea unit purchasing. Changed parameters on factory purchase. Extensively modified ship handling in combat and non-combat. Modified battle prediction to improve land unit attack. (Kevin Moore)</li>

  <li>- fix bug 2818023 again moving unit to carried-over battle causes existing units to be ignored (ComradeKev)</li>

  <li>- new flag images for Italy and Russia (U-Boat)</li>

  <li>- fix partially repaired factories showing as completely repaired (ComradeKev)</li>

  <li>- Changed testCanRetreatIntoBlitzedTerritory() to allow retreat into blitzed territory (ComradeKev)</li>

  <li>- fix bugs 2815448 defending subs not getting sneak attack (Seidelin) </li>

  <li>- fix bug 2813511 naval units not asked to retreat (Seidelin)</li>

  <li>- fix bug 2807885 fighters asked which transport to load (Seidelin)</li>

  <li>- Partial refactor of validateAirCanLand (ComradeKev)</li>

  <li>- add isInfantry marker to infantry units for all mods (sgb)</li>

  <li>- fix bug where strat bombers hit by aa en route to a battle lives (sgb)</li>

  <li>- fix bug 2816632 Marine unit doesn't work with LL (sgb)</li>

  <li>- fix bug 1888062 multinational transport bug (sgb)</li>

  <li>- remove non working "Use Destroyers and Artillery" in Iron Blitz (sgb)</li>

  <li>- fix bug 2815448, Defending subs don't get sneak defense (sgb)</li>

  <li>- fix bug 2803021, NWO PUs to spend don't display (sgb)</li>

  <li>- move copies of blank_relief to images/relief tiles, this allows all maps to share a copy (sgb)</li>

  <li>- change labels/dialog on repair screen to make it clear we are not purchasing units (sgb)</li>

  <li>- fix bug 2802962, bug where units loaded onto transports in a pending battle zone do not die when their transports do (sgb)</li>

  <li>- fix bug 2807875, Factories count towards production limit (sgb)</li>

  <li>- fix bug 2815801 Bid placement Error (sgb)</li>

  <li>- Complete gutting of NonCombatMoveSea; Removed most plane analysis code and replaced with calls to invitePlaneAttack in SUtils; </li>
  tweak to purchasing when resources are high to help with other maps; 
  prepared code for purchasing units for the best transport attack (Kevin Moore)

  <li>- Add some missing units for NWO and activate tech for extra 4 players in NWO-9 (ComradeKev)</li>

  <li>- Check if SBR damages unit production before displaying factory damage (ComradeKev)</li>

  <li>- Fix bug 2801738 just use Infantry instead of chineseInfantry so they stack properly (ComradeKev)</li>

  <li>- Add victory conditions to game notes (ComradeKev)</li>

  <li>- Add NOs to game notes for AA50 (ComradeKev)</li>

  <li>- Fix bug 2807397 Revise NWO 9 Player placements for E/W Romania (ComradeKev)</li>

  <li>- Fix number of paratroops shown loading on to bomber (ComradeKev)</li>

  <li>- Change default route finding to try land routes first (ComradeKev)</li>

  <li>- Fix allMatch and someMatch returning true on empty collections (ComradeKev)</li>

  <li>- Add victory conditions to game notes (ComradeKev)</li>

  <li>- Enable turning on/off relief tiles on AA50 (ComradeKev)</li>

  <li>- Add Relief Tiles for AA50 (Much thanks to Imperious Leader)</li>

  <li>- Fix bug 281534 fighter movement calculation (ComradeKev)</li>

  <li>- Moved capitol markers to better fit with AA50 reliefs (BraveHamster)</li>

  <li>- Fix bug 2810759 Non-amphib units taken as casualties before amphib units (Seidelin)</li>

  <li>- Fix bug 2807878 Planes attacking w/ amphib units can't retreat (Seidelin)</li>

  <li>- Strong AI fix bid purchasing and put in code for blitzing empty territories (Kevin Moore)</li>

  <li>- show line/column of xml errors when a game fails to parse (sgb)</li>

  <li>- Modify AI: Apply purchasing changes to sea units (Kevin Moore)</li>

  <li>- Show user ip/port lobby server tries to connect to when hosting a game fails because the computer is not reachable from the lobby server (sgb)</li>

  <li>- Modified AI: purchasing for seaLion, improved blitzing, tweaked combat and non-combat to better protect capitals and factories, add comments in SUtils (Kevin Moore)</li>

  <li>- fix bug 2808834 online games suddenly fail (sgb)</li>

  <li>- fix bug 2806095, missing files in mac build (sgb)</li>

  <li>- Add some test cases</li>

  <li>- Fix bug 2459410 Fighters on carriers with allied fighters can't attack (ComradeKev)</li>

  <li>- Fix bug 2807115 Air improperly calculating max distance with existing carriers (ComradeKev)</li>

  <li>- Fix exceptions when undoing a paratroop attack move (ComradeKev)</li>

  <li>- Fix aircraft being able to fly too far when building carriers (ComradeKev)</li>

  <li>- Fix bug 2806723 ships allowed to move through enemy navies during combat move (ComradeKev)</li>

  <li>- Fixed stopping in zone with ignored units causes movement to end (ComradeKev)</li>

  <li>- Added AA50 Technology Tree to game notes (ComradeKev)</li>

  <li>- Check defending units for attack power before popping kamikaze message (ComradeKev)</li>

  <li>- Add method to land paratroops (remove dependence on bombers) (ComradeKev)</li>

  <li>- Fix 1 AA hit kills all paratroops (ComradeKev)</li>

  <li>- Fix paratroops refusing to fight (ComradeKev)</li>

</ul><h3>Changes for 1.0.3.4</h3><ul>

  <li>- Better internet ip detection (sgb)</li>

  <li>- Fix bug where a territory could not be strategic bombed and conquered in the same turn (sgb)</li>

  <li>- Fix bug 2804677 Retreating into enemy spaces (sgb)</li>

  <li>- Add menu to change look and feel (sgb)</li>

  <li>- Fix bug 2799810  Admin right-click menu (sgb)</li>

  <li>- Fig bug 2801742 Rockets throw error in NWO (sgb)</li>

  <li>- Fix bug 2801740 java error in every roll in a PBEM game. (sgb)</li>

  <li>- Fixed not being able to place bid units at non-factories (ComradeKev)</li>

  <li>- Fix bug 2675636 Crash when ignoring enemy units (ComradeKev)</li>

  <li>- Fix bug 2779955 Cause battle when new/ignored units are in contested zones (ComradeKev)</li>

  <li>- Minor change to the Strong AI calculation of the strength of sea units near a territory (Kevin Moore)</li>

  <li>- Fixed the connections or E/W Romania in NWO9 (ComradeKev)</li>

  <li>- Added name_place.txt for NWO (ComradeKev)</li>

  <li>- Updated rockets.png for Russians in NWO (ComradeKev)</li>

  <li>- Fixed some connections in Europe.xml (ComradeKev)</li>

  <li>- Added name_place.txt for Europe (ComradeKev)</li>

  <li>- Fixed neutrals not able to be captured after a failed attempt (ComradeKev)</li>

</ul><h3>Changes for 1.0.3.3</h3><ul>

  <li>- put game name in window title (sgb)</li>

  <li>- fix bug 2753571 - Unloaded cargo not being removed when transport sinks, also odds calculator fails with transports in revised (sgb,  gruetzdark)</li>

  <li>- fix bug 2779959 - Stay in the Mobilization Zone (sgb)</li>

  <li>- fail when loading game where xml case and file name case differs (sgb)</li>

  <li>- fix map name/unit case in nwo maps (sgb)</li>

  <li>- mark territories with battles (sgb)</li>

  <li>- Make it so map utility programs can find the centers, polygons, and map.properties files by using the</li>
  path of the map's image file. (Stephen Wicklund)
  
  <li>- Make it so the user can specify the unit's scale when using the 'Auto Placement Finder' utility.(Stephen Wicklund)</li>

  <li>- add a setting to "Lock" the map, so you can observe a game without the map moving all around (Stephen Wicklund)</li>

  <li>- add  a setting to suppress the showing of battles between two AIs (Stephen Wicklund)</li>

  <li>- add a setting to choose how long the AI pauses between each movement (Stephen Wicklund)</li>

  <li>- add a better ai (Kevin Moore)</li>

  <li>- limit number of units in one row of production panel to 8 (sgb)</li>

  <li>-  The following list of bugs were fixed- (Comradekev)</li>
	Fix the engine forcing the repair of at least 1 damage
	Amphib units taken as first casualties if partial retreat is possible
	Fix subs blocking naval bombardment
	Fix paratroop code (die with AA casualties, retreats, non-dependent in regular combat)
	Fix AARadar not inflicting casualties on aircraft
	Fix disappearing fighters on combined US/China turn
	Fix factories with PU value <3 shouldn't get Increased Production bonus
	Fix warships allowed to battle subs/trns, then move in noncombat movement
	Fix error generation when placing IC, undoing it, then trying to re-place it
	Fix error generation when trying to place both new fighter and CV in sea zone
	Fix Null Pointer when trying to edit a sea zone owner
	Fix US being able to place an IC in a newly captured territory 
	Fix NWO territories Romania, Czech., Normandy, and Le Harve.
	Multi-player transport fleets throw - 'wrong number of casualties selected' error
	Ask if BB/CR should bombard
	Add ability to ignore defending Trns
	Fix NWO map names
	Add damage totals to factory icons (black text)
	US units that move into enemy occupied SZ in non-combat (trn/sub) fight during Chinese combat
	Fix null pointer when loading maps with 'Show Map Blends' selected on the View menu

</ul><h3>Changes for 1.0.3.2</h3><ul>

  <li>-  The following list of bugs were fixed- (Comradekev unless otherwise specified)</li>
	Darkened/moved Italian flag (Seidelin)	
	Tech tokens not removed from client after successful roll (Seidelin)
	Factories not repaired on Client
	Not charged for tech rolls 
	Out of Bounds exception thrown when trying to save games (all games)
	Fix Null Pointer when selecting 'do not attack' subs
	Transports with cargo blocking movement
	Can't build new fighters on old carriers
	Defending carrier with fighters aboard- fighters don't return fire in 1st combat round
	Defending subs should be able to return sneak attack fire
	Transports killed after subs submerge
	Transports/subs causing Itialian NO to not be met
	Repairing multiple factories is buggy
	Defending fighters should be allowed 1 move if their CV dies
	US/China combined turn
	
Added New World Order 5 and 9 player games (Sieg)
	Added relief map and blending support to NWO map (ComradeKev)

</ul><h3>Changes for 1.0.3.1</h3><ul>

  <li>- update docs to correct how to run TripleA from the command line using the ant run command.</li>

  <li>- The following list of bugs were fixed- (Comradekev)</li>
	Move Chinese capital to impassable neutral so any time a Chinese terr is liberated, it goes to China
	Some dialogs not appearing on Client computers
	Paratroops should be able to overfly blitzed territories
	Factory repair charges not being applied
	Use allied AA in a territory if they have Radar
	Limit max damage from rocket attacks
	Fix the UK nat'l objective
	Technology throws exceptions 
	Add useTech option for all games
	Allow new AA to be placed if there's already one in the terr
	Fix null pointers when transporting units
	Allow partial retreat for a combined amphibious assault
	Defending subs should be able to return fire befor applying sneak attack casualties
	Pathfinding uses impassables
	Allow loading of Trns in SZ with enemy subs
	Consider carrier route (can't go on land) when attempting to find landing spots for fighters
	Add ability to pre-set techs 
	Remove SBR raid from blitzed territory
	Allow amphib assault w/o having to combat sub-only forces
	Fix bomber -v bomber comes to stalemate after one round of combat
	Fix defending subs still firing after submerging
	SBR throws null pointer in edit mode
	Hosted games show more hits than units when transports present
	Hosted games throw exceptions when undoing transport moves
	Fix air not firing at subs when accompanying DD dies 
	Fix client game factories not repaired
	Disallow blitzing through AA and factories
	Fix low luck AA not inflicting damage
	Fix 'Attack Subs' dialog only showing up on Host
	Fix surface ships being allowed to move into enemy SZ during non-combat
	Add option to continue after victory for all games
	Fix exception on host when getting technology
	Fix partial retreat from amphib assault not working
	Should be able to stop in SZ with a trn/sub, then continue trip
	Add dialog to disallow file names with slashes
	
  <li>- Fix for tech tokens (Seidelin)</li>
	
  <li>- Add ShowMapOnly mode for passively viewing games (Smutt) </li>

  <li>- Added 'Neutrals Are Impassable' property to eliminate neutrals from pathfinding (ComradeKev)</li>

  <li>- on windows, put saved games in users home folder, rather than the triplea install directory.  this works better on Vista. (sgb)</li>

  <li>- fix [ 1945380 ] battle calculator window buttons lost (sgb)</li>

  <li>- update launch4j generated exes to use launch4j 3.0.1 (sgb)</li>

  <li>- updated embedded jre to 6_11 (sgb)</li>

</ul><h3>Changes for 1.0.3.0</h3><ul>

  <li>- Disable game properties button if there are no game properties (Chris McIntosh)</li>

  <li>- Fix spelling in classic xml (Chris McIntosh)</li>

  <li>- The following list of bugs were fixed- (Comradekev)</li>
	#2554414 Only one Mechanized Infantry per tank should be allowed
	#2554418 Jet Fighters not attacking at 4
	Games throw exceptions when trying to affect Tech Tokens
	Chinese unit max for territory placement not limited to Chinese-only units
	Territory Turn Limit removed from options
	Option added for inclusion of Tech development
	China should be able to place units on newly captured territories
	Added Japanese Inf in Solomon Islands (aa-42)
	Fix null pointer when choosing NOT to attack subs
	Paratroops should be limited to 1 per bomber
	Bombers should not be able to move before picking up paratroops
	Radar/damaged factory icons not displaying
	Fix factory repair cost for Increased Factory Production technology
	#2474056 Captured AA ownership
	#2554411 Rockets allowed to overfly impassables
	#2554412 Rockets firing after Non-Combat move 
	#2554419 Factory repair costs with Enhanced Production technology
	Factories added with edit mode are damaged
	Should allow more than 1 AA in a territory for some games
	Should be able to place in enemy occupied sea zones
	Added stalemate condition for trn -v trn battles
	Low-Luck AA support for RADAR tech
	Mechanized Inf should be able to blitz
	AA hits separated for combined fighter/bomber groups
	
  <li>- 2006022 Undo movement jumps back to top of list (Chris McIntosh)</li>

  <li>- 1910223 Ability to cancel odds calculator (Chris McIntosh)</li>
	
</ul><h3>Changes for 1.0.2.0</h3><ul>

  <li>- Maps images, and XML for AA50 (Zero Pilot and Black Elk)</li>

  <li>- Update game notes (sgb)</li>

  <li>- Better error message if no server properties for this version (sgb)</li>

  <li>- Mods can now be installed without unzipping anything.  Simply create a zip file with contents that look like any of the folder in maps. (sgb) </li>

  <li>- Add new Game chooser dialog that shows games notes. (sgb)</li>

  <li>- Move xml files from games folder to /maps/<mapName>/games.  For example, revised.xml is now in maps/revised/games (sgb)</li>

  <li>- Add chat ignore feature, thanks to Tango for the icon - http://tango.freedesktop.org/Tango_Icon_Library (sgb)</li>

  <li>- Add full TripleA 50 support (ComradeKev)</li>
    MUCH thanks to Seidelin for playtesting!

  <li>- Add Choose AA Casualties property (value=true) to Revised.xml (President Douchebag)</li>

  <li>- Break up rulesets into individual rules (while keeping overall ruleset setting) (ComradeKev)</li>

</ul><h3>Changes for 1.0.1.4</h3><ul>

  <li>- Add blank_relief.png to various maps to fix exceptions and fix misspellings in POS *.txt files (ComradeKev)</li>

  <li>- Fix bug [ 2153973 ] BattleCalc during EDIT hangs the game (ComradeKev)</li>

  <li>- Fix bug [ 1228661 ] Fighters can't move to combat unless carrier moves in range (ComradeKev)</li>

  <li>- Fix bug [ 1951595 ] edit mode, fgt and inf placement in sz (ComradeKev)</li>

  <li>- Tweak blending code to account for missing base/relief tiles (ComradeKev)</li>
	Map makers need to include a blank_relief.png file, nothing extra is required for base tiles.

</ul><h3>Changes for 1.0.1.3</h3><ul>

  <li>- When executing sql in headless lobby, show error messages on the console (sgb)</li>

  <li>- Update Great War map to remove small country markers (Jason Clark)</li>

  <li>- Add Revised relief tiles (Zero Pilot)</li>

  <li>- Update Revised colors (President Douchebag)</li>

  <li>- Set max memory for mac release (sgb)</li>

  <li>- Fix abend when there are no original owners in a territory (ComradeKev)</li>

  <li>- Change so only original owner gets the faded kamikazi zone marker (ComradeKev)</li>

  <li>- Fix display of Convoy Route text (ComradeKev)</li>

  <li>- Fix PlacementPicker abends (ComradeKev)</li>

  <li>- Fix Null Pointer [ 1068223 ] for non-required files in AutoPlacementFinder app (ComradeKev)</li>

  <li>- Fix bug [ 1937303 ] casualty window shows all casualties as defending nation (ComradeKev)</li>

  <li>- Fix bug [ 2066114 ] Industrial Tech advancement crashes stats tab (President Douchebag)</li>

  <li>- Add code to identify offending territory in AutoPlacementFinder exceptions for centers.txt (ComradeKev)</li>

  <li>- Add code to allow Relief Map Blending (Overlay, Linear_Light, Multiply, Difference) via map.properties settings includes 3 parameters (ComradeKev) </li>
	map.mapBlends=true
	map.mapBlendMode=Linear_Light
	map.mapBlendAlpha=0.5f
	
</ul><h3>Changes for 1.0.1.2</h3><ul>
  <li>- Fix territory connections in Pacific</li>

  <li>- Fix bug where hasLandRouteToEnemyOwnedCapitol causes abend for players with no Capital.  Returns none for 'optional' players</li>

  <li>- Re-create code to change ownership of units so British/Australians can play on same turn in pacific</li>

  <li>- Fix thrown exception with neutral blitz/flyover. (Comradekev)</li>

  <li>- Fix bug [ 2005292 ] LHTR planes not able to land on produced carriers. (ComradeKev)</li>

  <li>- Add ability to manually select AA casualties via "Choose AA Casualties" game property. (President Douchebag)</li>
  
  <li>- Fix bugs [ 1668008 & 1683940 ] Fighter ability to move one space to land when CV is sunk (ComradeKev)</li>

  <li>- Fix territory connections in Pacific (ComradeKev)</li>

  <li>- Fix bug [ 1809209 ] transport retreat/die after unload leaves unloaded units in place (ComradeKev)</li>

  <li>- Change BattleStepStrings names to match text for clarity (ComradeKev)</li>

  <li>- fix null pointer that leads to potential lobby crash (sgb)</li>

  <li>- update great war map (Jason Clark)</li>

</ul><h3>Changes for 1.0.1.1</h3><ul>

  <li>- Replace code for using the Large flags for Capital markers and tweak their placements in Pacific (ComradeKev)</li>

  <li>- Fix abend when capturing Commonwealth Convoy Center (player with no capital) (ComradeKev)</li>

  <li>- allow lobby server to run in headless mode  (sgb)</li>

  <li>- fix lobby.properties. If a lobby.properties file is in the root TripleA directory, use that to connect to the lobby (sgb)</li>

  <li>- reduce lobby backup frequency to 7 days (sgb) </li>

</ul><h3>Changes for 1.0.1.0</h3><ul>

  <li>- Fix bug [ 1830015 ] transport load/unload after being in combat (ComradeKev)</li>

  <li>- Add Convoy Centers & Convoy Routes, as well as labels (ComradeKev)</li>

  <li>- Add Tokyo Express - Ability for DDs to carry one inf in Pacific (ComradeKev)</li>

  <li>- Fix amphib marines combat display  (ComradeKev)</li>

  <li>- Add name_place.txt for pacific to clean up territory name placement (ComradeKev)</li>

  <li>- Add Australian player purchases (units transferred to British control for combined play after buy) (ComradeKev)</li>

  <li>- Add Australian capital and territories (ComradeKev)</li>

  <li>- Add partial support for Commonwealth Convoy Center cash distribution (ComradeKev)</li>

  <li>- Add Naval and Air bases (ComradeKev)</li>

  <li>- Add partial support for Kamikazi zones (ComradeKev)</li>

  <li>- Fix lhtr strategic bombing (dav eagle2)</li>

  <li>- fix [ 2015235 ] Compilation error under OpenJDK (karrde712)</li>

</ul><h3>Changes for 1.0.0.3</h3><ul>

  <li>- allow factories with non 0 movement to move (sgb)</li>

  <li>- update great war to 2.2 (Jason Clark)</li>

</ul><h3>Changes for 1.0.0.2</h3><ul>

  <li>- Fix dice click problem, reopen bug [ 1673719 ]  right-click-drag should not deselect unit upon release (sgb)</li>

  <li>- Fix bug where selecting unit and transports and moving to a sea zone may move a transported unit more than once (sgb)</li>

  <li>- Fix bug  [1988219] lhtr fighters cant land on new carriers (sgb)</li>

</ul><h3>Changes for 1.0</h3><ul>

  <li>- add tdice dice servers (sgb)</li>

  <li>- lock warnings don't show error dialog (sgb)</li>

  <li>- fix bug [ 1962058 ] fighter move in non combat (sgb)</li>

  <li>- allow selection of text on chat panel (sgb)</li>

  <li>- remove non existent irony dice server (sgb)</li>

</ul><h3>Changes for 0.9.4.2</h3><ul>

  <li>- in edit mode, don't always ask the user to choose the units to remove (sgb)</li>

  <li>- add game id, to be used in future pbem server (sgb)</li>

  <li>- remove uneeded base tiles, this fixes the white space near algeria (sgb)</li>

</ul><h3>Changes for 0.9.4.1</h3><ul>

  <li>- fix bad anti aliasing effects when scaled at 100% (sgb)</li>

  <li>- increase max heap size to 196M (sgb)</li>

</ul><h3>Changes for 0.9.4</h3><ul>

  <li>- simplify right click map dragging (sgb)</li>

  <li>- reorganize menus slightly, add export menu (sgb)</li>

  <li>- turn antialiasing on for map drawing, makes scaling look better on windows (sgb)</li>

  <li>- fix spelling mistakes in revised (zero pilot)</li>

  <li>- updated revized map (zero pilot)</li>

  <li>- fix bug 1890628 freeze in triplea 0.9.3 (sgb)</li>

  <li>- fix bug 1905413 can't move units with a warning (sgb)</li>

  <li>- fix bid (all bid PUs were being added to the player) (sgb)</li>

  <li>- In europe incomplete, changed the transport cost of artilery to 2, so 2 may be transported (comradekev)</li>

  <li>- fixed bug[ 1896778 ] In Pacific game cannot move between sea zone 37 and Kiangsi (comradekev)</li>

  <li>- fixed bug [ 1910221 ] Undone Movement Null Pointer (sgb)</li>

  <li>- update great war to version 2.0 (Jason Clark)</li>

  <li>- fix highlight unit drawing bug (sgb)</li>

  <li>- fix null pointer when ai plays in capture the flag (sgb)</li>

  <li>- improved game notes button (sgb)</li>

  <li>- fix null pointer when attacking neutral countries (sgb)</li>

  <li>- add ant run command for running from command line (sgb)</li>

</ul><h3>Changes for 0.9.3</h3><ul>

  <li>- fix [ 1870424 ] can't leave tic tac toe game after the game is over, also fix tic tac toe networked mode (sgb)</li>

  <li>- disable main button on startup screen, as it overrides send message send (sgb)</li>

  <li>- more PBEM posting fixes (tclayton)</li>

  <li>- re-add screenshot overlay settings to map.properties in revised (tclayton)</li>

  <li>- fix bug [ 1860285 ] solutions chooser offers no solutions (tclayton)</li>

  <li>- fix bug [ 1851498 ] id should not be required in pbem games (tclayton)</li>

  <li>- fix bug [ 1668015 ] disallow neutral territories in route in revised (tclayton)</li>

  <li>- fix bug [ 1878700 ] edit mode: remove unit bug (tclayton)</li>

  <li>- fix bug [ 1875092 ] Missing "No place for unit to land" warning (tclayton)</li>

  <li>- fix bug [ 1862922 ] foreign planes on carrier (tclayton)</li>

  <li>- fix [ 1867299 ] Initial industrial complexes have limited production (comradekev)</li>

  <li>- fix bug [ 1746101 ] defending units in pacific show incorrectly in battle display (comradekev)</li>

  <li>- change Load new game to Choose Game on startup screen. (sgb)</li>

  <li>- fix bug [ 1855420 ] Unable to move fighters during non-combat movement (tclayton)</li>

  <li>- fix bug [ 1856374 ] movement panel crash (tclayton)</li>

  <li>- put engine version in system properties for debugging (sgb)</li>

  <li>- mark kamikaze moves as such in the history (sgb)</li>

  <li>- fix bug [ 1856656 ] IllegalState exception (sgb)</li>

  <li>- disable chat time menu in non networked games (sgb)</li>

  <li>- add limited chat flood control (sgb)</li>

  <li>- [ 1837246 ] deploy troops phase window behavior (sgb)</li>

  <li>- fix bug [ 1855427 ] submerged subs prevent air units from moving (sgb)</li>

  <li>- add japanese, british, russions rockets, australian, canadian, neutral puppet state marine and neutral cruiser unit images (zero pilot)</li>

  <li>- use rocket images when a player has rocket tech advance (sgb)</li>

</ul><h3>Changes for 0.9.2</h3><ul>

  <li>- fix bug where if your capital fell, and you captured another players capital, you could buy units (sgb)</li>

  <li>- PBEM posting fixes and cleanup (tclayton)</li>
  <li>-   don't proxy PBEMMessagePoster, remove serialization (was broken in multi-player)</li>
  <li>-   fix EndTurnDelegate serialization</li>
  <li>-   only show Turn Summary Posting widgets if posting is enabled</li>

  <li>- fix bug [ 1825831 ] in multiplayer mode, all players can edit (tclayton)</li>

  <li>- fix bug [ 1825841 ] comment mode split bar visible (tclayton)</li>

  <li>- WeakAi improvements (masch)</li>
  <li>-   fix in land route calculation (does not take neutrals into account)</li>
  <li>-   improvement in Non-combat move. Moves towards enemy territories even if there are no units.</li>
  <li>-   purchase 20% transports if player is amphibious. Can boost that - buy</li>
  <li>-   only transports if landing point is heavy armed e.g. UK or Japan</li>
  <li>-   Try to capture unprotected land in amphibious combat ( 1 transport on different route )</li>
  <li>-   Ignore channel feature for sea routes, if endpoint is on channel territory ( otherwise you cannot attack that)</li>

  <li>- patch [ 1827892 ] Fix NPE crash when loading PBEM game (rrowell)</li>

  <li>- for installer with java, update embeded jre to 1.6 (sgb)</li>

  <li>- fix bug [ 1823400 ] Filename typo causes Exception to be thrown (sgb)</li>

  <li>- fix bug [ 1825576 ] Missing entry in four_if_by_sea.xml (sgb)</li>

  <li>- fix bug [ 1767304 ] Great War v.1.5 sz67 to sz57 bug (sgb)</li>

  <li>- fix bug [ 1563219 ] Possible to buy more units than can be placed  (sgb)</li>

  <li>- fix bug [ 1535135 ] loading save game bug (sgb)</li>

  <li>- fix bug [ 1718350 ] AA guns on LL fire once (sgb)</li>

  <li>- upgrade to looks 2.1.4 (sgb)</li>

  <li>- partial fix for bug [ 1750148 ] Transport error unloading to enemy territory from hostile water (sgb)</li>

  <li>- fix bug [ 1753871 ] SaveGameFileChooser bug (sgb)</li>

  <li>- fix bug [ 1692668 ] AI UK loads US troops on UK turn (sgb)</li>

  <li>- new Territory/Production summary options for Turn Summary (tclayton)</li>

  <li>- fix game xml files and PlayerList class to preserve proper player ordering (tclayton)</li>

  <li>- new Comment Log feature for adding comments/trash talk to game history (tclayton)</li>

  <li>- new PBEM Turn Summary posting feature (tclayton)</li>

  <li>- new "Edit Mode" feature (tclayton)</li>

  <li>- add PersistentDelegate support and IDelegateHistoryWriter interface to engine (tclayton)</li>

  <li>- new UnitAutoChooser feature (tclayton)</li>
  <li>-   create UnitAutoChooser class to translate chosen categories into possible unit solutions</li>
  <li>-   update MovePanel to use UnitAutoChooser for unit selection and route planning</li>
  <li>-   update UnitChooser to support UnitAutoChooser and solution browsing</li>
  <li>-   fix existing UnitChooser arrow icons and add left/right icons for solution browsing</li>

  <li>- MoveDelegate cleanup (tclayton)</li>
  <li>-   move all validation methods to MoveValidator so they can be called on client side</li>
  <li>-   make helper functions in MoveDelegate static, so they can be called on client side</li>
  <li>-   fix a few spelling mistakes in symbol names</li>

  <li>- partial fix for bug [ 1742775 ] Operating system freeze on Windows 98 with Ati Graphics Card (sgb)</li>

  <li>- Added support for "color" property, including color picker UI (dowobeha)</li>

</ul><h3>Changes for 0.9.1</h3><ul>

  <li>- implemented minimax AI and alpha-beta AI; currently used in Tic Tac Toe and King's Table (dowobeha)</li>

  <li>- implemented new King's Table game and Tic Tac Toe game (dowobeha)</li>

  <li>- created common code package to minimize code duplication between different games (dowobeha)</li>

  <li>- enhanced game framework to allow easier implementation of new grid-based games (dowobeha)</li>

  <li>- show time in chat panel, default is to show chat time in lobby, but not in game (gansito)</li>

  <li>- bug fixes (tclayton):</li>
  <li>-  [ 1204024 ] Missing Sea Zone </li>
  <li>-  [ 1510049 ] unloading troops bug</li>
  <li>-  [ 1640658 ] fighters in classic attacking on friendly carrier</li>
  <li>-  [ 1641051 ] Transport Unloading Bug</li>
  <li>-  [ 1652870 ] each phase should begin with focus on tabs panel</li>
  <li>-  [ 1655181 ] clean up history log entries</li>
  <li>-  [ 1659713 ] Java Exception</li>
  <li>-  [ 1661095 ] MovePanel should dynamically select best units for route</li>
  <li>-  [ 1662464 ] null pointer exception when skipping move phase</li>
  <li>-  [ 1662938 ] shadow units don't appear in map overlap sections</li>
  <li>-  [ 1671750 ] improve logic for transport load order</li>
  <li>-  [ 1672743 ] exceptions thrown by delegates get mangled by proxy</li>
  <li>-  [ 1696749 ] Unload problem from allied transport after undo</li>
  <li>-  [ 1753866 ] load and unload should have default selections</li>

  <li>- feature [ 1749993 ] new "History Log" feature (tclayton)</li>

  <li>- feature [ 1746894 ] Save Screenshot feature (tclayton)</li>

  <li>- feature [ 1673208 ] show move validation warnings/errors when moving mouse (tclayton)</li>

  <li>- feature [ 1661088 ] code cleanup - implement MovePanel getMovableMatch() method (tclayton)</li>

  <li>- new revised map (zero  pilot)</li>

  <li>- in revised, remove connection between 25 Sea Zone and 43 Sea Zone (zero pilot)</li>

  <li>- new vc image (zero pilot)</li>

  <li>- japanese tanks defend at 2 in pacific (comradekev)</li>

  <li>- non jopanese units defend at 1 in first round of pacific (comradekev)</li>

  <li>- fix empty sea zone in gulf of mexico in classic,battleship_row,four_if_by_sea,and iron_blitz (Scarbrow)</li>

  <li>- four if by sea turn order changed (Scarbrow, rodthegod)</li>

  <li>- add attack/defense/movement to production panel (gansito)</li>

  <li>- move test classes to test directory (sgb)</li>

  <li>- add export game setup charts menu (gansito)</li>

  <li>- show battle casualties in battle display (ahmet)</li>

  <li>- mark remote players as remote (ahmet)</li>

  <li>- allow multiple canals per sea zone (tekkyy)</li>

  <li>- allow centering map on battles (ahmet)</li>

  <li>- alt mouse scroll zooms the map in and out (ahmet)</li>

  <li>- new unit images (lssah)</li>

  <li>- add moderator functions, moderators can boot players, change passwords, and ban ip addresses (sgb)</li>

  <li>- better logic for determining attacker defender in odds calculator (Gansito)</li>

  <li>- add uninstaller (Gansito)</li>

  <li>- allow odds calculator to specify simulation count (Gansito)</li>

  <li>- banned ips and banned words are stored in lobby database (sgb)</li>

  <li>- the lobby server can now ban ip address (sgb)</li>

  <li>- add serialversionuid's to several classes (dagon)</li>

  <li>- add unit icon to unit images on the territory tab (dagon)</li>

  <li>- add menu to show/hide units (Gansito)</li>

  <li>- lobby game table doesn't loose selection when games are added/removed or updated (sgb)</li>

  <li>- better route finding logic (sgb)</li>

  <li>- added six nation free for all mod for revised map (the_devil_inside)</li>

  <li>- fix bug [ 1655283 ] Java 6 reserves java.awt.Window method getWindows() (sgb)</li>

  <li>- update to great war 1.3 (Jason Clark)</li>

  <li>- add canals to Great War and Big World (Black Elk)</li>

</ul><h3>Changes for 0.9.0.2</h3><ul>

  <li>- fix bug [ 1640596 ] 0.9.0.1 Revised Map Wrap Issue (sgb)</li>

  <li>- Fix bug where dissapearing networks players would not be removed from the game (sgb)</li>

  <li>- allow lobby server to ping clients to ensure the are still there (sgb)</li>

</ul><h3>Changes for 0.9.0.1</h3><ul>

  <li>- Adjusted British starting units (Jason Clark)</li>

  <li>- fixed infantry defense in Classic (sgb)</li>

</ul><h3>Changes for 0.9</h3><ul>

  <li>- improve great war map (Jason Clark)</li>

  <li>- improve great war african markers (Jason Clark)</li>

  <li>- fixed orientation of french zeppelin in great war (Jason Clark)</li>

  <li>- In great war, the US now has a starting transport, 1 inf and 1 cav.  1 us cruiser removed. (Jason Clark)</li>

  <li>- In great war, removed connection between Tanga and Weidmannshiel. (Jason Clark)</li>

  <li>- focus on action button when battle window is activated (sgb)</li>

  <li>- lobby server checks client's computer is network accessble when client hosts a game (sgb)</li>

  <li>- fix [ 1611289 ] map scrolling bug (sgb)</li>

  <li>- client only waits 10 seconds for connection to servr to be made before aborting (sgb)</li>

</ul><h3>Changes for 0.8.6</h3><ul>

  <li>- fix infantry in classic (sgb)</li>

  <li>- make convoy zones stand out better (sgb)</li>

  <li>- read output of exec'd lobby games (sgb)</li>

  <li>- Saved games in user.home/triplea (not .triplea) for linux and user.home/Documents/triplea for mac (sgb)</li>

  <li>- better logic for finding local ip address (sgb)</li>

  <li>- fix loby where clients could not find real server address (sgb)</li>

</ul><h3>Changes for 0.8.5</h3><ul>

  <li>- allow neutrals to have different unit types (sgb)</li>

  <li>- fix bugs where all bombers in lhtr defend at 2 (sgb)</li>

  <li>- update big world map (surtur2)</li>

  <li>- alt click/unclick selects 1/10 the type (Nate)</li>

  <li>- allow weak ai to move into empty nuetral territories (Nate)</li>

  <li>- make dialog clearer for planes can't land (sgb)</li>

  <li>- handle marti dice server error messages (sgb,clausewitz)</li>

  <li>- allow setting of lobby server lookup url in a file called lobby.properties with a key server in the root triplea directory (sgb)</li>

  <li>- fix max select when more than one type of unit present (sgb)</li>

  <li>- fix some click to continue to press sapce to continue (sgb)</li>

</ul><h3>Changes for 0.8.4</h3><ul>

  <li>- change click to continue text to press space to continue on battle screens (sgb)</li>

  <li>- add an option in battle calculator that at least 1 attacking land unit must survive (sgb)</li>

  <li>- fix transport capactity in europe, add connection between adriatic and central med, make saudia arabia nuetral (sgb)</li>

  <li>- change network to use nio (sgb)</li>

  <li>- fix bug where units originally in a sea zone with a submerged sub that is attacked by another unit cant leave the sea zone (sgb)</li>

  <li>- show battle calculator on current territory when pressing ctrl B (sgb)</li>

  <li>- ctrl+ and ctrl - zoom in and out (sgb)</li>

  <li>- mark lhtr as complete. low luck rules for heavy bombers still need to be added for all versions (sgb)</li>

  <li>- allow fighters to hover in sea zone where carriers can be produced under them for lhtr (sgb)</li>

  <li>- move dice server config into properties file (sgb)</li>

  <li>- allow controlling of name placements using name_place.txt (sgb)</li>

  <li>- fix sea zone boundaries when map is scaled (sgb)</li>

  <li>- add great_war mode (surtur2 and Triplelk)</li>

  <li>- update triplea_linux.sh (Daniel Roethlisberger)</li>

  <li>- show messages when people join/leave chat (sgb)</li>

  <li>- fix scroll bug where map would jump when mouse scrolled in non wrappable maps (sgb)</li>

  <li>- make convoy zones more transparent (sgb)</li>

  <li>- fix neutral fighting bug (sgb)</li>

  <li>- fix spelling mstakes in classic map (sgb, RogerCooper)</li>

  <li>- add max button to place dialog where number of units that can be placed is limited (sgb)</li>

  <li>- fix bug [ 1563239 ] Bad scroll increment for scrollbars (sgb)</li>

  <li>- fix bug  [ 1563227 ] Continue button does not show up (sgb)</li>

</ul><h3>Changes for 0.8.3</h3><ul>

  <li>- make odds calculator use MustFightBattle, update ui (sgb)</li>

  <li>- allow scaling of auto placement finder.  On the command line, type the scale after the command, </li>
eg "java -classpath triplea.jar util/image/AutoPlacementFinder 0.5" (sgb)

  <li>- add map decoration images.  create a file called decorations.txt in the map directory.  The format is the same as place.txt, with an image name, then list of points where</li>
the image should be drawn (multiple points are fine).  The image name should be the name of a file in the misc image folder (the same folder that has vc.png) (sgb)

  <li>- disable territory name drawing for territories listed in map.properties with a property like dont_draw_territory_names=Germany,Japan (sgb)</li>

  <li>- allow for map scaling (sgb)</li>

  <li>- let ai play in multiplayer games (sgb)</li>

  <li>- fix [ 1533252 ] problem clearing out pbem (sgb)</li>

  <li>- make the game look better on a mac (sgb)</li>

  <li>- better factory images (eleazar)</li>

  <li>- lhtr hb rules (not sure if low luck is correct) (sgb)</li>

  <li>- lobby server/client (sgb)</li>

  <li>- you can kick players out of a game on startup screen (sgb)</li>

  <li>- add odds calculator (zengland)</li>

  <li>- fix bug [ 1505192 ] air land in conquered territory (sgb)</li>

  <li>- allow networked games to be password protected (sgb)</li>

  <li>- for mac and linux, save games in home folder (sgb)</li>

  <li>- add convoy centers in europe map (iron cross)</li>

  <li>- put saved games in users home directory (sgb)</li>

  <li>- fix misspelt territory names in revised and lhtr (Jeffrey Henning)</li>

  <li>- add lhtr victory citries (sgb)</li>

  <li>- super subs defend at 3 in lhtr (sgb)</li>

  <li>- make lhtr aa guns not fire in non combat move (sgb)</li>

  <li>- pacific and europe map fixes (Opurt, FlyingSpaghettiMonster)</li>

</ul><h3>Changes for 0.8.2.1</h3><ul>

  <li>- fix installer with embedded java to actually use the embedded java (sgb)</li>

  <li>- default sound to off (sgb)</li>

  <li>- fix nz territory in four if by sea (rod the god)</li>

</ul><h3>Changes for 0.8.2</h3><ul>

  <li>- fix bug where observers joining mid game may ignore some updates (sgb)</li>

  <li>- lock game data before switching to history (sgb)</li>

  <li>- fix bug where casualty selection would sometimes appear before the battle panel (sgb)</li>

  <li>- fix bug where naval bombardment doesnt work for the first player to fight in round 0 (sgb)</li>

  <li>- change two if by sea to four if by sea (rod the god)</li>

  <li>- remove nuetral player in capture the flag (sgb)</li>

</ul><h3>Changes for 0.8.1</h3><ul>

  <li>- add capture the flag map (iron cross)</li>

  <li>- let ai place in places other than the capitol if not all units can be placed in the capitol (sgb)</li>

  <li>- fix move bug when no units are selected with pop up (sgb)</li>

  <li>- fix "Not enough units in starting territory" bug when hitting done (sgb)</li>

  <li>- documentation updates (sgb)</li>

  <li>- fix history update bug in multiplayer (sgb)</li>

  <li>- fix bug where if A has 1 carrier and no fighters in a sea zone and is allied to B with 1 carrier and 3 fighters in the saem sea zone, when A moves his carrier out of the sea zone, B's 1 fighter doesnt move with it (if A moved his carrier in the sea zone after B moved his carrier into the sea zone)</li>

  <li>- show strategic bombing raid casualty notification (sgb)</li>

  <li>- fixed bug where deselecting game-confirm enemy casualties would also stop confirming your own automatically selected casualties (sgb)</li>

  <li>- europe and pacific map fixes (zero pilot)</li>

</ul><h3>Changes for 0.8</h3><ul>

  <li>- save last used map skin and unit size (beagle)</li>

  <li>- add next and back buttons to history (sgb)</li>

  <li>- renamed game xml files (sgb)</li>

  <li>- moves canal info to the xml file (if you have a mod based on revised or classic, canals will be broken unless you add them in the xml, do a search for canal in classic.xml or revised.xml to see how it is done) (sgb)</li>

  <li>- fix bug where aa guns in retaken allied capitols werent reverting to there original owner (sgb)</li>

  <li>- replace random ai with weak ai (sgb)</li>

  <li>- fix pbem saved emails not always showing up on the start screen (sgb)</li>

  <li>- highlight units on mouse over when moving (sgb)</li>

Change for 0.7.5

  <li>- when changing to a skin that has relief images, always show the relief images (sgb)</li>

  <li>- add destroyer production to europe map (sgb)</li>

  <li>- fix map skins in zip files on windows (sgb)</li>

  <li>- map skins must use - not : to seperate skin from map names (eg revised-Coal, not revised:Coal).  Windows doesnt allow : in file names (sgb)</li>

  <li>- if user presses done when no moves were made, confirm that they do not want to move (sgb)</li>

  <li>- fix bug [ 1440134 ] rockets shouldnt move after firing (sgb)</li>

  <li>- add tripleawarclub dice server (clausewitz, pughead, sgb)</li>

</ul><h3>Changes for 0.7.4</h3><ul>

  <li>- remove autosave... from console output (sgb)</li>

  <li>- allow map skins to depend on each other (add a dependencies.txt file to the skin, with a single line dependencies=skin1,skin2,skin3)  skin1 is the name of the skin (eg pact_of_steel:coal, if pact_of_steel:coal is in a zip file, do not include the .zip)</li>

  <li>- better retreat dialog (sgb)</li>

  <li>- allow map to have PU images.  Images should be in the map folder, in a folder called PUs.  They should be named 1.png, 2.png...  if no png image is found for a given number, a string will be drawninstead. (sgb)</li>

  <li>- maps (and skins) can be zip files (sgb)</li>

  <li>- map skins can override unit,flag and vc images (sgb)</li>

  <li>- map skin directories must now be named original_map_name:Skin, rather than original_map_nameSkin as before (sgb)</li>

  <li>- move images and maps to top level folders (these are not on the classpath).  (sgb)</li>

  <li>- allow defining where to place PU markers using pu_place.txt.  The x,y location is such the point is the bottom left of the image. (sgb)</li>

  <li>- allow turn off drawing map names in map.properties using,  map.showTerritoryNames=false (sgb)</li>

  <li>- move chat panel to main window for networked games (sgb)</li>

  <li>- fixed bug where autosave game would add too many PUs at start up (sgb)</li>

  <li>- fix bug where attacking air units couldnt retreat if all attacking subs moved to attacking sea zone via submerged route (sgb)</li>

  <li>- allow clients to save a networked game (sgb)</li>

  <li>- game menu to show who is playing what player (sgb)</li>

  <li>- when a player (not an observer) leaves the game, the game is saved automatically, and the game ends (sgb)</li>

  <li>- observers can join and leave the game (server can optionally ban new observers) (sgb)</li>

  <li>- new startup screen (sgb)</li>

  <li>- add minimap (map by Clausewitz)</li>

  <li>- add delegate execution manager, block delegates from executing while save in progress (sgb)</li>

  <li>- make game data lock into a read/write lock, extend the game data lock to history (sgb)</li>

  <li>- add random ai (sgb)</li>

  <li>- if two players with the same name join the game, add a _1 to the second player (sgb)</li>

  <li>- remove ISaveableDelegate, all Delegates are saveable (sgb)</li>

</ul><h3>Changes for 0.7.2.4</h3><ul>

  <li>- move some code into swing event thread (sgb)</li>

  <li>- dont let players press dont place once player selection is done (sgb)</li>
 
  <li>- should read you need java >= 5.0, not java > 5.0 (sgb)</li>

</ul><h3>Changes for 0.7.2.3</h3><ul>

  <li>- make battle window a dialog (it will always be in front of the main window!) (sgb)</li>

  <li>- fix invalid roll count in multiplayer games when all bombers are hit by aa guns (sgb)</li>

  <li>- fix null pointer when placing units in sea zone with enemy units (classic game only) (sgb)</li>

  <li>- fix null pointer when when selecting null territories during movement (sgb)</li>

Change for 0.7.2.2

  <li>- fix convoys (adam_j)</li>

  <li>- fix bid purchase (sgb)</li>

  <li>- Iron blitz mod (ic)</li>

  <li>- fixed string index out of bounds when rolling pbem dice (sgb)</li>

</ul><h3>Changes for 0.7.2.1</h3><ul>

  <li>- fix stat panel in europe (sgb)</li>

  <li>- fix bug  1357768  0.7.2 dead defenders firing (sgb)</li>

Change for 0.7.2

  <li>- on PBEM screen, add id field (for challenge id) (sgb)</li>

  <li>- when clicking on a battle in history, center map on that territory (sgb)</li>

  <li>- allow unloading units from a battle zone into newly conquered territories (sgb)</li>

  <li>- allow saving games during battles (sgb)</li>

  <li>- shift click on a unit (or territory) to select all units in the territory (sgb)</li>

  <li>- rename attachment to attachment (sgb)</li>

  <li>- remove singleton image factories, move to UIContext (sgb)</li>

  <li>- when retreating from a sea zone, if a fighter has no movement, the fighter gets a 1 movement bonus (sgb)</li>

  <li>- battleships can only bombard if they are in a sea zone where transports unloaded (sgb)</li>

  <li>- fix bug [ 1277099 ] map refresh problems undoing move with captured aa gun (sgb)</li>

  <li>- Japanese victory points for a&a pacific (Adam_J)</li>

changes for 0.7.1

  <li>- updated readme and user docs (George_H)</li>

  <li>- if we have multiple transports that unloaded troops to an amphibious assault, then the transports </li>
  retreat from a  naval battle that precedes the amphibious assault, then too many units will retreat (sgb)

  <li>- various no pop up movement bugs (sgb)</li>

  <li>- fixed chinese tech in big world 1942 map (sgb)</li>

  <li>- partial fix for marines (marines still do not show up correctly in battle table) (sgb)</li>

  <li>- fixed missing connection from solomon in pacific map (sgb)</li>

  <li>- fixed bug [ 1259381 ] Bid purchasing (sgb)</li>

  <li>- fixed no pop up movement for scaled units (sgb)</li>

  <li>- removed territory attachments for sea zones in big world map (sgb)</li>

  <li>- Fixed missing connections in big world map, north to south brazil, and sea of Okhotsk to West Bering Sea (kc1189)</li>

  <li>- More email validation (Adam_J)</li>

  <li>- Chinese infantry mechanism added for a&a pacific (Adam_J)</li>

  <li>- Convoy Zones implemented (Adam_J)</li>

  <li>- Add code for marines (Adam_J)</li>

  <li>- Add code in for kamikaze (Adam_J)</li>

  <li>- fix bug located http://maddlinks.com/triplea/index.php?showtopic=707 (Adam Jette)</li>

</ul><h3>Changes for 0.7.0</h3><ul>

  <li>- add movement help to help menu (sgb)</li>

  <li>- remove hints menu (sgb)</li>

  <li>- movement now done without pop up dialogs  (sgb, lnxduk)</li>

  <li>- only allow transports to unload units to 1 territory  (sgb)</li>

  <li>- fixed bug [ 1238910 ] PBEM mode cannot accept subdomains  (sgb)</li>

  <li>- add "click" to select casualties button, many users are confused and dont know to click to select casualties  (sgb)</li>

  <li>- reduce network traffic somewhat by more efficient serialization  (sgb)</li>

  <li>- autosave now happens at the end of a turn, after combat move and before non combat  (sgb)</li>

  <li>- use annotations to determine when to autosave  (sgb)</li>

  <li>- change to jdk 1.5, 1.5 is now required to build and to run  (sgb)</li>

  <li>- fix bug where versions like 0.6.0.1 would be displayed as 0.6.1  (sgb)</li>

</ul>

<h3>Changes for 0.6.0.1</h3>

<ul>

  <li>- fix bug [ 1225276 ] Aircraft unable to attack or land (sgb)</li>

</ul><h3>Changes for 0.6.0</h3><ul>

  <li>- updated developer docs, incomplete for now (George_H)</li>

  <li>- draw a line under overflow units so you can tell what belongs in a territory (sgb)</li>

  <li>- fixed bug where you could retreat subs if all your opponents destroyers were destroyed in one round of combat (sgb)</li>

  <li>- fixed bug where damaged battleships would not repair while viewing history (sgb)</li>

  <li>- fixed small map refresh (whole map goes white) when switching skins (sgb)</li>

  <li>- fixed bug where sometimes dice would not show up on the select casualties panel (sgb)</li>

  <li>- removed "Heavy Bombers Pick best of X Dice" option from classic and wandering head big world, it didnt work (sgb)</li>

  <li>- Fixed bug where transport moves could be undone before moves where the transport had been loaded/unloaded (sgb)</li>

</ul><h3>Changes for 0.5.4</h3><ul>

  <li>- fixed bug where units could blitz through territories with an aa gun if they blitzed in 2 steps  (sgb)</li>

  <li>- fixed bug [ 1188411 ] Missing client text (Chat window) 5.2.2 (sgb)</li>

  <li>- fixed bug [ 1205387 ] Saving game during combat 0.5.3 (sgb)</li>

  <li>- fixed bug [ 1205775 ] 0.5.3 eMail Bug - hyphens not allowed in emails (sgb)</li>

  <li>- fixed bug [ 1205504 ] Units can land in amphibious assaults when transport is sunk (sgb)</li>

  <li>- fixed bug [ 1198828 ]Heavy Bomber Tech Broken 0.5.3 (sgb)</li>

</ul><h3>Changes for 0.5.3</h3><ul>

  <li>- added europe and pacific maps (incomplete versions) by iron cross (George_H)</li>

  <li>- added extra dice statistics such as, median, variance, and standard deviation (George_H)</li>

  <li>- fix bug [ 1023326 ] Fig Landing Problem, J1 (sgb)</li>

  <li>- more flexible validation for planes landing on carriers (sgb)</li>

  <li>- add stat export menu item Game->Export Game Stats (sgb)</li>

  <li>- upgraded plastic look and feel to version 1.3.1 (sgb)</li>

  <li>- add vc drawing and added vc cities to stats (sgb)</li>

  <li>- better email address ui and validation, allow up to 5 emails in to and copy (sgb)</li>

  <li>- added white factory images (zero_pilot)</li>

  <li>- added drawing capitol markers (capitol markers contributed by black elk) (sgb)</li>

  <li>- added junit.jar file to lib and removed it from .ant.properties (sgb)</li>

  <li>- fixed bug  [ 1070176 ] Mistakes in calculating Battlescore (change in TUV) (sgb)</li>

  <li>- fixed bug [ 1116632 ] v0.5.1.1 TripleA skipping battle in Borneo (sgb)</li>

  <li>- fixed bug [ 1145318 ] Another Error on 5.2.2 (sgb)</li>

  <li>- fixed bug [ 1157717 ] 0.5.2.2 Error with question : Sumerge subs (sgb)</li>

  <li>- fixed bug [ 1175467 ] game "stuck" when doing multiple battles with same units (sgb)</li>

  <li>- fixed bug [ 1171596 ] Rocket Tech bug v0.5.2.2, we now always ask what territory to attack with rockets, even if there is only one choice, this allows the user to decline a rocket attack (sgb)</li>

  <li>- during battles the dice are sorted according to unit type so that when you review the dice rolls, you can tell what unit rolled for which dice (sgb)</li>

  <li>- fix bug [ 1144356 ] alter email header on PBEM (this is really a feature request) (sgb)</li>

  <li>- added new chinese units and cruiser, halftrack, marine units (iron_cross)</li>

  <li>- fixed [ 1158469 ] Missing units in Purchase Menu when odd number of choices (sgb)</li>

  <li>- you can now specify victory cities in xml using a territory attachement (sgb)</li>

  <li>- added tile map drawing (sgb)</li>

  <li>- add a copy to clipboard button on the console (sgb)</li>

  <li>- if available, console will print stack traces when enumerating threads (sgb)</li>

  <li>- put neutral player color in map.properties (sgb)</li>

</ul><h3>Changes for 0.5.2.2</h3><ul>

  <li>- fixed Dont play button on client screen. (sgb)</li>

  <li>- threading fixes. (sgb)</li>

</ul><h3>Changes for 0.5.2</h3><ul>

  <li>- add switch in map.properties to disable scrolling map around the edges (sgb)</li>
 
  <li>- added scripted random for debugging (sgb)</li>

  <li>- added new map by WanderingHead (wandering head)</li>

  <li>- add confirmation prompt when exiting the game (sgb)</li>

  <li>- jdk 1.4 - 1.5 compatability (sgb)</li>

  <li>- Add has relief property to map.properties (sgb)</li>

  <li>- Add default unit scroll size to map.properties (sgb)</li>

  <li>- Changes to make TripleA compile under Sun JDK 1.5.x (George_H)</li>

  <li>- Added better unix shell scripts for TripleA, thanks DMan for the scripts (George_H)</li>

  <li>- Added better path search so TripleA can run from any directory (sgb)</li>

  <li>- Now all map utils have proper "save as" dialogs (George_H)</li>

  <li>- Added new class to prompt user to select a directory so map utils won't save files to a hardcoded dir (George_H)</li>

  <li>- Define player colour in map.properties to allow easy modification and adding new players (sgb)</li>

  <li>- Added option to limit PUs lost in a territory during one round. This is necessary to implement LHTR ruleset. (Ali Ibrahim)</li>

  <li>- Fixed bug in Irony PBEM random source: It did not use the max parameter passed to the random methods. This fixes the AA casualty selection problem in PBEM. (Ali Ibrahim)</li>

  <li>- Added new technology activation delegate to allow control of when technologies actually take effect. This is used to allow delay of technology activation in LHTR. (Ali Ibrahim)</li>

  <li>- Changed mouse behavior such that only the left button is used to select a territory to put units in. (Ali Ibrahim)</li>

  <li>- Added more options for unit size using submenu. (Ali Ibrahim)</li>

  <li>- Changed ordering of properties in the launcher properties tab to use ordering in game XML file. (Ali Ibrahim)</li>

  <li>- Added Map Skins code to allow multiple (1 and greater) map skins to be used for each game based on a directory search pattern. Skins must be in maps folder with game name as prefix (ie. revisedMySkin). (Beagle)</li>

  <li>- Changed how bombardment works. Now users pick where to bombard before any battles are resolved. This allows users not to bombard with a unit (for example if they wish to move it during non-combat) by picking "None". This also fixes the bug where a a unit could retreat from a battle and bombard in the same turn. It also allows user to divide their bombardment shots however they like when there are multiple bombardment targets. (Ali Ibrahim)</li>

  <li>- Fixed bug #1067768 concerning the border of seazone 27 and Belgian Congo. (George_H)</li>

  <li>- Fixed bug #1067331 by removing the connection between seazone 51 and 56 for Pact of Steel mod. (George_H)</li>

  <li>- Fixed bug #1067073 by removing the connection between seazone 15 and 16 for Pact of Steel mod. (George_H)</li>

  <li>- Fixed bug #1043826 concerning missing sea zone border & missing pixles on border. (George_H)</li>

  <li>- Added channel and remote messengers. (sgb)</li>

  <li>- Added game vault. (sgb)</li>

  <li>- Fixed bug [ 1053071 ] No non-combat movement (sgb)</li>

  <li>- Fixed bug where properties werent being updated on client (sgb)</li>

  <li>- Fixed bug [ 991810 ] Internet Bid Problem (sgb)</li>

  <li>- Fixed bug [ 1051937 ] Number of bid PUs displayed (sgb)</li>

  <li>- Fixed bug [ 1102812 ] flag image names not based on xml names (sgb)</li>

  <li>- Fixed bug [ 1102225 ] Error by adding better error messages (sgb)</li>

  <li>- Store pbem emails in saved game (sgb)</li>

  <li>- Fixed bug [ 1095206 ] AA Firing too quickly v0.5.1 (sgb)</li>

  <li>- Fixed bug [ 1092852 ] bug in 2bysea Version .5.1 (sgb)</li>

  <li>- Fixed bug [ 1021352 ] advanced tech prob (sgb)</li>

  <li>- Fixed bug [ 1021350 ] Tech Prompt (sgb)</li>

  <li>- Fixed bug [ 1006050 ] Unable to conquer territories (sgb)</li>

  <li>- Fixed bug [ 1021351 ] No Buy Confirmation (sgb)</li>

  <li>- Add micro to Version, ie version can now be xx.xx.xx.xx (sgb)</li>

</ul><h3>Changes for 0.5.1</h3><ul>

  <li>- Fixed bug where defending transported units were not correctly removed when their transports were killed. (Ali Ibrahim)</li>

  <li>- Fixed bug where transported AA guns fired in naval battles. (Ali Ibrahim)</li>

  <li>- Added a new developer document with map utils info. (George_H)</li>

  <li>- Added menu option to use small unit images on map. (Ali Ibrahim)</li>

  <li>- Large improvement and re-organizing of user documentation. (George_H)</li>

  <li>- Fully implemented Pact Of Steel mod (by Black Elk/Beagle). (George_H)</li>

  <li>- Improved map directory structures and code for triplea concerning TerritoryData class. (George_H)</li>

  <li>- Small iteration fix applied to PolygonGrabber to prevent crash. (Beagle)</li>

  <li>- Improve all map utilities so they are user friendly and better to use. (George_H)</li>

  <li>- Fixed bug where air units could define retreat paths (they still can in some games). (Ali Ibrahim)</li>

  <li>- Added MersenneTwister Thread Safe (MT199937) Random Number Generator with Permission from Sean Luke. (George_H)</li>

  <li>- Added Low Luck option following DAAK rules. However, the low luck rules were not implemented for sbr's and tech rolls. Also it is incompatible with the heavy bomber downgrade option. (Ali Ibrahim)</li>

  <li>- Allowed transports carrying aa guns to move in combat, although the aa guns still cannot be loaded/unloaded in the combat move. (Ali Ibrahim)</li>

  <li>- Fixed map bugs (missing connection between sz25, sz43, wrong connection between sz51, sz56, misspelling of Angola). (Ali Ibrahim)</li>

  <li>- Added logic to prefer routes without neutral countries. (Ali Ibrahim)</li>

  <li>- Fixed bug which did not allow placement of bid units. (Ali Ibrahim)</li>
 
  <li>- Fixed bug which did not allow placement of units in classic. (Ali Ibrahim)</li>

  <li>- Fixed bug which did not allow placement of AA guns correctly. (Ali Ibrahim)</li>

  <li>- Fixed bug which did not correctly reload transports which had conducted an amphibious assault and then retreated. (Ali Ibrahim)</li>

  <li>- Added capability to bid for allies. (Ali Ibrahim)</li>

</ul><h3>Changes for 0.5.0</h3><ul>

  <li>- Added TUV (total unit value) column in statistics panel. Added TUV lost in battle as part of battle end message. (Ali Ibrahim)</li>

  <li>- Fixed bug in statistics table when adding a player such as Italy (George_H).</li>

  <li>- Added logic to check production limits to display in production panel. (Kevin Sanders).</li>

  <li>- Added logic to not consider moving land units into water if there are no transports there. (Ali Ibrahim)</li>

  <li>- Added game defintion file, flags, color for Italian player. (George_H).</li>

  <li>- Fixed bug where allied air units which are cargo attacked. (Ali Ibrahim)</li>

  <li>- Changed game logic to allow destroyers to pass over submerged subs. (Ali Ibrahim)</li>

  <li>- Fixed bug which didn't allow fighters to consider landing in gibralator due to issue with pathing and neutrals. (Ali Ibrahim)</li>

  <li>- Added warning for users using Java 1.5 about some serialization problems which cause an incompatibility with saved games in Java 1.4. (George_H)</li>

</ul><h3>Changes for 0.4.9</h3><ul>

  <li>- Fix for bug #1010428 bypassing the unit selection popup message when there is only 1 unit to be moved. (Ali Ibrahim)</li>

  <li>- AI rules added,experimental. (Sean Bridges/Troy)</li>

  <li>- Stack trace when starting triplea after a saved game fixed. (Sean Bridges)</li>

  <li>- Fixed bug when defending subs get first strike fire, even if an enemy destroyer is present. (Sean Bridges)</li>

  <li>- Changes in Battle Panel relating to SWING event thread to stop game from freezing in battle mode. (sgb [Sean Bridges])</li>

  <li>- Fix for Bug #1001946 fixed for units crossing water. Now crossesWater only returns true if the route starts and ends on land and also contains a water territory. (James Damour)</li>

  <li>- Fixes for Points 1,4 (and possibly 3) for Bug #1003736. (Ali Ibrahim)</li>

  <li>- Clean up of neutrality violation messages. (Ali Ibrahim)</li>

  <li>- Now defending planes can land in any adjacent territory if their carrier is lost in combat. (Ali Ibrahim)</li>

</ul><h3>Changes for 0.4.8</h3><ul>

  <li>- Automatic casualty selection has been also added (Ali Ibrahim)</li>

  <li>- Drag scrolling and mouse wheel scrolling (since 0.4.7).  (lnxduk)</li>

  <li>- TripleA Chat improvements. (lnxduk)</li>

  <li>- Fix for null network interface on IRIX 6.5 OS. (George_H)</li>
  </ul>
</div>