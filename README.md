# End Table Dashboard

## Overview
The **End Table Dashboard** is a compact smart display designed to sit neatly on a nightstand or side table.  
It’s built around an **ESP32** microcontroller and features a **2.4" TFT display**, a **momentary push button**, and a **custom 3D-printed enclosure**.

The device connects directly to your **Home Assistant** instance via **ESPHome**, allowing it to fetch and display real-time data from your Home Assistant entities — such as temperature, humidity, or any other sensor values you choose to integrate.  

In my setup, the built-in button is used for **remotely controlling the room light**, so I can easily turn it on or off without having to get up and reach the main switch.  

## Features
- Single push button  
- SHT40 temperature and humidity sensor  
- 2.4-inch TFT display  

## Parts Used
- [ESP32 WROOM32 Development Board](https://aliexpress.com/item/1005006449303342.html)  
- [Waveshare 2.4" TFT Display](https://aliexpress.com/item/1005009014044858.html)  
- [DFRobot SHT40 Temperature & Humidity Sensor](https://www.dfrobot.com/product-2437.html)  
- [400-slot Breadboard (55 × 83 mm)](https://aliexpress.com/item/1005007085965483.html)  
- [Momentary Push Button](https://aliexpress.com/item/4001081730289.html)  
- [Male-to-Female Dupont Wires](https://aliexpress.com/item/1005004647016228.html) and [U-shape Breadboard Wires](https://aliexpress.com/item/1005007175633091.html)  
- 2 × M2 × 3 mm socket screws  

## Schematic
## Breadboard Connections
<img src="https://github.com/CezarZcezar/End-Table-Dashboard/blob/master/Images/Connection_Schematic.png" style="width:50%;">

## Enclosure
<img src="https://github.com/CezarZcezar/End-Table-Dashboard/blob/master/Images/Enclosure.png" style="width:50%;">

## Final Assembly
<img src="https://github.com/CezarZcezar/End-Table-Dashboard/blob/master/Images/Inside_View_1.JPEG" style="width:50%;">
<img src="https://github.com/CezarZcezar/End-Table-Dashboard/blob/master/Images/Assembled_View_1.JPEG" style="width:50%;">
<img src="https://github.com/CezarZcezar/End-Table-Dashboard/blob/master/Images/Assembled_View_2.JPEG" style="width:50%;">

## Software

### Installation Using Web Browser
To install the firmware, connect your ESP32 board to a PC and flash the software using the **ESPHome Web Builder** in your Home Assistant server, or directly from the [ESPHome website](https://web.esphome.io/).  
Remember to **enter BOOT mode** before the first flash.

### Installation Using Python Utilities
Alternatively, you can flash the firmware using Python utilities: `esphome` and `esptool`.

1. Install the required tools:
   ```bash
   pip install esphome esptool
   ```
2. Compile the firmware:
   ```bash
   esphome compile .\end_table_dashboard_1.yaml
   ```
   After compilation, a project folder will be created. Locate the firmware.bin file and copy it to the parent directory.
3. Flash the firmware (remember to specify the correct COM port):
   ```bash
   esptool --port [port] --baud 115200 write_flash --flash_size=detect 0x00000 firmware.bin
   ```
## Future improvements
- Add air quality sensors
- Design a dedicated PCB
