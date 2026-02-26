# A-smart-dustbin-system
An automated smart dustbin design with motion detection and overflow alret

🗑️ CPLD-Based Smart Automatic Waste Bin

📌 Project Overview

This project implements a CPLD-based automatic smart waste bin system designed to provide touchless operation and intelligent overflow monitoring.

The system uses motion detection and level sensing to automatically control the bin lid and alert users when the bin is full.

The system provides:

Automatic lid opening using motion detection

Automatic lid closing after a preset delay

Overflow detection using level sensor

Audio alert using buzzer when bin is full


⚙️ Hardware Components

CPLD (Complex Programmable Logic Device)

IR / Ultrasonic Motion Sensor (Hand detection)

Ultrasonic / Level Sensor (Overflow detection)

Servo Motor / DC Motor (Lid control)

Motor Driver Module

Buzzer (Overflow alert)


🧠 System Operation

🖐️ Hand Motion Detection

The motion sensor continuously monitors for hand presence.

When a hand is detected, a HIGH signal is sent to the CPLD.

The CPLD activates the motor driver.

The lid opens automatically.

After a preset delay (using counter/timer logic), the lid closes automatically.

This ensures a touchless and hygienic disposal process.

🚮 Overflow Detection

The level sensor continuously monitors the waste level inside the bin.

When the bin reaches maximum capacity, the sensor sends a HIGH signal.

The CPLD activates the buzzer.

The buzzer remains ON until the bin is emptied or reset.

This prevents overflow and improves waste management efficiency.


🗂️ Software / Logic Description

The system is developed using:

Verilog HDL

Quartus Design Software

Main logic blocks:

Input signal processing

Finite State Machine (FSM) for lid control

Counter module for timing delay

Comparator logic for overflow detection

Output control logic for motor and buzzer


⏱️ Initialization

Upon power-up:

The lid remains closed

The buzzer is OFF

Sensors stabilize before normal operation begins


🧪 Development Environment

Quartus Prime

Verilog HDL

CPLD Development Board


👩‍💻 Author

Yap Boon Jie

Electronic Engineering Student

Universiti Teknologi Malaysia

