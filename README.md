# Live Clock with Date and Time

## Overview
This project is a live clock application that dynamically displays the current date and time in an animated and visually appealing format. It connects to Wi-Fi to fetch accurate time data from the internet and automatically adjusts for daylight saving time (DST). Built on the Arduino platform, it is designed to be modular, customizable, and easy to use.

![WhatsApp Image 2025-01-19 at 11 58 49 PM (1)](https://github.com/user-attachments/assets/d2ee99b2-067e-4e09-99fd-34536d71a0b4)



## Features
- **Live Time Display**: Continuously updates to show the current time in real-time.
- **Date Integration**: Displays the date along with the time.
- **Wi-Fi Connectivity**: Connects to the internet using Wi-Fi to synchronize time via Network Time Protocol (NTP) servers.
- **Daylight Saving Time Support**: Automatically detects and adjusts for daylight saving time based on your location.
- **Smooth Animations**: Implements animated transitions for digits for an engaging user experience.
- **Modular Design**: Built with object-oriented programming principles for easy customization and scalability.

![WhatsApp Image 2025-01-19 at 11 58 49 PM](https://github.com/user-attachments/assets/5acd5960-caaa-4fb8-91f5-d091c4bf7bdb)


## Components
### `Digit.h`
Defines the `Digit` class, which represents an individual digit in the clock display. It includes:
- Attributes like `value`, `newValue`, `frame`, `height`, and position coordinates (`x`, `y`).
- Methods for accessing and modifying digit properties, setting positions, and managing frames.

### `Digit.cpp`
Implements the methods defined in `Digit.h`. Key functionalities include:
- Getting and setting digit values.
- Managing animation frames.
- Setting and retrieving digit positions.

### `RollingClock.ino`
The main Arduino sketch that:
- Connects to Wi-Fi and synchronizes time using NTP servers.
- Automatically adjusts for daylight saving time based on the configured time zone.
- Instantiates and manages `Digit` objects.
- Handles real-time updates for the clock.
- Implements the display logic and animations.

## Author
- Affan Beg
## How to Use
### Requirements
- **Hardware**: Arduino-compatible microcontroller with Wi-Fi support (e.g., ESP8266 or ESP32).
- **Software**: Arduino IDE and necessary libraries (WiFi, NTPClient, etc.).

### Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/YourUsername/live-clock
