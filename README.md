# Pozyx-Linux-library
A Linux/RPi library for use with the Pozyx shield.

Modified from https://github.com/pozyxLabs/Pozyx-Arduino-library to use linux/i2c-dev.h header or [pigpio library](http://abyz.co.uk/rpi/pigpio/index.html) for bitbanged i2c on Raspberry Pi.

Tested on Minnowboard Turbot and Raspberry Pi 2 (with firmware 0.9 and before library updates to v1.0). Might require installing packege libi2c-dev on Linux or pigpiod library on RPi.

The platform can be selected in Pozyx.h by defining either LINUX or RPI. Used gpio pins can be set in Pozyx_core.cpp (default GPIO 338 for interrupts on Linux and pin 2 for SDA, pin 3 for SCL and gpio 17 on RPi (BCM numbering)).

All the examples haven't yet been updated for Linux. Orientation_3D -example should work, building can be done with make.

The library requires **firmware version 1.0** installed on the Pozyx devices.

Documentation for the library can be found here:
https://www.pozyx.io/Documentation/Datasheet/arduino

The following folders can be found together with this library:

1.  **examples**. These example scripts showcase some basic functionality of the Pozyx device, each example comes with a tutorial that can be found on the pozyx website https://www.pozyx.io/Documentation
2.  **unit_test**. This folder contains a collection of Arduino scripts that can be run to test certain functionalities of the Pozyx device. They also serve as some good examples for some Arduino library functions.
3.  **useful**. This folder contains a number of useful Arduino sketches that provide basic functionality such as discovering all pozyx devices or configuring them.
