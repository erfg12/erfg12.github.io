---
layout: post
title: Getting Your Dreamcast Online, Without A Broadband Adapter!
tags: [Sega, Dreamcast]
categories: tutorials
---

Few people these days have dial up internet. Most everyone has ethernet cables with broadband, which leaves older technology behind. Even with the addition of the broadband adapter, you will not be able to play some games that require the dial up modem. Luckily there is a new developer out there to bring the Dreamcast back online with the use of a Raspberry Pi!

<div class='video'>
<a href='https://www.youtube.com/watch?v=KOo5Kay9fcU' title='Click here to watch the video!' target='_BLANK'><i class="svg-icon youtube"></i><div class="play"></div><img src="https://img.youtube.com/vi/KOo5Kay9fcU/0.jpg" /></a>
</div>

## Required Materials

- Raspberry Pi (used model A in example)
- RJ-11 Phone Data/Voice Wire
- 330 Ohm Resistor
- 330 ohm 1/4W 5% Carbon Film Resistor
- Heavy-Duty 9V Snap Connector
- 9v Battery
- Soldering Iron and Solder
- Wire Strippers
- Kazade’s SD Card Image
- Win32 Disk Imager
- RJ-45 ethernet cable for your Raspberry Pi
- Fax to USB modem adapter
- Disc Juggler
- Dreamcast Web Browser (US) (Europe)
- Blank CD-R’s for burning. You will need a CD burner as well.

## Setup Instructions

- Take your RJ-11 Voice/Data cable and cut it open about 4-5 inches and cut the inside red wire. Use your wire strippers to strip the ends of this red wire. Solder the 1UF capacitor to one end of the red wire and solder the red 9v snap connector on to that same end. Now on the other end of the RJ-11 red cable you will solder both the other end of the 1UF capacitor and the 330 ohm 1/4w resistor. On the other end of the resistor you will solder the black 9v snap connector cable. Once finished, it should look like this.
- Use Disc Juggler to burn your Planetweb or Dreamkey web browser CDI. Follow this video.
- Use WIN32 Disk Imager to write Kazade’s SD card image to your SD card for your Raspberry Pi. Plug in your Raspberry Pi’s RJ-45 ethernet cable and your fax to USB modem with your new RJ-11 cable. You can plug in the Raspberry Pi’s power to turn it on.
- Plug in your RJ-11 cable in to your Dreamcast, put in the Planetweb or Dreamkey burnt disc and turn it on. We will now be setting up the modem. Once you set up your modem, you are ready to play online! Follow Kazade’s thread on AssemblerGames.com to watch for upcoming updates.

## Modem Settings

- User Login: dream
- Password: dreamcast
- Dial Up Number: 555
- DNS1: 0.0.0.0
- DNS2: 0.0.0.0
- Modem Init: AT&F0
- Dial: Tone
- Dial Area Code: Off
- Blind Dial: On
- Proxy: No
