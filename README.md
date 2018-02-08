# gnome-reddit-wallpaper

## Overview

A python script which by default will retrieve the top image of the day from https://www.reddit.com/r/EarthPorn/ and sets it as the wallpaper in the GNOME windows manager. Also contains an optional ``` redditwallpaper.desktop ``` file that can be placed inside of the ``` .config/autostart ``` folder.

## Requirements

To execute, there are some python packages that need importing as well as Python 3+

``` Python
import praw
import urllib

```

Python script which takes an image from a subreddit and sets it as Gnome's wallpaper

## Options

When executing the script, there are some options available:

* ```--overwrite``` Allows overwriting of the image, regardless of whether there is already one saved.
* ```--sub <name>``` Without this it will default to r/earthporn but a different subreddit can be specified.
* ```--time <time>``` Defaults to the best of the 'day' but other options exist e.g. 'all', 'year', 'month'.