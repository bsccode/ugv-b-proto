

## Overview

This repository hosts the code and documentation for a prototype autonomous unmanned ground vehicle (UGV). Designed for experimentation with autonomous navigation and control systems, the prototype leverages a Raspberry Pi 4B and an ESP32 for core computing and wireless communication. Equipped with a motor set controlled via an L298 motor driver, it showcases precise movement and maneuverability capabilities.

## Hardware Requirements

- **Raspberry Pi 4B**: Central processing unit.
- **ESP32**: For wireless communication and peripheral control.
- **L298 Motor Driver**: Controls the motors.
- **Motors (2x)**: DC motors for propulsion.
- **Chassis**: Structure holding all components.
- **Wheels (4x)**: Provide mobility.
- **Ultrasonic Sensors**: Detect obstacles. (TODO)
- **Infrared Sensors**: For line following. (TODO)
- **IMU (Inertial Measurement Unit)**: Determines orientation. (TODO)
- **GPS Module**: Enables outdoor navigation. (TODO)
- **Compass (Magnetometer)**: Indicates heading direction. (TODO)
- **LIDAR Sensor**: Advanced obstacle detection and mapping. (TODO)
- **Camera Module**: For visual data processing. (TODO)
- **Battery and Power Management System**: Powers the prototype.
- **Wheel Encoders**: Measure wheel rotation.

## Software Requirements

- **Arduino IDE**: For ESP32 programming.
- **Python**: For control algorithms on Raspberry Pi.
- **ROS (Robot Operating System)**: Optional, for advanced robotics projects.

## Installation

1. **Raspberry Pi Setup**: Install Raspberry Pi OS, enabling SSH and Wi-Fi.
2. **ESP32 Setup**:
   - Install Arduino IDE and add ESP32 board manager URL.
   - Install the ESP32 board via Board Manager.
   - Select your ESP32 board under Tools > Board.
3. **Library Installation**:
   - Install `Bluepad32` for ESP32 in the Arduino IDE.
   - Ensure Python is installed on Raspberry Pi and install necessary libraries for sensor processing and ESP32 communication.

## Wiring

Connect motors, sensors, and the L298 motor driver to the ESP32 following the pin assignments in the code. Ensure correct power supply connections for the ESP32, motors, and sensors.

## Code Overview

The provided code snippet is tailored for the ESP32, facilitating:

- **Controller Connection**: Manages gamepad connections using `Bluepad32`.
- **Motor Control**: Directs motor speed and direction based on gamepad inputs.
- **Sensor Data Processing**: Integration points for sensor data processing are available for customization.

## Usage

1. Upload the code to ESP32 using Arduino IDE.
2. Ensure Raspberry Pi is operational and communicating with ESP32.
3. Connect a gamepad to the ESP32 to control the vehicle.

---
