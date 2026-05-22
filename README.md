# Cybersecurity : CSN150

## Project: ESP32 CAM

## Purpose
Set up ESP32 CAM.

## Equipment
- ESP32Cam
- USB Micro Data Cable

## Links to documentation and tools
- Video 1: https://youtu.be/4inE-n6kXSE
- Arduino ESP32 install guide: https://docs.espressif.com/projects/arduino-esp32/en/latest/installing.html
- ESP32 WiFiScan example: https://github.com/espressif/arduino-esp32/blob/master/libraries/WiFi/examples/WiFiScan/WiFiScan.ino
- CH341SER driver: https://www.wch-ic.com/downloads/CH341SER_ZIP.html

## AI GPTs used
- Perplexity AI

## Steps I followed
1. Installed Arduino IDE.
2. Added the ESP32 board package in Arduino IDE.
3. Selected the correct ESP32 board and COM port.
4. Opened the ESP32 CAM example sketch.
5. Uploaded the sketch to the ESP32.
6. Opened the Serial Monitor to view available Wi-Fi networks.

## Problems and Solutions
### Problem
`E (485) camera: Camera probe failed with error 0x105(ESP_ERR_NOT_FOUND) Camera init failed with error 0x105`

### Solution
Checked the camera connections, reseated the camera module, and verified the correct camera board configuration. Camera probe errors are commonly caused by loose camera flex connections or incorrect camera interface configuration. [web:3][web:6][web:9]

### Problem
Arduino code would not load on ESP32-CAM.

### Solution
Installed the correct USB-to-serial driver. In this case, the **CH341SER** driver was used successfully. Some ESP32 boards also require the CH340/CH341 family driver before the COM port appears correctly in Arduino IDE. [web:16][web:19]

## Final Report
The ESP32 was set up successfully in Arduino IDE, and the CAM sketch was uploaded and run. The Serial Monitor displayed nearby Wi-Fi networks and signal information, confirming the board was working as intended. [web:11][web:14]
