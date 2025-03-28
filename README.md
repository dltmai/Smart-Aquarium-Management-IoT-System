﻿# Smart Aquarium Management IoT System
## Overview
The Smart Aquarium Management IoT System is an intelligent aquarium monitoring and automation system that utilizes IoT technology, AI-driven recommendations, and mobile app control. The system collects real-time sensor data, processes it using an AI recommendation model, and controls the aquarium environment via ESP32.

## Features
- Real-time Sensor Monitoring: Tracks water quality parameters such as pH, temperature, TDS, and ammonia levels.

- AI Recommendation Model: Provides suggestions based on sensor readings (e.g., water change alerts, pH stabilizer recommendations).

- Automated Feeding System: Schedules and executes feeding times based on fish species and dietary needs.

- Remote Control via Mobile App: Allows users to control the filtration and feeding system remotely.
  
- Multi-Protocol Communication: Uses MQTT for device control, HTTP/WebSockets for cloud interactions, and BLE for initial setup.

## Protocols Used:
- MQTT: For controlling devices (e.g., feeding and filtration control).

- HTTP/WebSockets: For cloud data transmission and real-time monitoring.

- BLE: For initial device setup and configuration.

## Functional Flow

1. Read sensor data from aquarium.

2. Process data using the AI recommendation model.

3. Update the mobile app with the latest system status.

## Routing Table

| Condition | Action | 
|------------------|-------|
| pH < 6.5          | Alert user, recommend adding pH stabilizer   | 
| TDS > 300 ppm      | Alert user, suggest a partial water change  |
| Scheduled Feeding Time| Activate feeder motor |


## System Updates & Maintenance

- Add/Remove fish species to update feeding schedules and maintenance routines.

- Adjust nutrition, medication, and probiotic recommendations.

- Modify aquarium settings based on fish type data.

- Perform OTA firmware updates to enhance AI and system functionality.

## Demo Scenarios

- Monitor live water quality metrics via the mobile app.

- Schedule and execute automatic feeding.

- Control the filtration system remotely from the mobile app.
