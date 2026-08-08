An Internet-synchronized digital clock for the ESP32 featuring an **SSD1306 OLED display** (128x64 pixels). It automatically syncs time via NTP servers and displays dynamic sun or moon icons based on the time of day.

## Features
* **NTP Time Sync:** Accurate time via `pool.ntp.org` (configured for UTC+4).
* **Dynamic UI:** Sun/Moon icons change automatically based on the hour.
* **Auto-Reconnect:** Automatically recovers Wi-Fi connectivity.

## Hardware Setup
| Component | ESP32 Pin |
| :--- | :--- |
| **SDA** | GPIO 33 |
| **SCL** | GPIO 25 |

## Quick Start
1. Clone this repository or copy the code into the Arduino IDE.
2. Update your Wi-Fi credentials in the file:
   ```cpp
   const char* ssid = "YOUR_SSID";
   const char* password = "YOUR_PASSWORD";
