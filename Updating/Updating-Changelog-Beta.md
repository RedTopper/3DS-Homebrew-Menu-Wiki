## Beta 129
* Added support for grid icon overlay images in themes. Please see the Icon Overlays page in the Wiki for details.

## Beta 128
* Includes updater 2.1, which adds the following:
 * Lots of code cleanup
 * Error handling
 * Automatic creation of /gridlauncher/updater.cfg with a setting to skip info and automatically exit if the latest and installed version numbers do not match. (There's currently no way to enable this in the program)
 * Several UI improvements
* Displays the info and non-grid wallpapers on title error pages

## Beta 127
* Adds banners for themes. Same image format as the other banner images. Place them in the theme folder and call the file theme-banner.png or theme-banner-fullscreen.png

## Beta 126
* All menus (including the title menu) now refresh their icon layout when the number of rows is changed
* Includes updater v2.04 by @ihaveamac

## Beta 125
* Fixes issues with title-based apps (SVDT, HANS, Braindump) not getting the correct title ID.

## Beta 124
* Fixed a crash bug when using d-pad navigation or opening the title menu.

## Beta 123
* Added full screen banners. These have exactly the same format as normal banners. The filename and location is the same, except they have -banner-fullscreen.png at the end instead of just -banner.png. If a banner with -fullscreen.png is found, then the app's title, author, description and panel will not be displayed, so the banner can be seen full screen.

## Beta 122
* Cart banners now show on the main grid and update when carts are changed.

## Betas 120/121
* Addresses a bug retrieving the title ID from carts when they are inserted.

## Beta 119
* Titles can now display banners too. The launcher will automatically create a folder for them (/gridlauncher/titlebanners/). To help with creating the banner for the titles, the boot options screen now shows the title ID. So heres how you create the app banner:

 1. Press SELECT on the title to bring up the boot options menu and make a note of the title ID
 2. Create the banner in the same format as homebrew app banners
 3. Name the file titleid-banner.png (where titleid is the id shown on the boot options menu)
 4. Place the file in /gridlauncher/titlebanners/
* This does not yet work for the cart on the main grid as it does not have the title ID stored.

## Beta 118
* Added banners to HANS shortcuts. They need to be exactly the same format as homebrew app banners. Name them as per the following example:
 * /gridlauncher/folders/Games/mvdk.xml
 * /gridlauncher/folders/Games/mvdk-banner.png

## Beta 117
* SELECT button no longer shows the boot menu when a homebrew app is selected
* Selecting the cart icon when no cart is inserted now no longer causes the boot sound to play
* Fixed 3dslink progress display (again)
* Fixed display of top screen icons if no app banner is present
* Improved the audio waiting code - this now works with titles as well as homebrew apps

## Beta 116
* Adds banners for folders. Same format as app banners. Put them in the folder and call the file folder-banner.png
* Removed screenshots for now to make space for new features. This might come back later, but for now use the home button to take screenshots using the screenshot feature built in to hax 2.5.

## Beta 115
* Includes @smileyhead's excellent suggestion of app banners. Here's how they work:
 * Create a 400x222 pixel PNG image to use as the banner. I strongly recommend using transparency in this image so it doesn't cover the wallpaper entirely.
 * Put whatever you want on the banner image
 * Save it as appname-banner.png (where appname is identical to what comes before .3dsx in the app's 3dsx filename)
 * Put the banner image in the same folder as the 3dsx
* Now when the app is selected, the banner image will be shown instead of the icon.

## Beta 114
* Adds updater 2.01 by @ihaveamac
* Fixes progress indicator display when transferring files over 3dslink

## Beta 113
* Adds options for which logo to show. The option to show/hide the logo has now changed to cycle between four options: Gridlauncher (the default (new) logo), Gridlauncher compact (a smaller version of the default), HBL classic (the original logo) and None. The option is saved on a per-theme basis. The old setting to hide the logo is no longer used, so if it was hidden before then you will need to go back into your theme settings and cycle the setting to None.

## Beta 112
* Hopefully fixed HANS and XML shortcuts
* Fixed cursor getting lost when leaving the top left corner button using the DPad controls in the folder menu
* Fixed missing body text on reboot page

## Beta 111
* Splash screens for rebooting. These need to be named wallpapertopreboot.png (400x240) and wallpaperbottomreboot.png (320x240) and placed in the theme folder. They will be displayed after selecting the Reboot option
* Date display is now optional. You can disable it in the main settings

## Beta 110
* Fixes a bug populating the title menu for some apps which need them (e.g. Retroarch)
* Now displays the date on the status bar

## Beta 109
* Fixed a bug with the cart icon not showing if the title menu is opened without a cart inserted
* Changed HANS missing error page, SD missing error page, Netloader and boot options to use the info wallpapers
* Removed the long press recogniser to open the boot menu. Now, you need to highlight an app/title icon and press SELECT to bring up the HANS/R4 boot menu
* Fixed a hang when launching titles using HANS if the titles are still loading in the background
* Rounded the corner of the tick symbol
* New logo

## Beta 108
* Fixes a bug which caused the grid to be un-selectable when changing pages while corner buttons are selected
* Fixes bug launching cart using HANS from main grids
* Added boot option (HANS/Region4) manual override. Hold down on an app/title and after a couple of seconds a menu will pop up to allow you to choose whether to boot the app using HANS or Region4. This will override the HANS title booting option in settings
* Fixes a bug in which filtered titles would be reset if backing out of the title filter options before the titles had finished loading

## Beta 107
* Panel colours can now be changed

## Beta 106
* Fixed long theme titles overlapping theme author text

## Beta 105-a
* Updated HANS version in the archive to the latest version

## Beta 105
* HANS title booting

## Betas 102-104
* Test builds to try to fix the audio issues when returning from an XML title.

## Beta 101
* Prevent launching the cart from empty folders
* Fixed loading of title preload setting
* Reboot menu now shows the info and non-grid wallpapers (if available)
* Fixed corner button A selection

## Beta 95-100
* Testing releases

## Beta 94
Merges changes by @RedHat:
* Removed homemenuhax splash screen. Please use PNG splash screens from now on
* Added default theme splash screen. If /gridlauncher/themes/Default/splashtop.png and splashbottom.png exist, these will be shown if the currently selected theme does not contain splash images of its own
* Fixed memory leak in audio

## Beta 93
* Support for PNG top and bottom splash screens. Format the same as top and bottom wallpaper, call them splashtop.png and splashbottom.png, and place them in the theme folder. The splash screen for the currently selected theme will be shown on boot.
* Support for boot sounds. Format the same as BGM.bin, call it bootsound.bin, and place it in the theme folder. The boot sounds for the currently selected theme will be played on boot.
* Removes a lot more unneeded stuff from tinyxml to make space for new features

## Beta 91/92
Merges fixes by @RedHat:
* Changed Left/Right audio effect
* Removed audio pop
* Fixed audio load bug
* Includes fixed updater lua script

## Beta 90
* Fixes a crash when opening folders if there are no folders in /gridlauncher/folders and /3ds folder is hidden
* Sounds placed in the default theme folder will now be played if they do not exist in the currently selected theme

## Beta 89
* Support for backsoundbin, which will be played when exiting menus such as settings.

## Beta 88
* Added sound effects to corner buttons

## Beta 87
* This update adds move and select sound effect support. Place the files movesound.bin and selectsound.bin in your theme folder. The files need to be in the same format as BGM.bin. Your themes will then play the sounds when moving around the grid and selecting apps.

## Beta 85
* Fixed help menu crash
* Fixed software update author name
* Current folder will now be selected in the folders grid
* Moved random theme on wake option to theme settings

## Beta 84
* Background music and splash screen support c/o @RedHat
* Proper migration to ctrulib great-refactor branch

## Betas 81-83
* Various broken commits. Move along...

## Beta 80
* Support for HANS shortcuts
* Stripped out some unneeded code from tinyxml and other places too

## Beta 79
* Removed requirement for updater config.txt.

## Beta 78
* Memory management: theme images now freed on exit

## Beta 77
* Now logs the executable path and current version for parsing by the updater.

## Beta 76
* Typo fixes on settings page.

## Beta 75
* Adds framerate control - animations should now run at 30fps regardless of the hardware
* Added the option to hide the /3ds folder from the folders list
* Integrated support for @ihaveamac's amazing updater app. Just copy the files from /gridlauncher in the zip file to the root of your SD card and the update option will appear in gridlauncher settings

## Beta 74
* Just updated beta version number to test updater app

## Beta 73
* Fixes to random theme selection

## Beta 72
* Support for up to 16 frames in progress wheel animations. Create 36 x 36 PNG images (alpha optional) called progressWheelFrame1.png ... progressWheelFrame16.png and put them in the theme folder. When the theme is loaded the files will be loaded consecutively, and will stop when there are no more files, when 16 frames are reached, or when an invalid size or format image is encountered.

## Beta 71
* Fix theme selection for themes with smdh data

## Beta 70
* Support for custom progress wheel graphics. Create 36 x 36 PNG images (alpha optional) called progressWheelFrame1.png ... progressWheelFrame6.png and put them in the theme folder. If any of the frame images is missing or incorrect then none of them will be used and the default wheel will be shown
* Support for a different wallpaper on the bottom screen for non-grid pages. Call this file 'wallpaperbottomnongrid.png' and put it in the theme folder. It will automatically be detected and loaded when the theme loads
* Shows theme info from theme.smdh. If this file is not present or contains no information then the theme's folder name will be displayed instead

## Beta 69
* Displays a progress wheel while loading titles
* Top screen panels now show full width on info pages so they do not overlap the text
* Support for a different wallpaper on the top screen for info pages. Call this file 'wallpapertopinfo.png' and put it in the theme folder. It will automatically be detected and loaded when the theme loads

## Beta 68
* Fixes to grid handling:
 * Return from top left icon now returns to first column if RF loader is hidden
 * Main grid is now reselected when returning from the folders menu
 * Theme select and folders menus are now reselected when returning from their help pages

Thanks to @Goombi on GBATemp for contributions to these fixes.

## Beta 67
* Fix reloading already loaded title lists

## Beta 66
Bugfixes to background title loading:
* Pausing and resuming title loading should work properly now
* Launching an app while background loading is paused should now force the background load to cancel and the thread to die (therefore preventing a hang in this situation)

## Beta 65
* Improved background loading of the title menu. The "Title preload" option has now been replaced with "background title loading". If you enable this, then the titles will start loading and appearing in real time when you open the title menu. If you close the title menu before it has finished loading, the loading will be paused and will resume again when you re-enter the title menu. Hopefully this will improve stability on devices where the original title preload, which started as soon as the launcher booted, was causing lockups. This feature is very beta. I don't have many titles on my 3DS to test with, so I can't be 100% certain that this is stable or consistent. If you have problems, please report them in this thread and disable the background loading option.

## Beta 64
* Support for booting XML titles (not HANS shortcuts yet, just apps like Ironhax installer and others)
* Power off option in the START menu

## Beta 63
* Fixes title launching from the main grid.

## Beta 62
* Fixed panels being drawn on top of text

## Beta 61
* Various fixes merged from @Garcia98 including New3DS speedup on hax 2.5
* Added loading screen to folder opening
* Removed tid.bin saving for title launching
* Fixed duplicate cart icon in title menu

## Beta 60
* Added optional animation for transitions between grids.

## Beta 59
* Cursor position is now preserved when changing pages with the shoulder buttons or on-screen page controls. The cursor will still move to the first column when paging right or the last column when paging left with the d-pad controls.
* The tick indicator in the settings now has a background so it shows up better against the icons.

## Beta 58
* Ignored titles are now managed within settings so ignoredtitles.txt does not need to be edited.

## Beta 57
* Single row grid option

## Beta 56
* Adds an option to show the ID of the currently selected title in the bottom left corner of the top screen.

## Beta 55
* Adds random theme option in the theme selection page.

## Beta 54
* Fix for top wallpaper being duplicated on the bottom screen

## Beta 53
* Adds support for custom toolbar button backgrounds and symbols. These images all need to be 36x36 PNG images placed in your theme folder with the following names:

* Button backgrounds:
 * buttontopleft.png buttontopleftselected.png buttontopright.png buttontoprightselected buttonbottomleft.png buttonbottomleftselected.png buttonbottomright.png buttonbottomrightselected.png

* Button symbols:
 * backicon.png foldersicon.png helpicon.png homeicon.png settingsicon.png

## Beta 52
* Adds support for custom app icon background images. Place these in your theme directory as follows:
 * appbackground.png: 56 x 56 pixels. This is the background for unselected apps or empty spaces
 * appbackgroundselected.png: 56 x 56 pixels. This is the background for the currently selected app
 * cartbackground.png: 59 x 59 pixels. This is the background for the region free loader / cart when it is not selected
 * cartbackgroundselected.png: 59 x 59 pixels. This is the background for the region free loader / cart when it is currently selected

* The launcher will automatically detect whether the images have an alpha channel so it makes no difference whether the images have transparency or not. They will automatically be masked to the correct shape with rounded corners and the tab for the cart icons. You will get an error in log.txt if the images are invalid or the wrong size. You do not need to change any settings - the presence of the images is enough (as with wallpapers).

## Beta 51
* Settings have been separated into submenus:
 * Grid settings (3rd row, icon backgrounds, wraparound scrolling, dpad navigation)
 * Theme settings (water, colours, translucency, panels, logo, theme select)
* In addition, the water settings have been moved a submenu within the theme settings.

## Beta 50
* Resolves an issue with the folder selection not saving.

## Beta 49
* Rolls back the change to C arrays for menu entries due to huge issues with this approach.

## Beta 48
* The D-Pad navigation setting is now saved along with the other settings
* After using dpad button navigation on the folders or themes pages, the folders/themes grid would have no selection when returning to it. This is now fixed.
* Changes the menu entry storage from a linked list to a C array. This means entries can be added in any order (not necessarily in sequence), which is a step towards page-by-page loading of menus

## Beta 47
* Icons on the settings now draw correctly when toggling the third row
* Folders and themes grids now show a tick on the currently selected item, and prevent re-selection of the currently selected item
* Strange text appearing in the 'author' position when selecting some settings or help items has been fixed
* The colour preview on colour mixer screens is now right justified to prevent it overlapping the text

## Beta 46
* Fixes the bug where empty grid positions could be selected.

## Beta 45
* Prevents theme names from being truncated, meaning that theme names which are longer than the available space on the line can still be selected.
* Improves the colour mixer pages in settings by adding a preview of the colour being adjusted.

## Beta 44
* Folders and themes now draw in grids instead of the ugly button lists. They will show default icons with the first letter of the folder/theme on top, or if folder.smdh or theme.smdh is placed inside the folder/theme directory then the image inside this smdh will be used as the icon for the grid. This change also removes the 8 folder/theme limit, as the folder/theme grids inherit the paging ability of the other grids so can show as many themes/folders as are on the device.
* In addition, the “Reboot” icon now changes its text to “Rebooting…” when it has been activated so the user will know the device is in the process of rebooting.
* Finally, I have created a spinning progress wheel. This isn’t used anywhere yet but is included in this commit.

## Beta 43
* Fixes an issue where it was not possible to select the first column of icons after enabling the region free loader
* Screenshots are now saved in /gridlauncher/screenshots/. This folder will be created automatically when the launcher boots
* Added an option to adjust the offset of the top panel from the left edge of the screen

## Beta 42
* When returning to a grid after selecting a toolbar button with the dpad controls, the first icon in the grid will be selected instead of leaving the grid with no selection. Also a binary 3dsx is now included.

## Beta 41
* All menus now show the same number of rows, as determined in the settings
* Improved blocking of touches when moving between screens, resulting in a more responsive interface
* The bug with light text disappearing if red or green are set to 10 or 13 seems to be resolved now
* Improved updating of the UI when adjusting colour sliders or setting colours to default
* Increased the number of lines available for app descriptions from two to four
* D-Pad controls throughout the menu

## Beta 40
* Corrected the information on the folders help page
* XML titles now boot correctly when title preloading is disabled
* The tool bar icon backgrounds alpha slider no longer displays its value twice
* The help system has been improved with separate pages for about, folders, themes and ignoring titles all with a nice menu

## Beta 39
* Background loading of titles is now optional. If you have been having problems with stability since the introduction of this feature please try disabling it in the settings. The default settings is ON so you will need to go in and disable it if you don't want to preload the titles. You will then need to restart the launcher for this to take effect
* Proper icon for the theme selector
* Improved loading screen layout (if you have title preload disabled)
* Fixes a hang with the save manager if title preloading is disabled

## Beta 38
* All files and folders are now located in /gridlauncher. The necessary folders are created when the launcher opens if they don't already exist
* Folders no longer need the .hbfolder extension
* The word "Author:" has been removed from the app details
* Adjusting colours no longer triggers the config to save - it's just saved once when you exit the settings
* The title menu now shows the same number of rows as the main menu
* Toolbar button symbols now have their own alpha slider
* Theme selector - switch between any of the themes in /gridlauncher/themes/

## Beta 37
* Back panels for top and bottom screens now have independent alpha values
 * Default value is zero so they will not be visible initially
 * Set the alpha value to whatever looks best for your theme
 * Set to zero to disable the panel
* Page controls now have back panels
 * These use the same alpha value as the bottom panel
 * They are drawn in the 'inactive' colour so they match the app icon backgrounds
* Status bar images have been brought two pixels away from the edges of the screen
* Added an option to disable the jiggly-water-on-keypress effect

## Beta 36
* Changing the transparency of toolbar buttons will now also affect their shadow and icon
* Added the back button to the folders help page
* Added the option to add a translucent panel where text is shown to improve readability when using wallpapers
* Background loading of titles - no more loading screen!
* Ejecting/inserting a cart no longer triggers a reload of the whole title list - it just toggles the visibility of the cart icon

## Beta 35
* Fixed the problem with the toolbars not refreshing when changing their colour
* Added separate transparency options for top bar, static water, app icon shadow, bottom bar, toolbar icons, app backgrounds and paging controls. I will add support for translucent moving water when I figure out how! If anyone can have a look at gfxDrawWave() and gfxDrawSpriteAlphaBlendFade() in gfx.c from the original launcher and see if they can find some clues I would really appreciate it, as I don't seem to be able to work this out.
* Colour selection is now displayed in a nice grid with icons I drew this afternoon

## Beta 34
* Adds translucent toolbars when the translucent UI option is enabled!

## Beta 33
* Fixed a bug with the drawing of empty app backgrounds

## Beta 32
* Added support for wallpaper PNG files with a transparency channel. The background colour will show through any transparent areas.
* Fixed the bug which left a gap in the app backgrounds if the region free launcher was disabled
* Added an option to hide the “homebrew launcher” logo
* Separate title text colour now configurable in the theme settings. This allows you to change the colour of the app name title text on the top screen so it no longer has to match the colour of the top bar
* Icons for the new options in settings

## Beta 31
* The water enabled setting wasn't being saved - fixed!
* Added a check to make sure the background wallpapers are the correct size
* Adds an option in settings for a translucent UI. Currently this only affects the icon backgrounds and borders, but it makes the bottom screen look much better when using a custom wallpaper

## Beta 30
* The selected app indicator is now no longer drawn on top of the grid background, meaning the corners should look clean now
* Fixed the bug with the paging arrows appearing when toggling the third row of icons
* Added an option to disable the water completely
* Finally added custom wallpapers!
* Create a 400 x 240 PNG with no alpha channel (transparency). Call it wallpapertop.png and place it in the root of your SD card
* Create a 320 x 240 PNG with no alpha channel (transparency). Call it wallpaperbottom.png and place it in the root of your SD card
* The launcher will automatically find the files and set them as the wallpaper
* You may want to turn the water off in the settings so you can see the wallpaper properly

## Beta 29
* This update improves the screenshot code. Screenshots are now rotated in processing so are saved the right way round. Both screens are now drawn in one (larger) image so you don't have two separate files for the screenshot. Also, the screenshot PNG files are given unique filenames so they no longer get overwritten when you take another screenshot.

## Beta 28
* I have removed the old settings screen with the plain icons and turned the settings page into a grid in the same style as the main menu and title launcher. Each setting has its own icon and displays details on the top screen, along with a tick on the icon if the setting is enabled. The settings looks much more attractive now :)

## Beta 27
* The selected folder now has a tick on it
* Cleanup of button code
* SCREENSHOTS! Press X at any time and the screen will freeze for a fraction of a second. FTP in to your 3DS or put your SD card into your computer, and you will see /hbl-grid-screenshot-top.png and /hbl-grid-screenshot-bottom.png in the root of the SD card. The files are rotated 90 degrees at the moment as ctrulib and libpng use opposite coordinate systems. I just need to rotate the array containing the framebuffer data to get it in the correct orientation but I'm getting crashes in that code at the moment, so for now just rotate the image 90 degrees left after taking the screenshots

## Beta 26
* Tidied up the folder select screen, making space for two more folder buttons (8 in total now)
* The folder will no longer reload if the same folder is selected again
* The theme data is now stored in a separate config file so themes can be shared without overwriting other settings
* Custom water colours now apply also to still water
* Colour adjustment sliders now have (ugly) plus and minus buttons for finer tuning

## Beta 25
* Back button on settings page now unhighlights if you drag off of it
* Loading page when populating/updating the title menu
* Customisable colour scheme in settings - adjust the colours of the ting, background, inactive buttons, water and text
* Enabled options in the settings now display a tick instead of turning that horrible green colour

## Beta 24
* Title menu no longer allows selection of empty spaces
* Cart icon always shows in the title menu even if RFL is disabled in the grid settings
* Waves now move out of the way on the folders help page
* Waves no longer overlap the top status bar when they drop

## Beta 23
* This update fixes the problems with wraparound scrolling, and also adds a feature to ignore certain titles in the title menu. You will need to place ignoredtitles.txt from the archive in the root of your SD card along with boot.3dsx. This is a comma separated file which lists the title IDs which should be ignored. I have already placed in here the title IDs for six titles which the title launcher is unable to launch, so these will now be excluded from the menu. If you want to exclude any other titles, you can edit ignoredtitles.txt to add the title ID. If you need to know the title ID, try to boot it (it doesn't matter if it crashes) and then open bootlog.txt from your SD card. Copy the title ID from this file, then edit ignoredtitles.txt. Add a comma at the end and then the title ID. Make sure you don't add any spaces or other characters, and don't end the line with a comma

## Beta 22
* Adds optional wraparound scrolling (default is on, can be disabled in the settings). When enabled, both page scrolling arrows will be visible all the time as long as there is more than one page in the grid; scrolling before the first page will wrap to the last page, and scrolling after the last page will wrap to the first page.

## Beta 21
* The cart icon has now been moved to the first position on the title menu, and has the cart background
* The title menu now detects cart removal/insertion. It will no longer crash if you select the cart icon when no cart is inserted, and will successfully boot whichever cart is inserted
* System Transfer now shows the correct name in the title menu

## Beta 20
* Title menu scans for titles only the first time you open it. Subsequent times will not re-scan. If you insert or remove a cart then the titles list will be rescanned next time you open it
* The third row of icons now fits properly
* The icons are now properly centralised in two row mode
* The title launcher can now be closed with the B button
* Tapping in the top left corner of the screen now no longer closes the about page

## Beta 19
* Properly centralised time no matter what time or format it is being displayed in
* Title launcher! The bottom right button with a little home symbol on it will let you choose a title and launch it (thank you @suloku for the title launching code!)
* Version number is now displayed on the about page
* The waves now slide down to get out of the way of the text on the about page and slide back up again when it's close. For the best effect, do this with the animation on. It looks so cool ;)

## Beta 18
* Cart tab on the region free launcher
* Less harshly rounded borders on app icons
* The grey backgrounds on empty spaces in the grid are now optional

## Beta 17
* Fixed duplicate apps in title menu

## Beta 16
* Added temporary logging of title IDs for debugging title menu

## Beta 15
* This version finally, after several days of head-scratching, makes the title browser display in a grid like the main menu. This was a LOT of work as I had to extract the grid drawing code from the main menu and make it generalisable for other menus, then write code to translate the title browser data to the same structure as the main menu, pass the newly structured title menu to the new grid drawing function, and handle selection of a title from the grid (rather than a .3dsx). The hardest part was figuring out how to pass the title ID from the title browser to the grid menu data, then getting it back out again to find out which title was actually selected.

## Beta 14
* This version should fix the bugs exiting the launcher

## Beta 13
* Fixed a bug quitting the launcher using the start button

## Beta 12
* Bug fixes to text engine

## Beta 11
* This version adds support for unicode characters in the font engine. Please note that currently the only character I have actually added is 'é'. Also added rounded corners to the buttons in settings/folders

## Beta 10
* Uses the font Roboto using my custom font engine (to be released separately when fit for human consumption)
* Improves the display of the SVDT thing, along with instructions to use the D-Pad to select the title for any users who were expecting the titles to be displayed in a grid
* Passes the title selected to SVDT, so hopefully that's working how people are expecting now (I can't be sure since none of the people who have complained about it have yet explained what the problem is)

## Beta 9
* Improved performance of configuration. Previously, every time a single option was changed the whole config was loaded from SD card, the changed option was applied, and the whole config was then saved back to disk again. Now, the config is loaded from SD once, any changes are applied in memory, and the save routine is called separately so many config options can be changed and then saved once. This improves the performance of exiting the settings, which was previously slow and quite jumpy
* The grid now displays the icon for the currently selected cart where the region free launcher goes. Selecting the cart's icon now shows the details of the game on the top screen instead of the region free launcher. Changing carts results in this information being refreshed, and if no cart is inserted then the region free logo is displayed
* The confirmation to launch a cart has been removed. This was inconsistent with the home menu, and also inconsistent with all the other apps in the grid which launch as soon as you select them. So now, selecting to launch a game using the region free loader will make the game start straight away

## Beta 8
* The left arrow button now shows correctly if you are on > page 1
* The option to hide the region free launcher is now only visible if the region free launcher is actually available. The option is forced ON if the region free launcher is not available to prevent the first icon being hidden or inaccessible should the region free launcher not be installed
* I have drawn a new disabled wifi icon which I hope is clearer

## Beta 7
* Made the shadows around the toolbar buttons a bit more subtle
* Added a separate button to open the folders list (tapping the bar at the top still does the same, but I thought an individual button was needed)
* The animated water is now optional. If you disabled animated water in the settings then a still image of the water will be displayed

## Beta 6
* Folder support

## Beta 5
* Design update based on the amazing concept uploaded by @link6155
 * The waves have been reinstated
 * The app icon on the top screen is original size now (and thus no longer pixellated) and is now decorated by a nice drop shadow
 * The homebrew launcher icon is back
 * The blue in the colour scheme has been changed
 * The page arrows and indicators have been redrawn and recoloured to tie in better with the colour scheme
* In addition:
 * The toolbar icons on the bottom screen have been redrawn and have a nice shadow now
 * The corner radius of the icons has been adjusted so they are not as rounded
 * The region free loader now shows the game icon only on the top screen instead of the extra one on the bottom screen

## Beta 4
* 12/24 hour clock in the settings and also draws placeholders on the grid instead of white space where there are missing app icons (i.e. if there aren't enough to fill up the grid).

## Beta 3
* The bug with touch controls not working after the first page is fixed.
