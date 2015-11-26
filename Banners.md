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
&ltappname&gt-banner.png<br>&ltappname&gt-banner-fullscreen.png|The folder containing a 3DS homebrew app. &ltappname&gt must be identical to the part of the 3dsx filename before the extension.|Banners for 3DS homebrew apps.