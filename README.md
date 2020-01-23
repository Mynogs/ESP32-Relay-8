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

The ESP module needs new firmware with Lua-RTOS. It is available here https://github.com/whitecatboard/Lua-RTOS-ESP32. To flash the firmware and file system, please follow the instructions. The board type is generic.

The app on the board was created with p+. p+ is available here https://github.com/Mynogs/PPV2-Simulation-System.

Please set the user level to 2 in p+.

