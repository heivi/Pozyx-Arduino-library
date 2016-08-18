# Pozyx-Linux-library
A Linux/RPi library for use with the Pozyx shield.

Modified from https://github.com/pozyxLabs/Pozyx-Arduino-library to use linux/i2c-dev.h header or [pigpio library](http://abyz.co.uk/rpi/pigpio/index.html) for bitbanged i2c on Raspberry Pi.

Tested on Minnowboard Turbot and Raspberry Pi 2. Might require installing packege libi2c-dev on Linux or pigpiod library on RPi.

The platform can be selected in Pozyx.h by defining either LINUX or RPI. Used gpio pins can be set in Pozyx_core.cpp (default GPIO 338 for interrupts on Linux and pin 2 for SDA, pin 3 for SCL and gpio 17 on RPi (BCM numbering)).

The examples haven't yet been updated for Linux. 

See more documentation and the tutorials for these examples at:
https://www.pozyx.io/Documentation
