---
layout: post
title: Netflix Site
tags:
categories: hacks
---

This is a PHP web program you can use to make your own Netflix look-a-like website. It runs completely on PHP, no database setup required. All information and photos are pulled from IMDb.

I recommend setting this up on your home computer as most web hosting websites will not be ok with you uploading videos on to their servers. You can host this on your computer at home with WAMP, IIS with PHP or on Linux with Apache and PHP.

Upload the movies folder to your website directory (with WAMP it’s usually “C:\wamp\www”), then upload the your movies/videos into the videos folder. If it’s a TV show, folder with the seasons labeled.

Example TV shows:
/videos/breaking bad/season 1/episode_name.avi
/videos/breaking bad/season 2/episode_name.avi

Example Movies:
/videos/movie_name.avi
/videos/another_movie_name.avi

Any date/year issues with the data being pulled should have the year placed in the file name.

Example Fixing Year Issues:
Day The Earth Stood Still 1951.wmv
Day The Earth Stood Still 2008.wmv

Names of files are automatically parsed. For example, if a movie file has the name “The.Darjeeling.Limited(2007).avi”, the program will parse the file to read “The Darjeeling Limited” and search IMDb for it and pull the data. So, you can leave files with un-cleaned names and you don’t have to worry.

Also, to stream movies you will need VideoLAN version 2.0 and above with the web streaming plugin, as this supports most video types. For some reason, this works best with Firefox. IE may block this plugin…

If you upload a TON of movies TV-shows etc into videos and go to the website for the first time, it may take a bit to load as it needs to cache the information for faster viewing in the future.

# HOW TO SETUP / INSTALL

Requires Apache for Linux server, or IIS for Windows server and PHP module. For easy setup on Windows, you can use WAMP.

The administration section’s password is located in the includes/settings.ini.php file. Open the file with notepad and change the password.

============ REQUIRED PERMISSIONS CHANGES ==============
chmod 777 -or- “permissions to Everyone” –> /pics (folder)
chmod 777 -or- “permissions to Everyone” –> /data (folder)
==========================================================

Download this project from (https://github.com/erfg12/netflix-look-a-like)[the Github repo.]
