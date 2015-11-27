#Updating the launcher
Gridlauncher is in pretty much constant development, and so there are frequent updates. To make it easier for users to keep up to date with the latest version, @ihaveamac created a built-in updater. You can access this as follows:
1. Open Gridlauncher settings (the top left icon on the main grid)
2. Open the Software Update option, which is the following icon:

![Settings icon](settingsicon.png)<br>

The launcher will then check which version is the latest in this Github repository, and offer to download and install the update for you.

##Updating when using boot managers
Gridlauncher communicates not only its current version number, but also its current 3dsx filename and location to the updater. The updater will overwrite the file specified by Gridlauncher. For example, if your boot manager is /boot.3dsx and Gridlauncher is /boot1.3dsx, then /boot1.3dsx will be overwritten with the latest version of Gridlauncher by the updater.

##Updates to the updater
The package downloaded by the updater will also include the latest version of the updater itself, and this will be installed when the update is applied. The updater is therefore able to update itself.