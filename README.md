MacOS Dual Screen Wallpaper Changer
======================

Applescript for applying a split wallpaper across multiple desktops.

Based on code from:
- Philip Hutchison, April 2013
- http://pipwerks.com
- MIT license http://pipwerks.mit-license.org/

## What it does

It randomly selects two halves of a split image from a directory and
applies them to the primary and secondary desktops.

## How to use it

### Folder structure

Create ``~/Pictures/Wallpapers/dual screen`` directory and fill it with
images.  Pairs of images should have the same name except for one should
contain a "\_P\_" and the other should contain a "\_S\_"


### Script file

You can run the script manually using the Script Editor, or on the CLI
with ``osascript``

```shell
osascript wallpaper.scpt
```

To automatically change the background periodically use geektool, or
crontab

```shell
*/30 * * * * osascript ~/path/to/wallpaper.scpt 
```
