## RFID Attendance System

This project implements an RFID-based attendance system using ESP8266 and various connected modules. The system is designed for educational purposes, providing a foundation to learn about RFID technology, ESP8266, and integrating additional components like an LCD and sensors.

## Features

* RFID card scanning for attendance recording.
* Tracks entry and exit times.
* Handles offline storage with text files in case of WiFi failure.
* Push-button functionality to confirm actions.
* Modular connections include an LCD for display and an RTC for timekeeping.
  
## Components Used

* ESP8266 Microcontroller
* RFID RC522 Reader
  * SDA -> D8 (GPIO15)
  * SCK -> D5 (GPIO14)
  * MOSI -> D7 (GPIO13)
  * MISO -> D6 (GPIO12)
  * RST -> D3 (GPIO0)
  * 3.3V -> 3V3 pin
  * GND -> GND pin
  * 16x2 LCD
  * SDA -> GPIO5 (D2)
  * SCL -> GPIO4 (D1)
* Ultrasonic Sensor
  * VCC -> +5V
  * Trig -> GPIO11
  * Echo -> GPIO12
  * GND -> GND
* Push Buttons: Connected between 3V3 and A0
* WiFi LED: Connected to GPIO2 (D4)
* SD Card Module: Standard SPI connections
* RTC Module: Connected via GPIO pins
  
- Refer to the Connections of Modules section for a detailed wiring guide.

## Getting Started

### Prerequisites
  * Install the Arduino IDE.
  * Configure the ESP8266 board settings in the IDE.
  * Install necessary RFID, RTC, SD card, and LCD module libraries.
    
### Setup
  1. Wire all components as specified above.
  2. Load the provided code onto the ESP8266.
  3. Use the serial monitor for debugging and system feedback.
     
### Usage
  1. Scan the RFID card to record attendance.
  2. Press the push buttons to confirm or modify entries.
  3. Utilize the LCD for real-time feedback and updates.
     
## Educational Purpose Disclaimer

This project is intended solely for educational purposes. It is designed to demonstrate the basic principles of RFID and microcontroller-based systems.

## License
This code may have been created based on the works of other individuals and resources. Proper credits have been maintained where due. Users are encouraged to respect intellectual property rights while utilizing this project.
