# Human-Following Robot

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Hardware Components](#hardware-components)
- [Software Requirements](#software-requirements)
- [Wiring Diagram](#wiring-diagram)
- [Installation](#installation)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## Overview

The **Human-Following Robot** is an Arduino-based project designed to autonomously follow a human using a combination of ultrasonic sensors, servo motors, and DC motors. This robot can be used for various applications, including personal assistance, security, and interactive demonstrations.

---

## Features

- **Autonomous Following**: Utilizes ultrasonic sensors to maintain a set distance from the target.
- **Servo-Controlled Scanning**: A servo motor sweeps the ultrasonic sensor to detect the position of the target.
- **Motor Control**: Four DC motors provide smooth and controlled movement.
- **Real-Time Feedback**: Serial monitoring for distance and sensor status.

---

## Hardware Components

- **Arduino Board** (e.g., Arduino Uno)
- **Ultrasonic Sensor** (e.g., HC-SR04)
- **Servo Motor** (e.g., SG90)
- **Adafruit Motor Shield** (v2) or compatible
- **DC Motors** (4 units)
- **Infrared Sensors** or **Line Sensors** (for RIGHT and LEFT detection)
- **Jumper Wires**
- **Power Supply** (appropriate for motors and Arduino)
- **Chassis** (for mounting components)

---

## Software Requirements

- **Arduino IDE** (version 1.8.13 or later)
- **Libraries**:
  - [NewPing](https://bitbucket.org/teckel12/arduino-new-ping/downloads/)
  - [Servo](https://www.arduino.cc/en/Reference/Servo)
  - [AFMotor](https://github.com/adafruit/Adafruit_Motor_Shield_V2_Library) (Adafruit Motor Shield library)

---

## Wiring Diagram

![Wiring Diagram](![Screenshot_20241007-170020_Drive](https://github.com/user-attachments/assets/7d74a0e4-7341-48d0-b5f3-a8930b6c47e0)
)

*Ensure all connections are secure and double-check pin assignments before powering the robot.*

---

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/NandishKoppad09/human-following-robot.git
