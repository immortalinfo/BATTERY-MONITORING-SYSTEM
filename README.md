# BATTERY-MONITORING-SYSTEM
code on how sensors measure the parameters like voltage, current, and temperature

This project uses an ESP32 microcontroller, a DHT11 sensor, and an ACS712 current sensor to monitor voltage, current, and temperature. The data is sent to ThingSpeak for visualization, and a buzzer alerts when thresholds are exceeded.

---

Features
- Reads **temperature** using DHT11.
- Measures **voltage** via ESP32 ADC.
- Measures **current** using ACS712 sensor.
- Sends data to **ThingSpeak** cloud platform.
- Triggers **buzzer alert** if voltage/current exceeds safe limits.
- WiFi-enabled data logging.

---

 Hardware Requirements
- ESP32 Development Board
- DHT11 Temperature Sensor
- ACS712 Current Sensor (30A version)
- Buzzer
- Jumper wires, breadboard, power supply

---

 Pin Connections
| Component | ESP32 Pin |
|-----------|-----------|
| DHT11 Data | GPIO 4 |
| Voltage Sensor | GPIO 34 (ADC) |
| Current Sensor | GPIO 35 (ADC) |
| Buzzer | GPIO 26 |
---
 Software Requirements
- Arduino IDE (with ESP32 board support installed)
- Libraries:
  - `WiFi.h` (built-in for ESP32)
  - `DHT.h` (install via Arduino Library Manager)

---

 Setup Instructions
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/esp32-energy-monitor.git
