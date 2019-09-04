---
layout: post
title: How to Minimize Discord on Startup
tags:
categories: tutorials
---

Here's a batch file that will minimize Discord on startup. There is a small setup needed to do this though.

1. Start up Discord first, right click on the system tray icon and uncheck the "Run Discord when computer starts" option.
2. Unzip the DiscordMinimize.bat program and place it in your startup folder "%APPDATA%\Microsoft\Windows\Start Menu\Programs\Startup".

Now when you restart your computer Discord will open and do its update/spin animation then when it goes in to its full chat window it will minimize.

HOW IT WORKS: It will use the default Discord startup commands and the batch file will detect when Discord launches then give it 10 seconds and kill the program. Effectively making it minimize back to the system tray.

(https://newagesoldier.b-cdn.net/downloads/DiscordMinimize.zip)[Download the DiscordMinimizer here.]
