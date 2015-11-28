#Installation
When you launch a homebrew exploit such as Ninjhax, the exploit will look on your 3DS SD card for a file called boot.3dsx. When the exploit is first installed, this file will be added to the SD card to provide a way of launching other homebrew apps. Gridlauncher replaces the boot.3dsx file to provide a more feature-rich launcher.

##Downloading the launcher
**[Download the latest version](https://github.com/mashers/3ds_hb_menu/raw/master/launcher.zip "Download the latest version")**

The latest version of the launcher can always be downloaded by getting launcher.zip from the repository.

##Copying the launcher to your 3DS
The easiest way to get the files onto your 3DS is to remove the SD card, place it in a card reader, and connect it to your computer. Then unzip launcher.zip downloaded from above, and you will be provided with one file and one folder:
* **boot.3dsx** - the launcher itself
* **gridlauncher** - a folder containing the built-in updater and a copy of HANS used for title booting

Simply copy these to the root of your SD card, replacing the existing files. Eject the SD card, put it back into your 3DS, and run your homebrew exploit to load Gridlauncher.

##Boot managers
Some 3DS homebrew users use a boot manager as their boot.3dsx. This allows you to select between different apps or launchers when initially starting your homebrew exploit. In this situation, the boot manager is boot.3dsx and should not be overwritten. Instead, you should rename Gridlauncher's boot.3dsx to something else, place it in the root of your SD card, and then configure your boot manager to launch it. Please refer to the documentation for your boot manager for more information on how to configure this.
