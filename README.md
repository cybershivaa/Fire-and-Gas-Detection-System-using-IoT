IoT-Based Fire and Gas Detection System using Arduino

This project demonstrates a real-time fire and gas detection system using Arduino Uno, an MQ2 gas sensor, flame sensor, and a 16x2 I2C LCD. It is designed to detect hazardous gas concentrations and fires, and display alerts for safety automation. Ideal for homes, laboratories, and small industrial environments.

📌 Features

🚨 Real-time detection of smoke/gas and fire
📟 LCD display with I2C showing current status
🔔 Buzzer alert on detection
✅ Startup message to indicate system readiness
⚙️ Easily expandable for IoT (e.g., GSM module, cloud logging)

🧰 Hardware Required

| Component            | Quantity |
|----------------------|----------|
| Arduino Uno          | 1        |
| MQ-2 Gas Sensor      | 1        |
| Flame Sensor         | 1        |
| 16x2 LCD Display (I2C) | 1        |
| I2C Module for LCD   | 1        |
| Buzzer               | 1        |
| Jumper Wires         | As needed |
| Breadboard           | 1        |
| 9V Battery or USB    | 1        |

🔌 Circuit Connections

MQ-2 Gas Sensor
- VCC → 5V  
- GND → GND  
- A0  → A0 (Analog pin)

Flame Sensor
- VCC → 5V  
- GND → GND  
- D0  → D2 (Digital pin)

Buzzer
- + → D4  
- – → GND

LCD with I2C Module
- VCC → 5V  
- GND → GND  
- SDA → A4  
- SCL → A5  

💻 How to Use

1. Connect the components as per the above table.
2. Upload the final Arduino code from this repo using the Arduino IDE.
3. Open Serial Monitor (9600 baud) to see the system logs.
4. LCD will show:
   - `System is Ready...` at startup
   - `Smoke Detected!` if gas is detected
   - `Fire Detected!` if flame is detected
5. The buzzer will sound for each detection.

