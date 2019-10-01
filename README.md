# HalloweenBox

The HalloweenBox project is inspired by the 'Uncanny eyes' project from Adafruit.  The code to create the eyes for the HalloweenBox, including the graphic files and the code to render the eyes on LCD screens, is taken from Adafruit.  The code for this project was customized to add sound, a button trigger, and PIR sensor.  

Hardware:
- Teensy3.2 board
- Adafruit ST7735 128x128 TFT display x 2
- Serial MP3 Player v1.0 WH-311 (Found on Amazon)
- PIR Sensor
- Wooden Box (from Michaels)
- 3D printed Eye holder

For reference:
How-to guide with parts list and 3D models is here:
https://learn.adafruit.com/animated-electronic-eyes-using-teensy-3-1/overview

Teensy 3.x: use 72 MHz board speed

Directory 'HalloweenBox' contains Arduino sketch. 'graphics' subfolder has various eye designs, as #include-able header files.

Folder 'convert' contains Python sketch for generating graphics header files. Requires Python Imaging Library. Example images are also in this directory.

Pin List:

0: Left Eye Wink
1: Both Eye Blink
2: Right Eye Blink
3: PIR
4: LITE (pull low to turn off display backlight)
5: RX for MP3 Player module (optional - needs to be defined but not connected)
6: TX for MP3 Player module
7: Display (Eye) Data/Command
8: Disply (Eye) Reset
9: Right Eye Select
10: Left Eye Select

A0: Joystick X (currently not used)
A1: Joystick Y (currently not used)
A2: Light pin for photocell (currently not used)

