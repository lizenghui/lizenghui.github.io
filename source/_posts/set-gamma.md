---
title: set gamma
date: 2018-10-31 10:45:57
categories: "ubuntu"
tags:
  - ubuntu
  - color
  - gamma
---

Open terminal and enter this command:
```
xrandr -q | grep " connected"
```
output is: LVDS-1-1 connected primary 1366x768+0+0 (normal left inverted right x axis y axis) 309mm x 173mm

Copy the value that comes before "connected". In this case as you can see its "LVDS-1-1" Yours might me something else.

Now try this command replacing "LVDS-1-1" with the value you got from the previous command.
```
xrandr --output LVDS-1-1 --gamma 0.8:0.8:0.8
```
The last three decimal values separated by colon sets the gamma value. The values have a range from 1.0:1.0:1.0 to 0.0:0.0:0.0 Default is 1.0:1.0:1.0

### Note:: I use xrandr to set brightness on my display. It will sometimes reset to the default value, sometimes during a program launch. So I use a script with a desktop shortcut for convenience.


