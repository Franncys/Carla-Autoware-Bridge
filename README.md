<div align="center">

# CARLA-Autoware-Bridge - Enables the use of CARLA for Testing and Development of Autoware Core/Universe
[![Linux](https://img.shields.io/badge/os-ubuntu22.04-blue.svg)](https://www.linux.org/)
[![Docker](https://badgen.net/badge/icon/docker?icon=docker&label)](https://www.docker.com/)
[![ROS2humble](https://img.shields.io/badge/ros2-humble-blue.svg)](https://docs.ros.org/en/humble/index.html)

</div>

## Introduction
The CARLA-Autoware-Bridge is a package to connect the CARLA simulator to Autoware Core/Universe with the help of the CARLA-ROS-Bridge.

## Overview
The simulation framework around the CARLA-Autoware-Bridge consists of the components:
- carla-autoware-bridge: This repository holding the CARLA-Autoware-Bridge.
- ros-bridge: Fork of the ros-bridge with our changes needed for the CARLA-Autoware-Bridge.
- carla-t2: Vehicle model and sensor kit packages of the CARLA T2 2021 Vehicle for Autoware.
- carla-ros-msgs:  Fork of the carla-ros-msg with our changes needed for the CARLA-Autoware-Bridge.
This repository is a **forked and updated version** of the original CARLA-Autoware-Bridge by TUMFTM:  
➡️ **https://github.com/TUMFTM/carla-autoware-bridge**

The following changes have been made in this fork:

### ✔️ New Features
1. **Sensor Logging**:
   - Added logging functionality for all vehicle sensors (e.g., camera, LiDAR, radar, etc.).
   - Logs are stored in a structured format, enabling easier analysis of sensor data for testing and debugging.

2. **Sensor Fault Injection**:
   - Introduced a new fault injection mechanism to simulate sensor malfunctions.
   - Allows for testing the resilience of the Autoware system under faulty sensor conditions (e.g., missing LiDAR data, noisy camera input, etc.).

3. **Communication with CARLA Scenario Runner**:
   - Integrated communication with a **forked version of CARLA Scenario Runner**.
   - Enables automated scenario execution for testing the system in various driving conditions and traffic situations.
   - This feature allows you to trigger and manage predefined driving scenarios directly from the CARLA-Autoware-Bridge.

---

This version focuses on enhancing the testing capabilities and integrating with the CARLA Scenario Runner for more complex and automated simulations.

## 🛠️ Installation Process
Follow the original installation instructions from the CARLA-Autoware-Bridge repository, with the only difference being that you will use **this updated version of the bridge** instead of the original one.
