---
layout: post
title: Make PC Game Cartridges
tags: 
categories: hacks
banner: pc-cartridge-banner.jpg
---

Gaming consoles like the Nintendo Switch and Sony Playstation Vita/TV are newer cartridge based media systems. There cartridges are pretty close in size to a normal SD card. I thought it would be fun to explore the possibilities of making our own game cartridges for the PC.

### Important Notes
Cheap MicroSD and SD cards typically have slow read/write speeds. So if you're plan on making one for older games, go ahead and use cheap ones. For more demanding games, use more expensive cards. Do not purchase unknown name cheap cards from Amazon or Ebay as they can be fakes.

```
Capacity	
SD: Up to 2 GB
SDHC: over 2 GB to 32 GB
SDXC: over 32 GB to 2 TB
SDUC: over 2 TB to 128 TB

Read mechanism	
Standard: 12.5 MB/s
High-speed: 25 MB/s
UHS-I: 50 MB/s or 104 MB/s
UHS-II: 156 MB/s full-duplex, or 312 MB/s half-duplex
UHS-III: 312 MB/s full-duplex, or 624 MB/s full-duplex
Express: ≥ 985 MB/s full-duplex
```

### Resources
- Windows PC with MicroSD or SD Card Reader
- [VMWare ThinApp](https://www.vmware.com/products/thinapp.html), [Cameyo Packager](https://online.cameyo.com/apps/1/download) or [DOSBox](https://www.dosbox.com/download.php?main=1).
- MicroSD card or SD Card for game storage media. Note the above speeds and sizes.
- [Autorun_Win10 app](https://github.com/erfg12/Autorun_win10) for making game media cartridges launch the executable or batch file upon insertion.

### Instructions
1. Download and run the Autorun_Win10 app on our Windows PC.
2. Format your storage media device (ex: Our SD Card) to be FAT32 or NTFS. Note that FAT32 has a restriction of file sizes over 4GB. I recommend NTFS.
3. You will use Cameyo Packager or VMWare ThinApp to create a packaged (containorized) version of your game. If it's an older DOS game, you can use scripts to auto launch DOSBox with your game in a .bat (batch) file.
4. Place your containorized game with any required files onto your storage media device, and create a new file in the root of the drive called `Autorun.inf`. This will make our game automatically launch when you insert the game into our Windows computer.

### Autorun.inf Structure
```
[autorun] 
open=Filename.exe 
icon=Filename.ico
```

### Gaming Boxes
You can make boxes for your cartridges to display on a shelf for safe storage. Here's a [full size DVD case with a MicroSD card holder](https://www.amazon.com/25PCS-14mm-Micro-Card-Clear/dp/B071KT56BL) or you can buy [Nintendo Switch replacement boxes](https://www.aliexpress.com/item/32921619896.html) and put [3D printed MicroSD card holders](https://www.thingiverse.com/thing:2838566) in them.