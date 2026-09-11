# Self‑Balancing Robot

This project implements a two‑wheeled self‑balancing robot using real‑time embedded
systems, PID control theory, C‑based firmware, and custom hardware integration.

---

## Overview

This robot features a compact three‑tier acrylic chassis, two 65mm diameter wheels, two DC motors with encoders,
and an STM32‑based control board. It uses continuous sensor feedback to adjust motor output and maintain upright balance.

---

[Robot Front View](Photos/Robot_Front_View.jpeg)

---

[Robot Right Side View](Photos/Robot_Right_Side_View.jpeg)

---

[Robot Left Side View](Photos/Robot_Left_Side_View.jpeg)

---

### Core Capabilities
- Self‑balanceing using PID control  
- IMU-based real‑time angle estimation  
- Modular firmware structure  
- Custom chassis and hardware integration  

[Balancing Demo](Videos/Robot_Balancing_Test.mp4)

---

## Hardware Overview

- Acrylic sheets made into 3-tier chasis
- Two 65mm Diameter Rubber Wheels with 6mm Clamping
- XT60 Connectors
- 22 AWG Wire
- VHB Double Sided Foam Tape
- M3 Standoff Spacers and Screws
- Two Metal DC Motors with Encoders
- STM32F103C8T6 Blue Pill Microcontroller  
- TB6612FNG DC Dual H-Bridge Motor Driver
- MPU6050 IMU 
- HC-05 Bluetooth Connector
- I2C Serial OLED Display
- ST-Link
- Mini Rocker Switch
- 12V to 5V Buck Converter

---

## Control System Architecture

- Complementary filter for angle estimation  
- PID controller for balancing 
- 1 kHz control loop  
- PWM generation on pins PB8 & PB9 using TIM4

---

## Future Improvements

- Full LQR implementation    
- Bluetooth remote control  
- 3D‑printed chassis upgrade
- Implement Encoder Feedback

---