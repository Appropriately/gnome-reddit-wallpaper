# gnome-reddit-wallpaper

## Overview

A python script which by default will retrieve the top image of the day from https://www.reddit.com/r/EarthPorn/ and sets it as the wallpaper in the GNOME windows manager. Also contains an optional `redditwallpaper.desktop` file that can be placed inside of the `.config/autostart` folder, that retrieves a new wallpaper on start up.

## Installation

Installation can either be done using the provided `install` script.

## Requirements

To execute, there are some python packages that need importing as well as Python 3+
As long as pip is usable, the `install` script can handle module installation.

``` Python
import praw
import wand
import urllib
```

## Options

When executing the script, there are some options available:

* `--overwrite` Allows overwriting of the image, regardless of whether there is already one saved.
* `--sub <name>` Without this it will default to r/earthporn but a different subreddit can be specified.
* `--time <time>` Defaults to the best of the 'day' but other options exist e.g. 'all', 'year', 'month'.