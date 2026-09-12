# 🤖 Line Follower & Obstacle Avoidance Robot

> An autonomous mobile robot that follows a predefined path using IR sensors and intelligently avoids obstacles using an ultrasonic sensor — combining both behaviors into one smart navigation system.

<p align="center">
  <img src="https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white"/>
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white"/>
  <img src="https://img.shields.io/badge/Embedded%20Systems-Robotics-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge"/>
</p>

---

## 🎥 Demo

> 📹 **Watch the robot in action:** [Demonstration Video](https://drive.google.com/file/d/10ywGYlCo1AMOZtAOg7_ATJkgfmt0OfiW/view?usp=sharing)

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Hardware Components](#hardware-components)
- [Software & Tools](#software--tools)
- [System Functionality](#system-functionality)
- [Control Logic](#control-logic)
- [Demonstration](#demonstration)
- [Future Improvements](#future-improvements)
- [Author](#author)
- [License](#license)

---

## 🔍 Project Overview

This project presents an autonomous mobile robot that can:

| Behavior | Description |
|----------|--------------|
| 🛣️ **Line Following** | Follows a predefined path using IR sensors |
| 🚧 **Obstacle Avoidance** | Detects obstacles and chooses the best path around them |

The robot uses **IR sensors** for line detection and an **ultrasonic sensor** for obstacle avoidance, making intelligent decisions to navigate safely.

---

## 🎯 Objectives

- Implement a line follower algorithm using IR sensors
- Implement obstacle detection and avoidance using an ultrasonic sensor
- Use simple decision-making logic for obstacle avoidance
- Combine both behaviors into a single autonomous system

---

## 🔧 Hardware Components

| # | Component |
|---|-----------|
| 1 | Arduino Uno / Nano |
| 2 | IR Line Sensors |
| 3 | Ultrasonic Sensor (HC-SR04) |
| 4 | DC Motors |
| 5 | Motor Driver (L298N / L293D) |
| 6 | Wheels & Chassis |
| 7 | Power Supply (Battery) |

---

## 💻 Software & Tools

| Tool | Purpose |
|------|---------|
| Arduino IDE | Writing & uploading firmware |
| Embedded C / C++ | Robot control logic |
| Serial Monitor | Debugging & sensor readings |

---

## ⚙️ System Functionality

### 1️⃣ Line Following Mode
- IR sensors detect the line
- Motors are adjusted to keep the robot following the line

### 2️⃣ Obstacle Avoidance Mode
- Ultrasonic sensor scans left, front, and right
- Robot compares distances and moves toward the side with more space
- Returns to line-following mode after avoiding the obstacle

---

## 🧠 Control Logic

```
[Continuously Monitor Sensors]
              |
              ▼
     [Obstacle Detected?]
        |            |
       Yes           No
        |            |
        ▼            ▼
[Check Left/Right]  [Continue Line Following]
        |
        ▼
[Move to Side with More Space]
        |
        ▼
   [Return to Line]
```

> ⚠️ **Priority is always obstacle avoidance over line following.**

---

## 🎥 Demonstration

Video:https://drive.google.com/file/d/1Y0n1nug40EUx6uDFXX24p9ueUT-0-j3y/view?usp=sharing 

---

## 🚀 Future Improvements

- Implement **PID control** for smoother line following
- Add **Bluetooth/Wi-Fi monitoring**
- Develop more advanced **path planning**

---

## 👤 Author

- **Name:** Mohammed Elsafty
- **Faculty:** Faculty of Computers and Artificial Intelligence

---

