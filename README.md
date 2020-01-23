# ESP32-Relay-8
PPV2-Simulation project with ESP32 and Lua-RTOS

A circuit board with 8 power relays. Work as a WiFi access point and is controlled with an Android app.

# Step by step

## Hardware 

Order the board from a manufacturer, use the Eagle PCB files. The board is one-sided. Solder mask is highly recommended.

Load all components. One socket for the ESP board and two for the relay module.

Detach the plugs from the relay module and solder them in again from below.

The spacers for the relay module are 10mm long. Adjust if necessary.

## Software

### ESP Module

The ESP module needs new firmware with Lua-RTOS. It is available here https://github.com/whitecatboard/Lua-RTOS-ESP32. To flash the firmware and file system, please follow the instructions. The board type is generic.

### p+

The app on the board was created with p+. p+ is available here https://github.com/Mynogs/PPV2-Simulation-System.

Please set the user level to 2 in p+.

### Android

I use the IoT Remote Control software on my Android phone.

Add a new button in the app. Configure it as follows:

Action Type: UDP

Content q.q = true

Host: 192.168.4.1

Port: 20000

This turns on the first realy.

Insert the next button, this time with q.q = false. This switches off the first relay.

The second relay is called q.r, the third q.s and so on.
