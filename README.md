# All of your games on Linux

# Process to play on Linux
## Tested with:
* Linux Mint 20.3, 21 and 21.1 (should work on ubuntu 20.04 and 22.04)
* CPU : AMD ryzen 5 5600X
* GPU : AMD radeon 6600XT
#
## Wine :
### run the following commands to install good packages and extensions of wine: 
```
sudo apt update 
apt full upgrade
apt install -y wine winetricks
```
#
## Steam :
### download steam for linux;
### Once it's done and you're connected, on Steam, go to:
* Steam ;
* Settings ;
* Steam play ;
* Check "Enable Steam Play for all other titles" checkbox ;
* Select a Proton version in the "Run other titles with:" selection window (the more recent before the experimental one should be good).
##
### If no downloads are running, you can try to install a non compatible linux game, and then the selected version of proton should be installed.
##
### Some of games, even with basic proton, could still not working. To be sure to run all of your games, check [this link](https://github.com/GloriousEggroll/proton-ge-custom/releases) to get proton GE on github.
### There's custom proton versions that you can download, these are really recommanded to launch launcher from steam like epic games, battlenet, etc...
### Once you've download a version of proton GE (the most recent should be enough), go to :
>/home/.steam/steam/compatibilitytools.d/
### and extract it in this folder. If the folder *compatibilitytools.d* doesn't exit, create it.
### Once it's extract, restart steam.
#
## Other launchers:
### Download your launcher .exe or .msi like you used to on Windows.
**The fowlloing process have to be done one launcher by one.**
### Go on steam :
* Games (not library) ;
* Add a non steam game to my library ;
* Select BROWSE... ;
* Go in the folder with the launchers ;
* Select one ;
* Click on ADD SELECTED PROGRAMS.
### In the list of your games :
* Right click on the launcher ;
  * Select Properties ;
  * Compatibility ;
  * Check "Force the use of a specefic Steam Play compatibility tool" ;
  * Select one of the GE proton version that you put in the compatibilitytools.d folder ;
  * close the window.
* Launch your launcher ;
### Once the install of the launcher is done :
* You have to right click againe one the launcher ;
* Properties ;
* change the path in the <u>shortcut</u> section, in <span style="color:red">target</span> and in <span style="color:red">start in</span> :
  * the path have to be something like this the following path.
  * >/home/user/.local/share/Steam/steamapps/compatdata/1234567890/pfx/drive_c/users/steamuser/Desktop/**[Launcher].lnk** ;
### In compatdata, to find which of the number like 1234567890 is your launcher, refers you to the date/houre that it was made, that can help you.
### So, when you find the .lnk laucher, just copy the all path in the <span style="color:red">target</span> and <span style="color:red">start in</span> of the properties of you're launcher on steam.

### thank you for reading this process.
