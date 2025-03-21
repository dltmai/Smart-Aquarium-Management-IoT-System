﻿# Smart Aquarium Management IoT System
 
## Introduction
The **Smart Aquarium Management IoT System** helps you manage your aquarium in a smart, automated, and effortless way. It uses sensors to monitor water quality, controls devices via ESP32, and offers a mobile app for real-time monitoring.

---

## Key Features
- Real-time **water quality monitoring** (pH, TDS, temperature...)
- **AI recommendations** for aquarium care
- Automated feeding schedule
- Remote control of **filtration and feeding system** via mobile app
- Add/Remove fish types, nutrition, and medication

---

## Main Data Structures
- **SensorData**: Sensor data (pH, TDS, temperature...)
- **FeedingSchedule**: Feeding time and amount
- **DeviceState**: Status of filtration and feeding systems

---

## System Workflow

### Initialization:
ESP32 powers on → Connects to Wi-Fi → Syncs with server → Sets up BLE (first-time setup)

### Main Operations:
Read sensors → AI processes data → Control devices → Update status → Notify mobile app

### Example Processing:
| Condition             | Action                                        |
|----------------------|-----------------------------------------------|
| pH < 6.5              | Alert user, recommend using pH stabilizer    |
| TDS > 300 ppm         | Alert user, suggest partial water change     |
| Feeding time arrived  | Activate feeding motor as scheduled          |
