# Car-Black-Box

# Overview
The Car Black Box project is an automotive event logging system developed using the PIC18F4580 microcontroller. It continuously monitors vehicle parameters such as speed, gear position, and time, and stores critical events in External EEPROM. The system allows users to view recorded logs on a CLCD display or transfer them through UART communication for further analysis.

# Features
1.Real-time monitoring of vehicle speed and gear position
2.Time stamping using RTC (DS1307)
3.Event logging in External EEPROM
4.CLCD-based user interface
5.UART communication for log download
6.7.Menu-driven navigation using Digital Keypad
Secure storage and retrieval of event records

# Technologies Used
1.Embedded C
2.PIC18F4580 Microcontroller
3.I2C Protocol
4.RTC (DS1307)
5.External EEPROM
6.UART Communication
7.CLCD Display
8.ADC
9.Timers and Interrupts
10.Digital Keypad

# Hardware Requirements
1.PIC18F4580 Microcontroller
2.DS1307 RTC Module
3.External EEPROM (24Cxx Series)
4.CLCD Display (16x2)
5.Potentiometer (Speed Simulation)
6.Digital Keypad / Push Buttons
7.UART Interface
8.Crystal Oscillator
9.Power Supply Circuit

# Software Requirements
1.MPLAB X IDE
2.XC8 Compiler
3.Embedded C

# Working Principle
1.Vehicle speed is monitored using ADC input.
2.Gear changes are detected through keypad switches.
3.RTC provides the current date and time.
4.Important events are recorded along with speed, gear, and timestamp.
5.Event logs are stored in External EEPROM through I2C communication.
6.Stored logs can be viewed on the CLCD or transmitted via UART.

Event Log Format
Time       Event     Speed
10:30:15   GR        25
10:31:20   G1        30
10:32:10   G2        45
10:33:05   C_ON      50

# Project Structure
CAR_BLACK_BOX/
│
├── main.c
├── adc.c
├── adc.h
├── clcd.c
├── clcd.h
├── ds1307.c
├── ds1307.h
├── external_eeprom.c
├── external_eeprom.h
├── i2c.c
├── i2c.h
├── uart.c
├── uart.h
├── matrix_keypad.c
├── matrix_keypad.h
├── timers.c
├── timers.h
└── README.md

# Key Challenges & Learnings
1.Challenges Faced
2.Managing EEPROM memory efficiently
3.Storing and retrieving event logs reliably
4.Synchronizing RTC time with event recording
5.Implementing menu-driven navigation
6.Handling UART data transmission
# Learnings
1.Real-time data logging techniques
2.I2C communication with RTC and EEPROM
3.Embedded memory management
4.UART communication protocols
5.Automotive event monitoring concepts

# Applications
1.Automotive Black Box Systems
2.Vehicle Event Monitoring
3.Driver Behavior Analysis
4.Accident Investigation Systems
5.Fleet Management Solutions

# Future Enhancements
1.GPS location tracking
2.SD Card storage
3.Wireless log transmission
4.Cloud-based monitoring
5.Accident detection using sensors

# Conclusion
The Car Black Box project demonstrates real-time vehicle event monitoring and logging using the PIC18F4580 microcontroller. By integrating RTC, EEPROM, UART, and CLCD modules, the system provides an efficient solution for recording and reviewing vehicle events, making it a practical embedded systems project for automotive applications.
