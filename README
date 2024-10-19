#dwm - dynamic window manager
============================
## dwm is an extremely fast, small, and dynamic window manager for X.


## Requirements
This configration build on my ThinkPad E590 Voidlinux. In order to build dwm you need the Xlib header files.

```sh
sudo xbps-install xorg base-devel libX11-devel libXft-devel libXinerama-devel freetype-devel fontconfig-devel fribidi-devel
```

## Installation
To installation you must clone the repository and  install the requirements. 

```sh 
git clone https://github.com/Senior-Moe/dwm.git ~/.config/suckless/dwm
sudo xbps-install xorg base-devel libX11-devel libXft-devel libXinerama-devel freetype-devel fontconfig-devel fribidi-devel
```
Afterwards enter the following command to build and install dwm (if
necessary as root):

    make clean install


## Running dwm
Add the following line to your .xinitrc to start dwm using startx:

    exec dwm

In order to connect dwm to a specific display, make sure that
the DISPLAY environment variable is set correctly, e.g.:

(root is necessary)
- make xsessions
```sh
mkdir /usr/share/xsessions
```
- make file dwm.desktop in xsessions directory
```
[Desktop Entry]
Encoding=UTF-8
Name=dwm
Comment=Dynamic window manager
Exec=dwm
Icon=dwm
Type=XSession
```


In order to display status info in the bar, you can do something
like this in your .xinitrc:

    while xsetroot -name "`date` `uptime | sed 's/.*,//'`"
    do
    	sleep 1
    done &
    exec dwm


## Configuration
The configuration of dwm is done by creating a custom config.h
and (re)compiling the source code.
