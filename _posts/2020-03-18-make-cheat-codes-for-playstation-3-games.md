---
layout: post
title: Make Cheat Codes for PlayStation 3 Games
tags: [Playstation, Sony]
categories: hacks
---

If you're looking to create your own cheat codes for PlayStation 3 games like God of War or Call of Duty games, here's an easy to follow guide to get started.

## Requirements

- PS3 with Custom Firmware in DEX mode (Ex: Rebug REX) or a PS3 Dev console.
- NetCheat : http://netcheat.gamehacking.org/ncUpdater/ncUpdateDir.zip
- ProDG : https://consolecrunch.org/threads/prodg-target-manager-download.4420/
- TrueAncestor SELF Resigner : https://www.sendspace.com/file/gpspjk

## Setup Steps

1. Install ProDG, place NetCheat and TrueAncestor folders on your desktop. Go into your ProDG folder and create shortcuts for Target and Debugger executables on your desktop.
2. Copy your game's EBOOT.BIN file. (Ex: GAMES/(game name)/usrdir/EBOOT.BIN or game/(game name)/usrdir/EBOOT.BIN if it's been patched) Place it into your TrueAncestor folder. Run TrueAncestor.exe and press option 1. You have a new EBOOT.ELF file.
3. Copy EBOOT.BIN and EBOOT.ELF into the TrueAncestor/tool directory. Open a command prompt and navigate to the TrueAncestor/tool directory. Type in `make_fself eboot.elf eboot.bin`. You now have a new EBOOT.BIN that has been decrypted! Replace your existing game's EBOOT.BIN with this new modified one.
4. Turn on your PS3 and hard wire your PS3 into your local network. Do not use a proxy and do not sign into PSN.
5. Start the game up. Open NetCheat and select TMAPI for your API in options. Click Connect and Attach buttons. Scan for your values here exactly as you would with Cheat Engine. If you're ready to debug and find functions, start ProDG Target, connect to your console's IP. Then start the ProDG Debugger exe and click on the gears icon to attach to the process. The game will freeze. Open the Target exe and click on the [-] icon on your console on the left panel to drop down a few options. Click on Kernel. You will see a green play arrow button, click on that to unfreeze the process.

You can now use the ProDG debugger to navigate to the memory addresses you find in NetCheat and create breakpoints to trace back to other functions. As well as replace bytes in the memory section of ProDG. Good Luck!
