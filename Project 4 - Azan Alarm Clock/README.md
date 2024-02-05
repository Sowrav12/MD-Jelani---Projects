# Prayer Alarm System with Arduino

## Overview
This project aims to create a prayer alarm system using Arduino Uno components. The system will play a unique sound of the user's choice for each of the five daily prayers. The prayer times will be dynamically fetched from a JSON file stored on an external storage device.

## Components
- Arduino Uno board
- RTC (Real-Time Clock) module
- External storage device (e.g., SD card)
- Speaker
- Breadboard
- Jumper wires
- Power supply (9V battery or wall outlet)

## Setup
1. Connect the RTC module to the Arduino Uno following the datasheet instructions.
2. Connect the speaker to the Arduino Uno using the breadboard and jumper wires.
3. Insert the external storage device (SD card) into the Arduino Uno's SD card slot.
4. Connect the power supply to the Arduino Uno (either a 9V battery or a wall outlet).

## Usage
1. Prepare the JSON file containing the prayer times for each day of the year.
2. Ensure the JSON file is named `prayer_times.json` and stored in the root directory of the external storage device.
3. Power on the Arduino Uno.
4. The system will automatically read the current date and time from the RTC module and fetch the corresponding prayer times from the JSON file.
5. At each prayer time, the system will play the specified sound through the speaker.

## JSON File Structure
The `AzanTimes.json` file should have the following structure:
```json
{
  "January": {
    "1": {
      "Day": "Monday",
      "Date": 1,
      "Fajr": [6, 15],
      "Shorooq": [7, 15],
      "Dhuhr": [12, 30],
      "Asr": [15, 15],
      "Maghrib": [17, 45],
      "Isha'a": [19, 0]
    }
  }
}
```
## Authors
&copy; MD Golam Jelani and Depanker Shrestha
