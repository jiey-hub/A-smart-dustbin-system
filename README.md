# A-Smart-Dustbin-System
A CPLD-based smart automatic waste bin is designed to enable touchless operation and intelligent waste level monitoring. This system enhances hygiene, user convenience improvement and supports efficient waste management through embedded digital logic control. 
# Key Features
- Touchless lid operation via motion detection
- Automatic closing after a programmable delay
- Real-time overflow detection
- Alert when the bin is full

# Hardware Components
- CLPD - Central control unit
- IR & Ultrasonic Sensor - Detects hand movement and monitors waste level
- Servo Motor - Controls lid movement
- Buzzer - Provides overflow alert

# System Operation
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

# System Architecture
