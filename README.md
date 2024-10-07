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

(![robo-wiring](https://github.com/user-attachments/assets/17daeea6-137d-4927-a328-b1e7fe1b75c7)



*Ensure all connections are secure and double-check pin assignments before powering the robot.*

---


## Installation

### 1. Open the Project
- **Launch the Arduino IDE**.
- **Open the `.ino` file** from the cloned repository by navigating to **File** > **Open** and selecting the appropriate `.ino` file.

### 2. Install Required Libraries
Ensure the following libraries are installed:

- **NewPing**
- **Servo**
- **Adafruit Motor Shield V2**

To install these libraries:

- Go to **Sketch** > **Include Library** > **Manage Libraries**.
- In the Library Manager, search for each library by name and click **Install**.

### 3. Connect Hardware
- **Assemble the robot chassis**.
- Connect the **ultrasonic sensor**, **servo motor**, and **DC motors** to the Arduino and Motor Shield according to the wiring diagram provided in this repository.

### 4. Upload the Code
- In the Arduino IDE, select the correct **Board** and **Port** from the **Tools** menu.
  - For example, if you're using an Arduino Uno, go to **Tools** > **Board** > **Arduino Uno**.
  - Then select the correct **Port** (e.g., **COM3** or similar, depending on your system).
- Once everything is connected, click the **Upload** button (right arrow icon) in the Arduino IDE to upload the code to the board.

---

## Usage

### 1. Power On
- Ensure the robot is connected to a stable power source.
- You can power it using batteries or a USB connection to the Arduino, depending on your setup.

### 2. Initialization
- Upon powering the robot, the **servo motor** will perform a sweep to calibrate the ultrasonic sensor.
- This helps the robot "scan" the surroundings and detect the initial position of the human target.

### 3. Operation
- The robot will autonomously start following the human target after calibration.
- It maintains an optimal distance using the **ultrasonic sensor** to avoid obstacles.

### 4. Monitoring
- Open the **Serial Monitor** in the Arduino IDE (press **Ctrl + Shift + M** or navigate to **Tools** > **Serial Monitor**).
- Set the baud rate to **9600** to view real-time data, including:
  - **Distance** measured by the ultrasonic sensor.
  - Status of the **RIGHT** and **LEFT** sensors.
  
You can use this information to debug and ensure the robot is following the target correctly.

**Clone the Repository**
   ```bash
   git clone https://github.com/NandishKoppad09/human-following-robot.git
