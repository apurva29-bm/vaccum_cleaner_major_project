# 🤖 Smart Robotic Vacuum Cleaning System with Wireless Control and Live Video Monitoring

An intelligent, solar-assisted robotic vacuum cleaning system developed using **Arduino Nano, Seeed Studio XIAO ESP32S3 Sense, and an Android application**. The system enables wireless robot movement, automated vacuum operation, live video monitoring, and AI-based object/dust detection through a smartphone.

---

## 📌 Project Overview

The Smart Robotic Vacuum Cleaning System is designed to provide an efficient and intelligent cleaning solution with wireless control and real-time visual monitoring.

The robot uses an Arduino Nano for movement control and vacuum motor operation, while the Seeed Studio XIAO ESP32S3 Sense handles live camera streaming. An Android application provides wireless control, video monitoring, and image detection capabilities.

The system also incorporates a solar-assisted power arrangement using a 6V solar panel and a 3-cell lithium-ion battery system.

## ✨ Key Features

- 📱 **Android Application Control:** Control robot movement and vacuum operation through a custom-built Android application.
- 🎥 **Live Video Monitoring:** Real-time camera streaming using Seeed Studio XIAO ESP32S3 Sense.
- 🔍 **AI-Based Detection:** Detect dust and objects through the Android application.
- 🚗 **Wireless Robot Navigation:** Bluetooth-based movement control using HC-05.
- 🧹 **Automated Vacuum Operation:** Control the vacuum cleaner through an integrated relay module.
- ☀️ **Solar-Assisted Power:** Solar energy integration with a 3-cell lithium-ion battery system.
- ⚡ **Dual-Controller Architecture:** Separate controllers for robot movement and camera monitoring.

## 🏗️ System Architecture

The system uses two independent microcontrollers to distribute the processing responsibilities.

### 1. Robot Movement and Vacuum Control

**Arduino Nano** manages:
- Bluetooth communication through HC-05.
- Forward, backward, left, and right movement.
- DC motor control through the L298N motor driver.
- Vacuum cleaner ON/OFF operation through a relay module.

### 2. Camera and Detection System

**Seeed Studio XIAO ESP32S3 Sense** manages:
- Live camera capture.
- Wireless video streaming.
- Camera-based visual monitoring.
- Communication with the Android application for video access.

### 3. Android Application

The custom Android application provides:
- Wireless movement commands.
- Vacuum cleaner control.
- Live camera feed.
- Image-based object and dust detection.
- Detection results and visual indicators.

## 🔌 Hardware Components

| Component | Purpose |
|---|---|
| Arduino Nano | Robot movement and vacuum control |
| Seeed Studio XIAO ESP32S3 Sense | Camera streaming |
| HC-05 Bluetooth Module | Wireless communication |
| L298N Motor Driver | DC motor control |
| BO Geared DC Motors (4) | Robot movement |
| Relay Module | Vacuum cleaner switching |
| Vacuum Cleaner | Cleaning operation |
| OV3660 Camera | Live video monitoring |
| 6V, 5W Solar Panel (1) | Solar energy input |
| Blue Boost Converter | Solar voltage conversion |
| XL4015 CC/CV Module | Voltage and current regulation |
| 3S BMS | Battery protection |
| 3 Lithium-ion Cells | Battery storage |
| Robot Chassis | Mechanical structure |

## ⚙️ Solar-Assisted Power System

The project incorporates a solar-assisted battery arrangement.

**Power Conversion Flow:**

1. A single 6V, 5W solar panel captures solar energy.
2. The solar output is connected to a boost converter.
3. The boosted voltage is regulated using an XL4015 CC/CV module.
4. The regulated output is intended for the 3S lithium-ion battery charging arrangement.
5. A 3S BMS provides battery protection.
6. The battery pack supplies power to the robotic system.

**Power System:**

`6V Solar Panel → Blue Boost Converter → XL4015 CC/CV → 3S BMS → 3-Cell Li-ion Battery Pack`

*Note: The charging circuit must be configured with a suitable 3S lithium-ion CC/CV charging profile and appropriate input/output ratings. The BMS is a protection circuit, not a substitute for a proper charger.*

## 💻 Software Requirements

| Software / Platform | Application |
|---|---|
| Arduino IDE | Arduino Nano programming |
| Embedded C / C++ | Microcontroller programming |
| Android Application | Robot control and detection |
| ESP32 Camera Firmware | Live video streaming |
| Bluetooth Communication | Wireless robot commands |

## 🔄 Working Methodology

1. **System Initialization:** The robot and camera controller are powered on.
2. **Wireless Connection:** The Android application establishes Bluetooth communication with the HC-05 module.
3. **Movement Control:** Commands are sent to the Arduino Nano to control the four DC motors.
4. **Vacuum Operation:** The application sends ON/OFF commands to operate the vacuum through the relay.
5. **Live Monitoring:** The XIAO ESP32S3 Sense captures video and provides a wireless camera stream.
6. **Visual Detection:** The Android application processes the visual input to identify dust and objects.
7. **Solar-Assisted Power:** The solar arrangement supports the battery charging system.

## 🧠 Technologies Used

- Embedded Systems
- Internet of Things (IoT)
- Arduino Programming
- ESP32 Camera Streaming
- Bluetooth Communication
- Android Application Development
- Image Processing and Object Detection
- Solar Energy Integration
- DC Motor Control

## 🎯 Applications

- Smart home cleaning systems.
- Automated floor-cleaning applications.
- Educational robotics projects.
- IoT-based automation systems.
- Embedded systems and computer vision research.

## 🚀 Future Enhancements

- Autonomous navigation using advanced sensors.
- Obstacle avoidance and intelligent path planning.
- Automatic battery monitoring.
- Improved dust classification and detection.
- Cloud-based monitoring and control.
- Automatic docking and charging.

## 👨‍💻 Project Information

**Project Title:** Smart Robotic Vacuum Cleaning System with Wireless Control and Live Video Monitoring

**Department:** Electronics and Communication Engineering

**Institution:** Jawaharlal Nehru New College of Engineering (JNNCE), Shivamogga

**Project Type:** Academic Major Project

## 📜 License

This project is intended for educational and research purposes. You may modify and improve the implementation with appropriate attribution.

---

⭐ If you find this project interesting, consider giving this repository a star!
