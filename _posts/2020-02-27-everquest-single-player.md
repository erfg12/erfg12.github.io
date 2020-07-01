---
layout: post
title: EverQuest Single Player
tags: [everquest]
categories: tutorials
banner: everquest-banner.jpg
---

Ever since I was young I wanted to play a single player version of EverQuest. Well today, I did just that, and I'm going to show you how you can too!

<iframe style="width:250px; height:250px;" src="https://www.youtube.com/embed/Uj_jZQqjRHE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Benefits
* Remove corpse retrieving
* Remove experience loss upon death
* Remove unmemorize spells upon death
* Higher HP/MANA/STA regen
* Soul bind anywhere
* Reduce NPC running away at low HP
* Higher hit chance
* Remove NPC bonuses
* Reduce stun chance
* Other minor adjustments

### Steps

1. [Install EQEmu](https://eqemu.gitbook.io/server/categories/installation/server-installation-windows)  - This is our EverQuest server.
2. Open eqemu_server.pl file, type in `setup_loginserver`, then type in `setup_bots`, then type in `database`, then type in `check_bot_db_updates`. Bots and local login server are now setup.
3. Install [MySQL WorkBench](https://dev.mysql.com/downloads/workbench/). First, click Edit > Preferences... > SQL Editor > (scroll down) Uncheck Safe Updates. Restart MySQL WorkBench. Double click on the first entry. Username is root, password is eqemu (lowercase). Click on the Schemas tab. Right click on PEQ > Set as Default Schema. [Here is the SQL Statements you would want to run](https://gist.github.com/erfg12/75e3dc772a0c9a5e432aec013e748cdb). Click the yellow lightning bolt above to run the update statements.
4. Download and install [EverQuest RoF2 client](https://archive.org/details/everquest_rof2). Open your EverQuest game folder, make a shortcut of EQGame.exe onto your desktop. Right click on EQGame.exe > Properties > add `patchme` to the end of your Target.
5. Open your EQEmu folder, run `t_start_server_with_login_server.bat`. This will launch several windows. Keep these open, as this is your game server. Hopefully there is no red text in any of these windows. If you have any issues, please consult the EQEmu project website or their Discord channel.
6. Run the EQGame.exe shortcut you made on your desktop. Type in an account username and password you want to use, this will automatically create the account in the database. Create your character and jump into the game!

Consult the [bot commands list](https://eqemu.gitbook.io/server/categories/bots/bot-commands) in the EQEmu wiki if you want to use bots. But, with the DB updates we made, you should be able to solo play EverQuest!