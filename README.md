# Self‑Balancing Robot

This project implements a two‑wheeled self‑balancing robot using real‑time embedded
systems, PID control theory, C‑based firmware, and custom hardware integration.

---

## Overview

This robot features a compact three‑tier acrylic chassis, two 65mm diameter wheels, two DC motors with encoders,
and an STM32‑based control board. It uses continuous sensor feedback to adjust motor output and maintain upright balance.

[Robot Front View](03-Photos/robot_front.jpg)
[Chassis Side View](03-Photos/chassis_side.jpg)

### Core Capabilities
- Self‑balanceing using PID control  
- IMU-based real‑time angle estimation  
- Closed‑loop motor control with encoders  
- Modular firmware structure  
- Custom chassis and hardware integration  

[Balancing Demo](04-Videos/balancing_test.mp4)

---

## Repository Map

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
- Encoder feedback via TIM2 and TIM3 in quadrature mode

---

## Setup Instructions

1.  **Wire Components**  
   Follow wiring diagrams in `/03-Photos` and `/07-Drawings`

2. **Flash Firmware**  
   Use ST‑Link to upload the firmware

3. **Power System**  
   C


---

## Future Improvements

- Full LQR implementation    
- Bluetooth remote control  
- 3D‑printed chassis upgrade
- Implemented Encoder Feedback

---