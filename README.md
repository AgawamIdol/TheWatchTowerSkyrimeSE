# The WatchTower Skyrim SE
![TheWatchTower](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/blob/main/images/invite_banner.png)

**Before getting started, download the .zip folder above and unzip it. These folders will be referenced during the installation process.** 
![Zip](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/blob/main/images/zip.png)

# Directory 
* [Installation](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/edit/main/README.md#installation) 
  * [Steam](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/edit/main/README.md#steam)  
    * [Disable Steam Overlay](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/edit/main/README.md#disable-steam-overlay) 
    * [Skyrim Updates](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/edit/main/README.md#skyrim-updates)
    * [Downgrade Steam](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/edit/main/README.md#downgrade-skyrim)
   * [Wabbajack](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/blob/main/README.md#wabbajack)
   * [Post Installation](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/edit/main/README.md#post-installtion)
     * [Installing Mods](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/edit/main/README.md#installing-mods) 
     * [Changing Game Files](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/edit/main/README.md#changing-game-files)

# Installation

## Steam
Install Skyrim SE from steam. It is ok if it is the latest version because we are going to downgrade it later. Make sure to open skyrim completely then quit. If you are using a non legitimate version, you are going to need to put the installation in your steam directory. Otherwise, wabbajack will not know where skyrim is installed. 

### Disable Steam Overlay
Steam overlay causes issues with ENB and it is recommended to be turned off. 
* Right click your game in your steam library
* Go to Properties
* Uncheck "Enable the Steam Overlay while in-game"

### Skyrim Updates
Bethesda is still updating this game. When it does it will break all your mods. You want to make sure that steam does not automatically update the game for you. 
* Right Click your game in your steam library
* Go to Properties
* Go to the updates Tab
* Change the drop down to "Only update this game when I launch it"

### Downgrade Skyrim
We are going to need to downgrade Skyrim from AE(Annivarsy edition) to SE(Special Edition). We are using Skyrim version 1.5.97. Download the **FullPatcher.exe** from [here](https://www.nexusmods.com/skyrimspecialedition/mods/57618?tab=files). If you run into any issues with the patcher, please make sure your game is fully up to date on Steam. 

## Wabbajack

Grab the latest version of Wabbajack.exe from [here](https://github.com/wabbajack-tools/wabbajack/releases). Put the Wabbajack.exe in it's own folder. Then, double-click the Wabbajack.exe to start the launcher. 

Once the launcher has opened, click "Install From Disk" and point it to "TheWatchTower.wabbajack" file that you downloaded that was included in the zip. **Installation Location** should NOT be in your skyrim directory. This is where all of the installed mods will go. Make sure you choose a place or create a folder that you can find later. **Download Location**, same thing. This is where all the mods will be downloaded before being installed. 

Wabbajack will ask you to log into Nexus. This is where most of the mods come from. The downloads will be automatic if you have a premium account. If not, you will have to hit the download buttons for each mod. There are about 600+. 😊

## Post Installtion
Before you can dive into the game, there are some files that need to be moved around. We are mainly bringing in .dll files and changing some settings to make sure the game runs smoothly. 

### Installing Mods

Go to the installtion folder and launch **ModOrganizer.exe**. Click yes to any pop ups that appear. First, we need to install a patch that is missing. Download it from [here](https://www.nexusmods.com/Core/Libs/Common/Widgets/DownloadPopUp?id=209150&game_id=1704). You need to add this mod to ModOrganizer and enable it. 

* Click the button in the upper left hand corner to add a mod. 
* Select the mod you just downloaded. 
* Double-click the mod on the right hand side to install it. (If it is already installed, ignore this step)
* Check the box next to it in the list to enable it. 

![Download](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/blob/main/images/Download.png)
![Enable](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/blob/main/images/Enable.png)

We also need a patch for particles. Download and install it using the above steps. [Skyrim Particle Patch](https://mega.nz/file/vpNFFawJ#aqjydQJ_08uRRzXRdK8cJwg55RwXXK2hV_uT7xagzNM)

### Changing Game Files
We need to now add some games files, as well as edit one file in our directory. 

In ModOrganizer, change the drop down from **SKSE** to **Explore Virtual Folder**. Then click Run. 
![Virtual](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/blob/main/images/Virtual.png)

This will open you directly to the Skyrim data folder. We need to go back a directory. On the left hand side, click **Skyrim Special Edition**. It is right above the highlighted folder. 
![Direct](https://github.com/AgawamIdol/TheWatchTowerSkyrimeSE/blob/main/images/Direct.png)

Drag and drop all of the **Game Folder Files** into this directory. Then click into the **Skyrim** folder. In here there is only one file. The SkyrimPrefs.ini file. There are some settings in here we need to change to get visuals to work properly. Double click it to open it. In here you want to:
* set bEnableImprovedSnow= value to 0.
* set bDrawLandShadows= 1
* set bTreesReceiveShadows= 1
* make sure fGamma= value is set to 1.0000

Now **save** this file and close out back to ModOrganizer. **DO NOT FORGET TO SAVE!!**

Change your drop down back to **SKSE**. Then click Run. Your game should now be good to play!
