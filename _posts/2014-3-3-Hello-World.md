---
layout: post
title: Make Your Own Amiibo
banner: https://d258qip9dwvby3.cloudfront.net/amiibo-banner.jpg
categories: tutorials
---

Amiibo figures are nothing more than NFC (Near Field Communication) chips and plastic. You can purchase NFC tags for very cheap. However, the Amiibo NFC chips are transmitting some encrypted code. But several developers have found ways to decrypt and use this data. They have uploaded their source code to GitHub. Lots of Android devices out there have the ability to read/write to NFC tags. So if we have an NTAG215 NFC tag and write the Amiibo data to it, we can claim it as our own on the console. Let’s get started!

[![Play Video](https://img.youtube.com/vi/0a0FJKGbYcU/0.jpg)](https://youtu.be/0a0FJKGbYcU)

## REQUIREMENTS
The Android app, unfixed-info.bin and locked-secret.bin files (DOWNLOAD BELOW)

Android device that has NFC capabilities (ex: Nexus 7)

NTAG215 NFC tags (NOT NTAG 203, 210, 212, 213 or 216)

## INSTRUCTIONS
On your Android device go to Settings > Security > Unknown Sources (turn on).

Install the TagMo.apk file on your Android device.

Place unfixed-info.bin, locked-secret.bin and Amiibo dump files on your Android device.

Launch TagMo app, touch the 3 dots in the upper right corner > Load key(s) file > and select the unfixed-info.bin and locked-secret.bin files.

Touch the LOAD TAG button and select your Amiibo .bin dump file.

Touch the WRITE TAG (AUTO) button and press your NTAG215 NFC tag to the back center of your device. Keep it pressed against your device until you see the message “DONE”.

**NOTE:** _The data writing should take less than 3 seconds._

You can now use these NFC stickers on anything! I personally stuck them on to print outs of the Amiibo”s and put them on a homemade key chain. You could also make your own Amiibo figures out of clay or plastic and stick them to the bottom and they would work exactly the same.

## FAQ
**Q)** I’m using a Samsung Galaxy device and the app crashes when trying to write to it.

**A)** Try this modified TagMo app.

**Q)** I’m using a Nexus 7 device and using version 2.3.4 TagMo app, but it keeps crashing.

**A)** I had the same issue. Version 2.3.1 works perfectly for Nexus devices.

**Q)** Can I get 20 heart link, majoras mask link, and skyward sword link?

**A)** Here: 20 Heart Wolf Link, Majora’s Mask Link, Skyward Sword Link.

**Q)** The app crashes and I have tried all versions of Tagmo.

**A)** If you downloaded your dumps from NFC-bank, try downloading to your PC, then transferring it to your phone via USB cable.

**Q)** Does this work for LoZ:BoTW?

**A)** Yes.

**Q)** Does this work for the Wii U, Switch and 3DS devices?

**A)** Yes.

**Q)** Do I need a jailbroken or hacked Android device to run Tagmo?

**A)** No.

**Q)** Can I re-write NTAG215s?

**A)** In my personal experience with them, no.

**Q)** If I play Super Smash Bros. with my NTAG215s, does it save the data to it?

**A)** Yes. It acts like a normal Amiibo figure.

**Q)** Can I use NTAG 203, 210, 212, 213 or 216?

**A)** No, because they are all different sizes and the consoles won”t recognize them as Amiibo.

**Q)** Can I use an iOS device? iPad, iTouch, iPod, iPhone, AppleWatch?

**A)** No. Some of these devices can send NFC signals but it is Apple”s locked down hardware.

**Q)** Can I just use my phone instead of an NTAG215 tag?

**A)** No. I recommend using Google and researching this further if you have questions about it.

**Q)** Do I have to use a specific file manager app like Root Browser?

**A)** No, you can use any file manager app you want.

**Q)** I bought some blank tags and when I scan them, it says “Mario (SSB)”.

**A)** SOME versions of Tagmo have “Mario (SSB)” is index 0. Others will say random digits. So yes, they are blank.

**Q)** Where is the printed template shown in the video?

**A)** Download [this zip](https://storage.googleapis.com/newagesoldier_dot_com/Amiibo%20Print%20Templates.zip). Read the README.txt file in it.

Don’t have an Android device with NFC capabilities? Here are some cheap ones on eBay.
– If you buy these with bad IMEIs or cracked screens you can get them cheaper.

– HTC EVO 4G LTE 16GB – $40 or less
– LG Escape 2 H443 8GB (not unlocked) – $40 or less
– LG Lucid 3 VS876 8GB – $40 or less

[Tagmo app download.](https://github.com/HiddenRambler/TagMo/releases)

[Bin files Download.](https://storage.googleapis.com/newagesoldier_dot_com/Amiibo%20Hacking.zip)

[Amiibo Dumps](https://nfc-bank.com/bins.php?categoryid=2)
