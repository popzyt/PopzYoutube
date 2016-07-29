
![Ajs/Ogar-Unlimited](http://ogarul.tk/ajs.gif)
### - The Next Generation Ogar
[![Build Status](https://travis-ci.org/AJS-development/Ogar-unlimited.svg?branch=master)](https://travis-ci.org/AJS-development/Ogar-unlimited) [![Join the chat at https://gitter.im/AJS-development/Ogar-unlimited](https://badges.gitter.im/AJS-development/Ogar-unlimited.svg)](https://gitter.im/AJS-development/Ogar-unlimited?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)  [![GitHub issues](https://img.shields.io/github/issues/AJS-development/Ogar-unlimited.svg)](https://github.com/AJS-development/Ogar-unlimited/issues)  [![GitHub forks](https://img.shields.io/github/forks/AJS-development/Ogar-unlimited.svg)](https://github.com/AJS-development/Ogar-unlimited/network)  [![GitHub stars](https://img.shields.io/github/stars/AJS-development/Ogar-unlimited.svg)](https://github.com/AJS-development/Ogar-unlimited/stargazers)  [![Plugin](https://img.shields.io/badge/Official%20Plugin%20Library-OgarUL--Plugin--Library-green.svg)](https://github.com/AJS-development/OgarUL-Plugin-Library)  [![MS](https://img.shields.io/badge/Client-AJS--dev-green.svg)](https://github.com/AJS-development/OgarUL-Client) [![Plugin](https://img.shields.io/badge/Forums-OgarUl-green.svg)](http://forum.ogarul.tk) [![Plugin](https://img.shields.io/badge/Stats-OgarUl-green.svg)](http://stats.ogarul.tk)  [![MS](https://img.shields.io/badge/Client-AJS--dev-green.svg)](http://play.ogarul.tk) 
[![Demo] (https://img.shields.io/badge/Demo-Heroku-green.svg)] (https://github.com/AJS-development/Ogar-unlimited/wiki/Demos)

A fully functional open source Agar.io server implementation, written in Node.js by the big ajs development team. Ogar Unlimited is designed to be used with the latest Agar.io client. It is basically what it says in the title, Ogar, except its functionality is unlimited!

**NOTE: FOR THOSE WHO CANT USE THE INSTALL DEPENDANCIES SCRIPT, YOU MUST DO NPM INSTALL AFTER YOU CD INTO THE SRC FOLDER**


### Highlight features in this modified copy
 1. PMSG command, to periodically send a message (no need for admin to be online to explain rules)
 2. OP , to do stuff in game WITHOUT a illegal clone client, see below
 3. MSG, FMSG commands
 4. Max IP Connections
 5. Troll command ;)
 6. More GameModes
 7. Ban, Unban, Ban List (with revolutionary ban technique, no lag, no DDoS attacks)
 8. Autoban option (see config.ini or advconfig.ini)
 9. More control (config.ini and advconfig.ini)
 10. and other features such as merge or nojoin or kick/killrange
 11. Better physics (ejected mass and split and virus)
 12. Colortext command (Changes console output color and style)
 13. Live Console (see gameserver.ini, where a live console appears) NOTE: this is way different that Ogarserv's Console
 14. Restart. Make it restart automatically or restart manually, Only works if use windows start script
 15. skins, to use custom skins, do <skinname> and then your name. for example `<spy> lol` will give you spy skin with name of lol use `[website]` to use a custom skin from a website (you need to use a url shortener though)
 16. customskins (see custom skins)
 17. Minions: you can create minions like agario powerups. press q to enter minion control mode (a b will appear next to your name). w = eject, space = split. press q again to exit
 18. Banlist file
 19. Opbyip
 20. Database free high score keeper
 21. pcmd command to do periodic commands
 22. range command for bulk commands
 23. easy verify system as anti bot mesure (config.ini or advconfig.ini)
 24. mousefilter as a anti bot measure
 25. plugins. Add gamemodes and commands easily! (See example plugin and template plugin)
 26. uniban. A pre-made banlist of already known bad ips
 27. garbage collection. prevent memory leak.
 28. chat
 29. Multi server support (see multiverse)
 30. Bots that team
 31. client configs
 
### Note:
Please note that this is updated very frequently and you should check for updates every week. I added an update system but It needs to be initialized by you (because I don't think it is the right thing to do, updating without your consent). Also you may copy this and modify it just please give some credit to the hard working dev team, that is all I care. Another note is that I am sometimes terrible in my grammar (I still cannot spell potato out loud). If there is an issue, please notify me. If there is something you want in this, just make a pull request.

### DO NOT BUY OGAR UL!
If you've purchased a copy of Ogar UL, you just got scammed. It is open source which means it is FREE. yes FREE! So if you paid any money, well, too bad.

### DO not get from other sources
If you got ogarUL from anywhere besides github, DELETE IT IMMEDIATLY!!! Those might be bundled with viruses and other things. Remember you are running this probably from `sudo`. Get the github one here: https://github.com/AJS-development/Ogar-unlimited


### How do I install plugins from the official library?
the official library is here: https://github.com/AJS-development/OgarUL-Plugin-Library


To install any plugins from the library, first do `plugin available` and remember the name of the plugin you want. then do `plugin install [name]` and you are set!

### How do I use other plugins?

To use a plugin, simply download the folder and drag it into the plugins folder in src or use the plugin add command. To use the plugin add command, the plugin must have a files.txt file. then click on that file, click raw, and then copy the url. Then do `plugin add [url] [pluginname]` and it will even reload automatically for you. Thats it! example, doing `plugin add https://raw.githubusercontent.com/AJS-development/OgarUL-Plugin-Library/master/devtools-plugin/files.txt devtools` will add a plugin called devtools to your plugins.

### How do I create a plugin? Is there Documentation?

This is the fun part, creating your own plugins. There is an example plugin you should look at and there is a template plugin. To get started, you can look at the plugin API documentation [here](https://github.com/AJS-development/Ogar-unlimited/wiki/Plugin-API-Tutorial).

### Multiverse
Multiverse is for having multiple servers in one console. This is how you use it. The command for multiverse is `multiverse [command] [arg]`. Available commands are `list`,`create`,`remove`, and `select`. The list is used by doing `multiverse list` and it will list servers and their ports. It will also tell you f that is the master or is selected. The create command creates a server. The args are `multiverse create [name] [port] [gamemode] [title]`. Make sure that the port is not repeated in other servers. The title arg is optional and spaces are allowed, it is what is displayed in the client. Note that only the master has a statsport and sends multiverse data. To remove a server, do `multiverse remove [name]`. To then control the server using console commands, you have to select it. Do `multiverse select [name]` to select a server and start controlling it.


### Easy Verify
For those of you who have trouble with minions and such, this feature is for you. Currently, there is no program that can get through all of ogar unlimited's filterrs anddd features, but in some future, someone might be able to crack the other anti bot mesures. So we created easy verify, a currently foolproof system that filters out bots. To turn on, turn verify to 1 in config. Then when a player spawns, he is frozen at a spot and is given a 3 digit code. Then that player presses w to kill himself and types in the code in the nickname box. Afteword, when pressing play again, it shows a success message. Press w again to play.

### Minions
You use minions by doing `minion [yourid] [amount] [minionname]`. Then, they will start following your mouse. You can control those minions by useing E and R keys. E for split. R for feed. If that doesnt work because of you client, turn useER to 0 in config.ini. then in game, q key. If you press it, a B will appear next to your name. then controls will be normal except now ejecting and splitting will happen on your minions not you. you can reenter normal control mode by pressing q again. You can disable minions by doing `minion [id]` in console for just you or do `minion destroy` and it will remove all minions.

### OP(2.4.5) - Guide,
You use OP by first setting who has op by doing op [id] in console. Then, that player can use the op features in game by pressing q. Then a c will appear next to your name. If you press w in this state, it gives you 100 more mass. If you press space in this state, you will be able to rejoin instantly. You will find out that if you press q again, two c's will appear next to your name. if you press w in this state, you shoot viruses. If you press space in this state, you shoot tiny things (almost invisible) that if someone eats, their mass is reduced by 100. Then, if you press q again,3 c's will appear.press w with 3c's, you shoot a virus, but whoever who eats it will be trolled :). If you press space with 3 c's the person who eats the virus will explode.If you  press q again, 4 cs will appear and if you press w, you will shoot a virus tha kills people and space, it shoots a kick virus. You can then exit op by pressing q again after doing an action or by pressing Q until the three c's will dissappear (so that you can normally split and shoot mass).

* Note: names (CC's) dont work when player name is blank and it doesnt work on Virus and Leap gamemodes

## Custom skins (guide)
You can use custom skins by putting them in customskins.txt
the format is `[shortcut] [skin]` for the skin field, to use a URL skin, you do `:http://url` DO NOT FORGET TO GET REID OF THE S IF IT IS HTTPS OR FORGET TO PUT A : BEFORE.To use an agario skin, use `%skinname`To use that skin in game simply do `<skinsshortuct>` and then your name,

You can see a more detailed guide on the [wiki] (https://github.com/AJS-development/Ogar-unlimited/wiki/Skins-and-skin-shortcuts)

## Obtaining and Using

As Ogar Unlimited is written in Node.js, you must have Node.js and its "ws", and "request" module installed to use it (unless you are using the Windows binary). You can usually download Node using your distribution's package manager (for *nix-like systems), or from [the Node website](http://nodejs.org). To install the "ws" and "request" module that is required, open up your system command line (cmd for windows, terminal for mac) and type "npm install ws" and do "npm install request". To see a detailed guide go to the [Installation guide] (https://github.com/AJS-development/Ogar-unlimited/wiki/Installation) in the wiki

(You can install and use Ogar unlimited on windows very quickly. First click `Installdependancies.bat` in src. Then wait (it takes a while), then click `Start.bat` and you're off! The next time you start the server, you only have to click `Start.bat`)

~~ (Binarys are also available in Releases)~~ OUTDATED

Currently, Ogar listens on the following addresses and ports:
* *:88 - for the stats server (I would use it to track servers)
* *:443 - for the game server

Please note that on some systems, you may have to run the process as root or otherwise elevate your privileges to allow the process to listen on the needed ports. **If you are getting an EADDRINUSE error, it means that the port required to run Ogar UL is being used. Usually, Skype is the culprit. To solve this, either close out skype, or change the serverPort value in settings/advconfig.ini to a different port. You will have to change your connection ip to "127.0.0.1:PORT"**

Once the game server is running, you can connect (locally) by typing `play.ogarul.tk/?ip=127.0.0.1:443` into your browser's address bar.

## Configuring Ogar UL
To control how your server is run, Edit files in `src/settings/`


## Custom Game modes
Ogar UL has support for custom game modes. To switch between game modes, change the value of "serverGamemode" in the configurations file to the selected game mode id and restart the server. The current supported game modes are:

Id   | Name                         | Additional Description
-----|------------------------------|-----------------------
0    | Free For All                 |
1    | Teams                        |
2    | Experimental (As of 6/13/15) |
3    | Timed FFA                    | Normal FFA but with time limit (see config.ini for time configuration)
4    | Virus Off                    | No virus in the map
5    | UnlimitPVP                   | Where you can split indefinitely and rejoin instantly - 1v1 game (created by me)
6    | UnlimitFFA                   | Same as above (Unlimited PVP) except in FFA (created by me)
7    | Shrinking FFA                | Shrinks the game(map size) as time passes
8    | Experimental v2              | An improved Experimental mode (created by )
10   | Tournament                   | Normal FFA, but with no respawn and time limit
11   | Hunger Games                 | Adapted from a movie called "Hunger Games"
12   | Zombie Mode                  |
13   | Team Z                       | Teaming in Zombie Mode
14   | Team X                       | Teaming in Experimental
15   | NoCollision Teams            | Same as Teams mode but with no collision between teammates
16   | NoCollision TeamZ            | Same as Team Z mode but with no collision between teammates
17   | NoCollision TeamX            | Same as Team X mode but with no collision between teammates
18   | Leap                         | Where you leap instead of split, made by Ogarplus
20   | Rainbow FFA                  | Hint: Use "Acid Mode" in the settings in the custom client
22   | BlackHole                    | Normal FFA but with one big black hole

## Console Commands
The current available console commands are listed here. Command names are not case sensitive, but player names are.
 
 - Help
   * Shows List Of Commands
 - Ophelp
   * Shows how to use OP
 - quickrestart
   * Quickly restart your server. This is not true restart and does not reduce memory;
 - multiverse [command] [arg]
   * manage multiple servers. see multiverse
 - Plugin [command]
   * manage plugins, reload, list, delete, add, available, install, update, search.
 - Chat [command] [args]
   * Chat from the console!. Commands: all, pm. For all `chat all [msg]` for pm `chat pm [id] [msg]`
 - Chatban [id]
   * Ban people from chatting!
 - Announce
   * Starts the high score announce feature
 - Verify [command] [id]
   * Verifies/reverifies a player .doing `verify reverify 1` forces 1 to verify again 
 - Minion [id] [amount] [minion names]
   * creates minions. to turn off, for a player do minion [id]. to destroy all minions do minion destroy
 - Update
   * gets current version of ogar unlimited and replaces the old with the new. Do update botnames to only update botnames or update skin to only update skins
 - Reset
   * Destroys everything and starts from scratch.
 - Range [start] [end] [command] [commandattr]
   * Does bulk commands. ex `range 1 10 freeze` would freeze players between 1 and 10
 - Pcmd [delay] [repeattime] [command] [commandat...]
   * Periodic commands
 - Opbyip [command] [ip]
   * Allows you to use the opbyip feature. the commands are add, remove, list, clear , record . This allows you to be automatically op based on your ip
 - Changelog [page]
   * Gets changelog from the servers
 - Explode [id]
   * explodes player
 - Blind [id]
   * Blinds/unblinds a player
 - Hide [id]
   * Hides/unhides a player
 - Split [ID] [Count]
   * Splits a player
 - Shrink [amount]
   * Shrinks the game (amount is optional)
 - Enlarge [amount]
   * Enlarges the game (amount is optional)
 - Freeze [id]
   * Freezes a player
 - Spawnmass [id] [mass]
   * sets a players spawnmass. set to 0 to return to normal value
 - Speed [id] [mass]
   * sets a players base speed. set to 0 to return to normal value
 - Colortext [color]
   * Changes console Color and Style (blue, green,red,yellow,bold,reset,dim,white, help)
 - Team [id] [team (r,g,b)]
   * Changes a players Team (you might have to split to see the changes though)
 - Resetvirus
   * Turns special viruses (from OP's) into normal ones
 - whitelist [IP]
   * whitelists an IP
 - Unwhitelist [IP]
   * Unwhitelists an IP
 - whitelist
   * Lists whitelist
 - Clearban
   * Clears ban list
 - Ban [IP]
   * Bans an IP and sends a MSG. Do ban record to record ban
 - Unban [IP]
   * Unbans an IP
 - Rainbow [id]
   * gives player rainbow effect
 - Kickbots [number]
   * Kicks a number of bots (leave field blank and it will kick all bots)
 - Killbots [number]
   * Kills a number of bots (leave field blank and it will kick all bots)
 - Restart [minutes]
   * Restarts the server after a number of minutes or if you leave min blank, restarts immediatly
 - Banlist
   * Lists banned IPs
 - Clearban
   * Clears ban list
 - Op [ID]
   * Makes player OP
 - Dop [ID]
   * De-OPs a player
 - Rop
   * Resets op
 - Pfmsg [delay] [duration] [x to repeat] [msg1] [msg2] [etc...]
   * Periodically sends a force message (seconds)
 - Spfmsg []
   * stops pfmsg
 - Pmsg [delay] [duration] [x to repeat] [msg1] [msg2] [etc...]
   * Periodically sends a message (seconds)
 - Spmsg []
   * stops pmsg
 - Troll [id]
   * You figure out this one, Its a suprise!
 - Fmsg [message 1] [message 2] [etc...]
   * Forces players to read a message, This is done by changeing leaderboard to msg, freezing players, and change their name temporarily
 - Msg [message1] [message2] [etc...]
   * Changes the leaderboard to a message for a short time
 - kick/killrange/ban [Start] [End]
   * Kicks/kills/bans in a range (eg: killrange 1 10 will kill players whos ids are between them)
 - Nojoin [id]
   * Makes person unable to join
 - Merge [id]
   * forces user to merge
 - Addbot [Number]
   * Adds [Number] of bots to the server. If an amount is not specified, 1 bot will be added.
 - Board [String 1] [String 2] [String 3] ...
   * Replaces the text on the leaderboard with the string text.
 - Boardreset
   * Resets the leaderboard to display the proper data for the current gamemode
 - Change [Config setting] [Value]
   * Changes a config setting to a value. Ex. "change serverMaxConnections 32" will change the variable serverMaxConnections to 32. Note that some config values (Like serverGamemode) are parsed before the server starts so changing them mid game will have no effect.
 - Clear
   * Clears the console output
 - Color [Player ID] [Red] [Green] [Blue]
   * Replaces the color of the specified player with this color.
 - Exit
   * Closes the server.
 - Food [X position] [Y position] [Mass]
   * Spawns a food cell at those coordinates. If a mass value is not specified, then the server will default to "foodStartMass" in the config.
 - Gamemode [Id]
   * Changes the gamemode of the server. Warning - This can cause problems.
 - Kick [Player ID]
   * Kicks the specified player or bot from the server.
 - Kill [Player ID]
   * Kills all cells belonging to the specified player.
 - Killall
   * Kills all player cells on the map.
 - Mass [Player ID] [Number]
   * Sets the mass of all cells belonging to the specified player to [Number].
 - Name [Player ID] [New Name]
   * Changes the name of the player with the specified id with [New Name].
 - Playerlist
   * Shows a list of connected players, their IP, player ID, the amount of cells they have, total mass, and their position.
 - Pause
   * Pauses/Unpauses the game.
 - Reload
   * Reloads the config file used by the server. However, the following values are not affected: serverPort, serverGamemode, serverBots, serverStatsPort, serverStatsUpdate.
 - Status
   * Shows the amount of players currently connected, time elapsed, memory usage (memory used/memory allocated), and the current gamemode.
 - Tp [Player ID] [X position] [Y position]
   * Teleports the specified player to the specified coordinates.
 - Virus [X position] [Y position] [Mass]
   * Spawns a virus cell at those coordinates. If a mass value is not specified, then the server will default to "virusStartMass" in the config.

## Contributing
Just make a pull request or make your own copy

## Things that I dont want you to copy (copying it to your own file or fork)
1. No-Lag antibot measures
2. OP
3. minions
4. smart bot/despawn
5. easy verify
6. Periodic things (pmsg, pcmd, etc..)
7. mousefilter
8. plugins
9. Adv Multiverse system
10. client config system

#####anything else, if you improved it, you dont have to give us credit, or else if you just copied, you must give us credit
