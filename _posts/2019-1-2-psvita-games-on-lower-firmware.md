---
layout: post
title: Play PSVita 3.61+ games on HENKaku
tags: [Sony, PSVita, Playstation]
categories: tutorials
banner: playstation-banner.jpg
---

If you have HENKaku on your PSVita and use something like PKGj to get your games, DLC, etc. you may see a (3.61+) in the content's title. This is because HENKaku can only be installed on PSVita or PSTV systems that are at 3.60 firmware version. You can technically update from 3.60 to 3.65 once you have HENKaku installed. But still newer games or updates will sometimes require 3.67 or 3.69 firmware versions.

Luckily there is a solution! If you update PKGj homebrew to the latest version, and install the plugin rePatch _(rePatch-reDux0)_, you can add a url_comppack variable to your config.txt file which lets you install a compatibility pack so you can play those games on your older firmware consoles!

**So let's go through the steps to set this system up:**

1. FTP to your console via VitaShell (press Select). Create the folder ux0:rePatch.
2. Install or update PKGj with the official [PKGJ.vpk](https://github.com/blastrock/pkgj/releases). Press X to install it in VitaShell.
3. Download this [config.txt](https://psvitamod.com/wp-content/uploads/2018/12/config.txt). Transfer it to your `ux0:rePatch` folder.
4. Download this [repatch.skprx](https://github.com/dots-tb/rePatch-reDux0/releases). Transfer it to your `ux0:tai` folder.

- If you do not have [NoNpDRM plugin](https://github.com/TheOfficialFloW/NoNpDrm/releases) installed, do so now and add it to your `ux0:tai/config.txt` file with step 5. I assume it is already installed.

5. Edit your `ux0:tai/config.txt` file _(press triangle > Edit)_, below the \*KERNEL section, type in `ux0:tai/repatch.skprx`, save and close. Restart your console.

Now open PKGj and select a 3.61+ game or DLC to install. You will see in red text that it is not compatible with your Vita. But now you should see a download compatibility pack option. After you select this, you will now get green status text. You can now install and use the content!
