#Banners
Banners are images which are displayed on the top screen when a homebrew app, title, shortcut, theme or folder is highlighted in a grid. Two types of banners are supported:

1. **Full screen banners:** If a full screen banner is present, the title, author and description text will not be shown on the top screen
2. **Small banners:** If a small banner is present, the title, author and description text will be shown on the right hand side of the top screen. Note that the small banner image is actually the same size as the full screen banner, so you will need to make sure the image does not overlap the text (or that if it does, it does not affect the readability of the text)

If no banner is present, then the icon highlighted on the grid will be displayed in its place along with the title, author and description text. If both banner images are present, then the full screen banner will take priority and the small banner will be ignored.

Banner files must all be PNG format and should be placed within one of the following locations. They can contain transparency and this is recommended for the best visual effect. All banner images, whether full screen or small banners, must be 400x222 pixels in size.

##Banner filenames and locations
The presence of the suffix '-fullscreen.png' indicates that the banner will prevent the title, author and description text from being displayed when the banner is shown. Text shown in pointed brackets should be replaced with the relevant information.

Filenames|Location|Description
--------|--------|-----------
\<appname\>-banner.png<br>\<appname\>-banner-fullscreen.png|The folder containing a 3DS homebrew app. \<appname\> must be identical to the part of the 3dsx filename before the extension.|Banners for 3DS homebrew apps.
\<shortcutname\>-banner.png<br>\<shortcutname\>-banner-fullscreen.png|The folder containing an XML shortcut. \<shortcutname\> must be identical to the part of the shortcut XML file filename before the extension.|Banners for XML shortcuts.
\<titleid\>-banner.png<br>\<titleid\>-banner-fullscreen.png|/gridlauncher/titlebanners/. \<titleid\> must be identical to the part of the title ID of the title. You can obtain the title ID by highlighting the title in the grid and pressing SELECT.|Banners for titles installed on the 3DS and game carts.
folder-banner.png<br>folder-banner-fullscreen.png|/gridlauncher/folders/\<myfolder\>/, where \<myfolder\> is the folder for which you want to add the banner|Banners for Gridlauncher folders.
theme-banner.png<br>theme-banner-fullscreen.png|/gridlauncher/themes/\<mytheme\>/, where \<mytheme\> is the folder for the theme for which you want to add the banner|Banners for Gridlauncher themes.

##Examples
![A cart without a banner](wiki/bannernone.png)
![A cart without a full screen banner](wiki/bannerfull.png)
![A cart without a small banner](wiki/bannersmall.png)