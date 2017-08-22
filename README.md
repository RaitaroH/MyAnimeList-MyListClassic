# MyAnimeList
![alt tag](https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/MyList%20-%20DeepDark.png)
My custom classic style for MAL. See bellow the code you need to use.

This is a style inspired by [FT DeepDark](https://addons.mozilla.org/en-US/firefox/addon/ft-deepdark/?src=search).

Credit to [Shishio-kun's](https://myanimelist.net/profile/Shishio-kun) tutorials (and who contributed to those) and [dzikibambus](https://myanimelist.net/profile/dzikibambus) for improvements to the anime images hover.

Also, credit where credit is due for the color palettes and images down bellow. ([@KDE](https://github.com/KDE), [@linuxmint](https://github.com/linuxmint))

<b>CLASSIC STYLE ONLY!</b>

My list [here](https://myanimelist.net/animelist/RaitaroHikami).

# Screenshots
![alt tag](https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/Screenshot.png)

# Installation
Follow the instructions from [here](https://myanimelist.net/forum/?topicid=200320#msg8158307). Under step 5 simply choose what code you want from bellow instead of the example provided on that page.

MAL.css is the common code for anime and manga pages.

Anime-specific.css has the code for the anime covers and also anime title hightlight. Covers.css has the anime cover images.

Manga-specific.css is like Anime-specific but also has incorporated the covers.

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

Also, under Anime-specific.css the code for anime titles highlighting is. Those anime are recommendations by me, so you should remove that code or change it to the anime you want.


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
--banner-height: 110px;
```
Note that sprites-hover is still in deepdark colors. You might also want to change --sprites-hover url to the white variant seen in the next example. Same with the 404 image.

Also note that the banner should be 990x250px or anything with that aspect ratio. Try to have the banner image as centered as possible. The banner-height variable should be played with to see if the banner looks better. I find it easier just to have the banner of proper aspect ration instead.

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
--banner-height: 110px;
--404: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/404_White.png");
--mal: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/MAL.png");
/*Sprites*/
--sprites: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/Sprites-transparent.png");
--sprites-hover: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/SpritesHoverWhite-transparent.png");
```
Note: 404 image and --sprites-hover changed to white variant.

Result:
![alt tag](https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/KDE_Screenshot_Green.png)



Linux Mint reproduction:
```
--main-color: rgba(154, 184, 124,1) !important;
--main-background: rgba(47, 47, 47, .7) !important;
--second-background: rgba(56, 56, 56, .7) !important;
--hover-background: rgba(64, 64, 64, .8) !important;
--main-text: rgba(255, 255, 255, 1) !important;
--dimer-text: rgba(255, 255, 255, .7) !important;
--shadow: rgba(154, 184, 124, .9) !important;
--title-highlight: rgba(154, 184, 124, .9) !important;
--border-color: rgba(47, 47, 47, 1) !important;
/*Images*/
--wallpaper: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/LM_Wallpaper2.png");
--banner: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/LM_Banner.png");
--banner-height: 100px;
--404: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/404_White.png");
--mal: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/MAL.png");
/*Sprites*/
--sprites: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/Sprites-transparent.png");
--sprites-hover: url("https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/SpritesHoverWhite-transparent.png");
```

Result:
![alt tag](https://raw.githubusercontent.com/RaitaroH/MyAnimeList/master/Images/LM_Screenshot.png)
