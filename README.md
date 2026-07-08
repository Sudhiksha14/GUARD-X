# 🚗 Guard-X – Vehicle-to-Vehicle Early Collision Detection System

## 📖 Introduction

**Guard-X** is an embedded Vehicle-to-Vehicle (V2V) collision prevention system developed to improve road safety by enabling nearby vehicles to exchange critical driving information in real time.

The system combines **STM32-based embedded controllers**, **ESP-NOW wireless communication**, **ultrasonic distance sensing**, and **IoT monitoring** to detect potential collision scenarios and provide immediate warnings to the driver. By continuously monitoring the surrounding environment and sharing telemetry data between vehicles, Guard-X helps reduce the risk of accidents caused by delayed driver response.

---

# 🚀 Project Highlights

- Embedded firmware developed using **STM32F103C8T6**
- Vehicle-to-Vehicle communication through **ESP-NOW**
- Real-time obstacle detection using **HC-SR04**
- Velocity estimation using **MPU6050**
- Remote monitoring and control using **Blynk IoT**
- Audio and visual collision warning system

---

# 🏗 System Architecture

The system architecture consists of multiple embedded nodes capable of exchanging telemetry information wirelessly. Each node measures its own motion parameters and obstacle distance while broadcasting this information to nearby Guard-X units for collision analysis.

---

# 🔌 Hardware Choice

| Hardware | Purpose |
|-----------|---------|
| STM32F103C8T6 | Main Processing Unit |
| ESP-01 (ESP8266) | ESP-NOW & Wi-Fi Communication |
| HC-SR04 | Distance Measurement |
| MPU6050 | Motion and Velocity Estimation |
| L298N | Motor Driver |
| DC Gear Motors | Vehicle Movement |
| LED | Visual Warning |
| Buzzer | Audible Alert |
| Battery Pack | System Power Supply |

---

# ✨ Key Features

### 🚗 Vehicle-to-Vehicle Communication

Nearby Guard-X units exchange real-time telemetry information using ESP-NOW, allowing vehicles to remain aware of surrounding traffic conditions without requiring internet connectivity.

---

### 📏 Obstacle Detection

The HC-SR04 ultrasonic sensor continuously measures the distance between the vehicle and nearby obstacles. Unsafe proximity immediately triggers warning signals.

---

### 📡 Wireless Telemetry Sharing

Vehicle speed, obstacle distance, and system status are periodically transmitted to neighboring Guard-X modules to improve situational awareness.

---

### 📱 IoT Dashboard

The system integrates with the Blynk IoT platform, allowing users to monitor telemetry data and remotely observe the operational status of the vehicle.

---

# ⚙️ Working Principle

```
Obstacle Detection
        │
        ▼
 HC-SR04 Measures Distance
        │
        ▼
 MPU6050 Estimates Motion
        │
        ▼
 STM32 Processes Sensor Data
        │
        ▼
 ESP-NOW Broadcasts Vehicle Status
        │
        ▼
 Nearby Vehicle Receives Data
        │
        ▼
 Collision Risk Evaluation
        │
        ▼
 LED + Buzzer Warning
        │
        ▼
 Blynk Dashboard Update
```

---

# 📈 Future Enhancements

- GPS-assisted vehicle localization
- CAN Bus integration
- Automatic emergency braking
- Camera-assisted object detection
- Machine Learning based collision prediction
- V2X communication support
- Mobile application for fleet monitoring

---
