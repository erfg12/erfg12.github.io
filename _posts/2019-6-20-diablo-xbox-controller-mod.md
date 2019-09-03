---
layout: post
title: Diablo 1 Xbox Controller & Keyboard Mod
tags: [Diablo, Xbox, PC]
categories: hacks
---

When I was trying to play Diablo 1 on my GPD Win I thought there has to be a way to incorporate controller support, similar to the Playstation 1 port. I remembered that there was an open source reverse engineered project for Diablo 1 called Devilution, so I figured that would be a good starting place for this project. After forking the repo, I started by getting familiar with the code base and creating new functions for how I would imagine this system working.

Things like detecting nearby items, monsters, towners, etc and being able to interact with them. Or, moving the cursor through the inventory and skills tree system and selecting what item or skill I need. So I created 4 new files. plrctrls.cpp/.h and joystick.cpp/.h and marking my code with //JAKE to make adding this modification for other Diablo 1 mods easy.

If you would like to grab the source code or add it to your own Diablo 1 mod, check it out at [https://github.com/erfg12/devilution](https://github.com/erfg12/devilution)

Here is the final product:

<video-js data-setup='{"fluid": true, "autoplay": false}' class="video-js vjs-default-skin vjs-big-play-centered" controls preload>
	<source
		src="https://newagesoldier.b-cdn.net/videos/diablo1_xbox_controller_mod/video.m3u8"
		type="application/x-mpegURL"
	/>
</video-js>

![](https://newagesoldier.com/devilution/img/diablo_keyboard.jpg)

![](https://newagesoldier.com/devilution/img/diablo_controller.jpg)

## New Keyboard Setup

- Spacebar - Attack nearby enemies, talk to towns people and merchants. Pickup & Drop items in inventory.
- Enter - Pickup gold, potions & equipment from ground, open chests and doors that are nearby.
- Arrow Keys and WASD Keys - Move character in that direction. Move cursor in inventory & speedbook.
- X Key - Cast spell or use skill. Back out of menus.
- Q Key - Use first health potion in belt.
- E Key - Use first mana potion in belt.
- Moved Speedbook key to H.

## New Functions

- Automap only moves when you hold down shift.
- Towns people, items and objects show information when nearby.
- Inventory snaps to grid system, use arrow/WASD keys to move around. Spacebar to pickup/drop items.
- Speedbook spells have snap grid system, use arrow/WASD keys to move around. Spacebar to select spell.
- Character info window level up attribute increase buttons now make cursor snap to them.
- Xbox One & 360 controller support added.

## Xbox Controller Button Layout

- **A Button:** Attack nearby enemies, talk to towns people and merchants, confirm menu clicks.
- **B Button:** Open inventory
- **X Button:** Pickup gold, potions & equipment from ground, open chests and doors that are nearby.
- **Y Button:** Cast spell or use skill. Back out of menus.
- **Back Button:** Open automap.
- **Start Button:** Open game menu.
- **Left Shoulder Button:** Open the speed spell book.
- **Right Shoulder Button:** Open character info window.
- **Direction Pad** & **Left Joystick:** Move character.
- **Right Joystick:** Move Cursor. Click for mouse left click.
- **Left Trigger:** Use first health potion in belt.
- **Right Trigger:** Use first mana potion in belt.
