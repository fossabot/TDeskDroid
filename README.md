# TDeskDroid - Telegram Desktop to Android theme converter
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FMrYadro%2FTDeskDroid.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2FMrYadro%2FTDeskDroid?ref=badge_shield)


## Dependencies
- python 3
- tinify
- pip3 (pip for python 3)
- pillow (follow Installation instructions)
- requests

## Installation
1. Install python 3 for your OS
2. Download or clone this repo to your PC
3. Go to that directory and run `pip3 install -r requirements.txt` via command prompt / terminal / whatever

## Converting
1. Put `.tdesktop-theme` files (the one is zip file) to `desktop` directory
2. If you want to optimize your jpeg you have to get your api key here https://tinypng.com/developers put it in `tinify.key` and change `tinyJpeg` to True
3. If you need to override some theme colors (if that's a bug please report it) you can use `%themefilename%.map` e.g. `windowBackgroundWhite=#ffffffff` one rule per line
   You can apply multiple overriding for theme packs. For example, if your theme file is named `MyTheme.Dark.1.0.tdesktop-theme`, you can use
   `MyTheme.map`, `MyTheme.Dark.map`, `MyTheme.Dark.1.map` and `MyTheme.Dark.1.0.map` for overriding theme packs.
4. Run `python3 main.py` via command prompt / terminal / whatever
5. Go to directory `android`, and send `.attheme` file to TG chat, then apply it

## About atthemes
- Colors in `.attheme` file are signed int from `ARGB` (yep color alpha goes first)
- Image has to be converted to `jpeg`, and put in binary mode into file between tags PWS and WPE
- `.atthemesrc` is sort of source file made by me so you can check it in more human friendly way on how conversion goes
- You have to use all the colors in `.tdesktop-theme` file


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FMrYadro%2FTDeskDroid.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2FMrYadro%2FTDeskDroid?ref=badge_large)