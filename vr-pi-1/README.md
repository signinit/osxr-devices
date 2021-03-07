# vr-pi-1

PoC device using RPI (3/4)

## Build Items

* Raspberry PI 3 B+ (should support higher versions - not tested)
* Waveshare 4inch HDMI LCD Resistive Touch Screen 800x480 ([3d model](display.display.dwg))
* double convex lenses with 42mm diameter, 68mm focal length
* power supply / battery pack
* standard M3 bolds and nuts

## 3D Printing Parts

* ([Lens Brachet](lens-bracket-v1.stl))
* 2x ([Side Bracket](side-brackets-v2.stl)) (1x mirrored)

## RPI Setup Instructions (not tested)

install raspbian lite

put config.txt into boot

run `sudo tvservice -d edid.dat`

sudo raspi-config
enable opengl kms
enable autologin
set gpu-memory 256

`sudo apt-get install xorg`

`startx`

`xrandr -o left`

install and run osxr

## TBD

* rebuildable / buyable headstrap
* create raspbian version (auto rebuild for every new osxr version)
* add external sensor mounting and connections (e.g. camera, gyro sensor, bluetooth, ...)
* improve wearing comfort