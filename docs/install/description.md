---
title: "What is YAMS?"
date: 2023-01-10T15:23:19-03:00
draft: false
weight: 1
summary: Everything you need to know about YAMS and what makes it awesome
---

# Welcome to YAMS! 🎬

YAMS (Yet Another Media Server) is an **opinionated** media server that just works. No fuss, no complexity - just a smooth, automated media experience that you can set up in minutes!

## The Story Behind YAMS 📖

Back in 2019, I had a mission: Create a media server that my non-tech-savvy girlfriend could use without calling me for help every five minutes. So I dove in, combining some awesome open-source projects and wrapping them up in Docker containers.

Fast forward to today, and guess what? Mission accomplished! 🎉 Not only does my girlfriend use it without any issues, but I've even got my mom (who lives 5000km away!) streaming her favorite shows with zero problems.

When my friends saw how well it worked, they all wanted one too. But explaining how to set everything up was like trying to teach a cat to swim - technically possible, but way more complicated than it needed to be.

That's when it hit me: Why not create a script that could do all the heavy lifting? And that's how YAMS was born! Now anyone can build their own kickass media server without needing a PhD in computer science. 😎

## What Makes YAMS Special? ✨

YAMS isn't just another media server - it's your personal Netflix-killer with superpowers! Here's what you get out of the box:

### 🤖 Fully Automated
- **Smart Downloads:** Just tell it what shows and movies you want - YAMS handles the rest
- **Perfect Organization:** Everything gets sorted and labeled automatically
- **Subtitle Magic:** Auto-downloads subtitles in any language you want (if they're available)

### 📱 Watch Anywhere
- Works on pretty much anything that can run Emby/Jellyfin/Plex:
  - 🖥️ Web browsers
  - 📱 iOS & Android phones/tablets
  - 📺 Smart TVs
  - 🎮 Gaming consoles
  - And tons more!

## What's Under the Hood? 🛠️

YAMS combines some of the best open-source media tools out there:

### Core Components:
- 📥 qBittorrent & SABnzbd: Your download powerhouses
- 🎬 Radarr: Your personal movie hunter
- 📺 Sonarr: Your TV show tracker
- 🔍 Prowlarr: Your search master
- 💬 Bazarr: Your subtitle wizard
- 🎮 Jellyfin/Emby/Plex: Your streaming brain

### Performance Features:
- 🚄 **Port Forwarding**: Automatic port configuration for faster downloads
- 🔗 **Hardlinking**: Saves massive amounts of disk space by creating multiple references to the same file instead of duplicating data
- ⚡ **Atomic Moves**: Ensures clean, instantaneous file transfers without incomplete or corrupted files

Want to dive deep into file management best practices? Check out the [TRaSH Guides File and Folder Structure](https://trash-guides.info/File-and-Folder-Structure/) for the ultimate deep dive!

### Extra Goodies:
- 🔒 gluetun: Keeps your downloads private and secure
- 🎛️ Portainer: Makes managing everything a breeze
- 🎵 Lidarr: Handles your music collection

All these pieces work together seamlessly to create a media server that's both powerful AND easy to use. It's like having your own streaming service, but better - because YOU'RE in control!

Ready to dive in? Let's [get started with the installation](steps.md)!
