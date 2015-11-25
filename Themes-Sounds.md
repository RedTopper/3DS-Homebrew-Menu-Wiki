#Themes -> Sounds and BGM
Gridlauncher supports background music, which is played on a loop, and sound effects, which are played when certain actions are taken. The files must be placed within the theme folder.

##Creating theme audio files
1. Download an MP3/MP4/whatever you want as BGM.
2. Load it up in audacity/any audio editor.
3. Delete all of the tracks but one (If it is stereo, make it mono, for example. The result should leave you with a mono file.)
4. Edit how you like it (make it louder, longer, faster, stronger).
5. Change the project rate to 44100Hz if it isn't already.
6. Export it as a WAV (Microsoft) signed 16bit PCM file.
7. Rename it to one of the file names below and put it in your themes folder.

##Audio files
Filename|Description
--------|-----------
BGM.bin|Background music played on a loop while the launcher is running
movesound.bin|The sound made when the cursor moves
selectsound.bin|The sound made when something is selected, e.g. on a grid
backsound.bin|The sound made when exiting a menu
bootsound.bin|The sound made while the splash screen is being displayed
