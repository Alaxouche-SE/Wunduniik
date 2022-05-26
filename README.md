# Wunduniik

![Logo](https://i.redd.it/1tfaz3eeas191.png)

A Skyrim SE Heavy Modlist Installer.

## Summary
- [Preamble](#preamble)
- [System Requirement & Necessary Tools](#system-requirement-and-necessary-tools)
  - [Pc Minimum And Recommanded Components](#pc-minimum-and-recommanded-components)
  - [Necessary And Useful Applications](#necessary-and-useful-applications)
- [Installation](#installation)
  - [Pre-Installation](#pre-installation)
  - [Wabbajack Installation](#wabbajack-installation)
  - [Post-Installation](#post-installation)
    - [Load Order Sorting](#load-order-sorting)
    - [BethINI and INIs](#bethini-and-inis)
    - [ENB](enb)
- [Using The List](#using-the-list)
  - [Starting The List](#starting-the-list)
  - [Configuring MCM](#configuring-mcm)
- [Updating The List]
- [Removing The List]
- [FAQ](#faq)
  - [Fix a Crash](#fix-a-crash)
  - [Reporting an Issue](#reporting-an-issue)
  - [Wide and Ultrawide Screens Options]
  - [Performance Options]
    - [Tweaking/Swithing ENB]
    - [Ini Configuration]
    - [Mod Configuration]
- [Credits And Thanks]
- [Contact Me]

## Preamble

**This modlist is currently __ONLY__ for SE!!**

**This modlist is focused mostly on graphics and textures**

Wunduniik is a 1200+ modlist based on **my** personal preferences. It improves the base game to make it look more like a game from 2022 rather than from 2011. The name, "Wunduniik" is dovahzul for "Traveler" which I think perfectly describes this list. When you travel, you discover new cultures, architectures... things can look very different.

### Creation Ethos

*"I decided to create this modlist because people kept asking how I got Skyrim to look so good. I know that when you begin, it can be hard to mod correctly and you can quickly be lost, but following this guide will help you build the Skyrim of your dreams! This very extended and detailed modlist will help you understand modding \minimizing bugs and conflicts to allow for a completely immersive gameplay experience. This is how I think the game is perfect, but if you think something could be better, the choice is yours. For each graphic mod I use 2K resolution, but you should install a range between 1K and 4K (8K sometimes, if your PC can handle it). I don't recommend installing less than 1K resolution textures."*

## System Requirements and Necessary Tools

### Pc Minimum And Recommanded Components

As Wunduniik is a modlist modlist based on graphics, you must have a good GPU.

Minimum Specs:
- CPU: I5 10th Gen or 2nd Gen Ryzen
- RAM: 16GB DDR4
- GPU: a 8GB GPU such as a GTX 1080, RTX 2070...
- Storage: a 500GB SSD is the best, but a HDD will do the work
- Screen: 1080p Screen in 60Hz (keep in mind that having higher resolution will decrease performances so you must have a good pc)

In comparison here are my specs:
- CPU: I7-7700
- RAM: Corsair Vengeance 16GB DDR4
- GPU: GTX 1070 (Overcloaked)
- Storage: 500GB SSD
- Screen: FHD Screen in 60Hz

### Necessary And Useful Applications

For the modlist to work you must have some apps:
Please ensure you have .NET v5.0 or higher installed. Download the **desktop app installer and console app x64** from Microsoft here https://dotnet.microsoft.com/download/dotnet/5.0/runtime, and also [Visual C++ x64](https://aka.ms/vs/16/release/vc_redist.x64.exe).

To help you with the INIs configuration, I highly recommand to have installed [Notepad ++](https://notepab-plus-plus.biz)

## Installation

### Pre-Installation

Prior to installing Ruvaak, please complete the following steps.

1. Install [Visual C++ x64](https://aka.ms/vs/16/release/vc_redist.x64.exe) & [.Net Runtime v5 desktop x64](https://dotnet.microsoft.com/download/dotnet/5.0/runtime).
2. Change Skyrim so it does not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
3. Fully uninstall Skyrim by deleting the folder and the Skyrim Special edition folder inside /Documents/My Games/.
4. Reinstall Skyrim into a location that is not Program files. Somewhere like C:\Games is a good location.
5. Start the game once and let it do the graphics check. Do not worry about the settings as it will be replaced during installation.

The next steps are optional **but** useful if you want to edit the list so if you want to skip, you can:

- Download the following applications:
  - [SSEEdit](https://www.nexusmods.com/skyrimspecialedition/mods/164)
  - [LOOT](https://www.nexusmods.com/skyrimspecialedition/mods/1918)
  - [BethINI](https://www.nexusmods.com/skyrimspecialedition/mods/4875)
  - [Wrye Bash](https://www.nexusmods.com/skyrimspecialedition/mods/6837)
  - [DynDOLOD 3.0](https://www.nexusmods.com/skyrimspecialedition/mods/68518)
  - [ZEdit](https://github.com/z-edit/zedit/releases)
  - [SSELODGen](https://www.nexusmods.com/skyrimspecialedition/mods/6642/)
  - [Synthesis](https://github.com/Mutagen-Modding/Synthesis/releases)
- Install them on the Modding file we just created. Your Modding folder should look like this now:

![image](https://i.redd.it/x6vy7rvu8u191.png)

### Wabbajack Installation

### Post Installation

#### Load Order Sorting

If needed (or if you added new mods with plugins), it's highly recommanded that you sort your modlist. To do so, launch Mod Organizer 2, and add as executable `LOOT.exe`. Now run LOOT to the executable list. To help you, I already made some configurations for a correct Load Order. Here is the [LOOT Settings](https://drive.google.com/file/d/1-zJu53bN4NCCfUx9K3jNiD_4oXQYMCot/view?usp=sharing) I use. Extract its content in "Your Disk"\Users\"Your User Profile"\AppData\Local\LOOT\games\Skyrim Special Edition. 

Tip: to get access to Appdata if you can't see it, in your files explorer, go to options, Display, and tick "display hidden files and folders":

![image](https://i.redd.it/9gy3rgdmgu191.png)

#### BethINI and INIs

BethINI is a really useful tool to edit your `Skyrim.ini`, `SkyrimCustom.ini` and `SkyrimPrefs.ini`. I already provided you my INIs, but some lines might not be set up correctly for your computer. Here are the lines you must check before starting your game:
- SkyrimPrefs.ini:
  - [Display]
    - iSize H=1080 -> Change this with your screen resolution Height
    - iSize W=1920 -> Change this with your screen resolution Width
    
      Those 2 lines can be changed directly through the Skyrim Launcher or BethINI
  - [Launcher]
    - sD3DDevice="NVIDIA GeForce GTX 1070" -> Change this with you GPU name
- Skyrim.ini:
  - [Display]
    - sScreenShotBaseName=C:\Games\The Elder Scrolls - Skyrim - Special Edition\Screenshots\Screenshots -> Create a folder called `Screenshots` and replace this line         with the path leading to the new folder. Also you can change this using BethINI.


#### ENB

Wunduniik was designed and set up to be used with [Rudy ENB for Cathedral Weathers - Zangdar Edit](https://www.nexusmods.com/skyrimspecialedition/mods/39113) latest version, but you can change it if you don't like it.

Also to help you with the ENB management, I strongly advise you use [ENB Organizer](https://www.nexusmods.com/skyrim/mods/67077). It will allow you to prepare presets of ENBs you can easely switch between as it will remember the files used and their configurations. Here is how you may use/set up it:

## Using The List

### Starting The List

Open `Mod Organizer.exe` and launch `SKSE` through the executables. As the modlist is quite big, depending on your pc, it may take some time to load the game. **THIS IS NORMAL DON'T PANIC!** Also I advise you to add Modding folder and Skyrim folder as exeptions in your Antivirus, it may cause some issues and even crashes.

### Configuring MCM

MCM have been configured thanks to [MCM Recorder](https://www.nexusmods.com/skyrimspecialedition/mods/61719). However if you don't like my settings, you to change them, but with the amount of MCM, it may take some time. Here is my configuration for (almost) all MCM:

## FAQ

This section is for now empty, but will fill up with the question that will be asked. 

### Fix a Crash

If you are playing with my modlist (or any other) and for some reasons, the game crashes, don't panic. It can happen. The first thing we want to know is why doest it crash. To find out, normally once you will go back to Mod organizer 2, the `Overwrite` folder will contain a new folder called `.NetScriptFramework`. Expand it until you see a `Crash.txt` file. We will take an example:

![image](https://i.redd.it/tlssuy3elu191.png)

We can see on this crash log that in the `Possible Relevant Objects`, the plugins *etheral_elven_overhaul.esp* and *JK's Temple of Mara....esp* are mentioned a lot. This means they may be the cause of the crashes. So just disable the corresponding plugins and restart your game. If it doesn't crash again, we fixed it, however if it crashes again, follow again the steps. If after that you just can't fix your crashes, you can ask me or the modding helpers in my discord server.

### Reporting an Issue

If, during your playthrough, you encounter any bug, incompatibily, that may disturb your gameplay/immersion, I invite you to head over to my discord server and to share the bug you found in the dedicated channel, so I can try to fix it for a future update. We are working together to make this modlist always better!
