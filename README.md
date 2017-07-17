WiFi Serial Interface
=====================

This sketch turns an ESP8266 (ESP-01) into a WiFi serial interface.

Port 23 gives a RAW serial interface at 115200 baud. Great for running
with `socat`, for instace:

$ sudo socat pty,link=/dev/ttyACM99,raw,wait-slave tcp:192.168.0.8:23

Port 24 gives an RFC2217 compatible interface including the ability to
set the baud rate. (**Work In Progress**)
