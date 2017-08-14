# MyAnimeList
![alt tag](https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/MyList%20-%20DeepDark.png)
My custom classic style for MAL. See bellow the code you need to use.

This is a style inspired by [FT DeepDark](https://addons.mozilla.org/en-US/firefox/addon/ft-deepdark/?src=search).

Credit to [Shishio-kun's](https://myanimelist.net/profile/Shishio-kun) tutorials (and who contributed to those) and [dzikibambus](https://myanimelist.net/profile/dzikibambus) for improvements to the anime images hover.

Also, credit where credit is due for the color palettes and images down bellow. ([@KDE](https://github.com/KDE))

<b>CLASSIC STYLE ONLY!</b>

My list [here](https://myanimelist.net/animelist/RaitaroHikami).

# Screenshots
![alt tag](https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/Screenshot.png)

# Installation
Follow the instructions from [here](https://myanimelist.net/forum/?topicid=200320#msg8158307). Under step 5 simply choose what code you want from bellow instead of the example provided on that page.

# Anime list
```
@import "https://rawgit.com/RaitaroH/MyAnimeList/master/MAL.css";
@import "https://rawgit.com/RaitaroH/MyAnimeList/master/Anime-specific.css";
@import "https://rawgit.com/RaitaroH/MyAnimeList/master/Covers.css";
#copyright
{
visibility: visible;}
```

# Manga list
```
@import "https://rawgit.com/RaitaroH/MyAnimeList/master/MAL.css";
@import "https://rawgit.com/RaitaroH/MyAnimeList/master/Manga-specific.css";
#copyright
{
visibility: visible;}
```
# Customization - no import
In case you do want to customize then you will have to use the code as is and NOT import it.

Under MAL.css, at the top, under root, color variables and image variables for the banner and background can easily be changed to meet your tastes. Is that simple.

If you don't want covers don't import Anime/Manga specific and Covers css.


Reproducing KDE Neon with a transparent look:
```
--main-color: rgba(61, 174, 233,1) !important;
--main-background: rgba(35, 38, 41, .7) !important;
--second-background: rgba(42, 46, 50, .7) !important;
--hover-background: rgba(49, 54, 59, .8) !important;
--main-text: rgba(239, 240, 241, 1) !important;
--dimer-text: rgba(239, 240, 241, .7) !important;
--shadow: rgba(61, 174, 233, .5) !important;
--title-highlight: rgba(61, 174, 233, .9) !important;
--border-color: #232629 !important;
/*Images*/
--wallpaper: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/KDE_Wallpaper.png");
--banner: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/KDE_Banner.png");
```
Note that sprites-hover is still in deepdark colors. You might also want to change --sprites-hover url to --sprites' url.

Also note that the banner should be 990x250px.

Result:
![alt tag](https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/KDE_Screenshot.png)

Or for a green color instead:
```
--main-color: rgba(61, 192, 141,1) !important;
--main-background: rgba(35, 38, 41, .7) !important;
--second-background: rgba(42, 46, 50, .7) !important;
--hover-background: rgba(49, 54, 59, .8) !important;
--main-text: rgba(239, 240, 241, 1) !important;
--dimer-text: rgba(239, 240, 241, .7) !important;
--shadow: rgba(61, 192, 141, .9) !important;
--title-highlight: rgba(61, 192, 141, .9) !important;
--border-color: #232629 !important;
/*Images*/
--wallpaper: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/KDE_Wallpaper.png");
--banner: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/KDE_Banner.png");
--404: url("");
--mal: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/MAL.png");
/*Sprites*/
--sprites: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/Sprites-transparent.png");
--sprites-hover: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/Sprites-transparent.png");
```
Note: 404 image removed. --sprites-hover changed to --sprites.

Result:
![alt tag](https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/KDE_Screenshot_Green.png)
