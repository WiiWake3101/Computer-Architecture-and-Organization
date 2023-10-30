# RFID-Based Attendance System using Arduino

This repository contains the Arduino code for an RFID-based attendance system. The system is designed to work with an Arduino board, an RFID module (MFRC522), a 16x2 LCD display, and some LEDs and a buzzer. It allows you to grant or deny access based on the RFID card's unique identifier (UID).

## Features
- Recognizes and logs attendance based on RFID card UID.
- Displays user information on an LCD screen.
- Provides visual and auditory feedback (LEDs and buzzer) to indicate access status.
- Supports multiple RFID cards for access control.

## Components Required
- Arduino board
- MFRC522 RFID module
- 16x2 LCD with I2C interface
- LEDs (Green and Red)
- Buzzer
- RFID cards (UIDs need to be configured in the code)

## Wiring Instructions
- Connect the MFRC522 RFID module and the I2C LCD to the appropriate pins on the Arduino.
- Connect LEDs (Green and Red) and the buzzer to the specified pins on the Arduino.
- Make sure to power the RFID module separately if required.

## Installation
1. Install the Arduino IDE on your computer if you haven't already.
2. Open the Arduino IDE and create a new project.
3. Copy and paste the provided code into your Arduino project.
4. Save the project with a suitable name.

## Configuration
- Customize the code by changing the UID values in the `loop()` function to match the RFID cards you want to grant access. You can add more card UIDs and corresponding user information as needed.
- Adjust the LED and buzzer pins if you've connected them to different pins on your Arduino.

## Usage
1. Upload the code to your Arduino board.
2. Place the RFID cards in the proximity of the RFID module.
3. When a recognized RFID card is detected, the system will display the user's name on the LCD, activate the green LED, and produce a brief buzzer sound.
4. If an unauthorized card is detected, the system will display an "UNAUTHORIZED ACCESS" message, activate the red LED, and produce a different buzzer sound.

## Credits
- This code is based on the RFID-Based Attendance System tutorial provided by [Techatronic](https://techatronic.com/rfid-based-attendance-system-using-arduino/).

For more detailed information, code comments, and a full demonstration of the project, please refer to the original tutorial linked above. Enjoy using your RFID-based attendance system!

**Note:** Be sure to properly handle and secure access to the code to prevent unauthorized modifications or access to your system.
