# Smart Dustbin System

## Project Overview
A CPLD-based smart automatic waste bin is designed to enable touchless operation and intelligent waste level monitoring. This system enhances hygiene, user convenience improvement and supports efficient waste management through embedded digital logic control. 
# Key Features
- Touchless lid operation via motion detection
- Automatic closing after a programmable delay
- Real-time overflow detection
- Alert when the bin is full

---

## Hardware Components

- Microcontroller Development Board  
- Ultrasonic Sensor (Distance Measurement)  
- IR Sensor (Overflow Detection)  
- Servo Motor (Lid Control)  
- Buzzer (Audio Alert)  

---

## Pin Configuration

| Pin | Function |
|-----|---------|
| PA0 | Ultrasonic Trigger |
| PA1 | Ultrasonic Echo |
| PA2 | IR Sensor |
| PA3 | Servo Motor |
| PA4 | Buzzer |

---

## System Operation

# Motion-Based Lid Control
- Motion sensor continously monitors for the hand presence.
- When motion detected, a HIGH signal is transmitted to the CPLD.
- The CPLD activates the motor driver to open the lid.
- After a predefined delay, the lid closes automatically.
This mechanism ensures hygienic and touchless waste disposal.
# Overflow Monitoring
- The level sensor continously measures the waste level.
- When the bin reaches the maximum capacity, a HIGH signal is transmitted to the CPLD.
- The CPLD activates the buzzer to alert users.
- The alert will reamin active until the bin is emptied.

---

## Software Description

The system is implemented using embedded C++ with servo motor control and sensor interfacing.

- Main processes:
- Distance measurement (Ultrasonic Sensor)  
- Overflow monitoring (IR Sensor) 
- Position control (Servo Motor) 
- Activation logic (Buzzer)  
- Serial monitoring for debugging  

---

## Initialization

During system startup:
- Lid in closed position initially
- Buzzer is OFF  
- Sensors stabilize before operation begins  

---

## Development Environment

- Embedded C++  
- Arduino-compatible IDE  
- Servo control library  

---

