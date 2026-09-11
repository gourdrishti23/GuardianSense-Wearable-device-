# GuardianSense-Wearable-device-
ESP32-based wearable system for fall detection, health monitoring, GPS tracking and GSM emergency alerts.
# GuardianSense – Wearable Fall Detection & Health Monitoring System

## Overview

GuardianSense is an ESP32-based wearable safety and health-monitoring
system designed to detect possible falls, monitor basic health
parameters, track the user's location, and provide emergency
notifications.

## Features

- Real-time fall detection
- Heart-rate monitoring
- SpO₂ monitoring
- Temperature monitoring
- GPS-based location tracking
- GSM-based emergency SMS
- Local emergency alert
- OLED/LCD display for system information
- Rechargeable battery-powered operation

## Hardware Used

- ESP32
- Motion Sensor
- Temperature Sensor
- Pulse Oximeter
- GPS Module
- GSM/SIM Module
- OLED/LCD Display
- Rechargeable Li-ion Battery

## Technologies Used

- Embedded C/C++
- ESP32
- Sensor Interfacing
- I2C Communication
- UART Communication
- GPS
- GSM
- IoT

## Working

The sensors continuously provide motion and health-related data to
the ESP32. A threshold-based algorithm analyzes the motion data to
detect a possible fall.

When a fall is detected, the system generates a local alert and
displays an emergency message. If the alert is not cancelled within
the defined time, the GPS module obtains the user's location and the
GSM module sends an emergency SMS to the designated contact.

## System Flow

Sensors → ESP32 → Fall Detection
        ↓
   Local Alert
        ↓
   GPS Location
        ↓
   GSM Emergency SMS
