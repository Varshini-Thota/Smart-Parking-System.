# Smart Parking System

## Overview

The Smart Parking System is an Arduino-based project that detects vehicle presence using an HC-SR04 Ultrasonic Sensor. The system indicates parking slot availability through LEDs.

## Features

* Vehicle detection using Ultrasonic Sensor
* Green LED indicates parking slot available
* Red LED indicates parking slot occupied
* Real-time distance measurement
* Simple and cost-effective design

## Components Used

* Arduino Uno
* HC-SR04 Ultrasonic Sensor
* Green LED
* Red LED
* 220Ω Resistors
* Jumper Wires

## Circuit Connections

### HC-SR04 Sensor

* VCC → 5V
* GND → GND
* TRIG → Digital Pin 9
* ECHO → Digital Pin 10

### Green LED

* Anode (+) → Digital Pin 2
* Cathode (-) → 220Ω Resistor → GND

### Red LED

* Anode (+) → Digital Pin 3
* Cathode (-) → 220Ω Resistor → GND

## Working Principle

1. The ultrasonic sensor continuously measures the distance in front of it.
2. If the measured distance is greater than 20 cm, the parking slot is considered available and the Green LED turns ON.
3. If the measured distance is less than 20 cm, a vehicle is detected and the Red LED turns ON.
4. Distance values are displayed through the Serial Monitor.

## Output

* Distance > 20 cm → Green LED ON (Parking Available)
* Distance < 20 cm → Red LED ON (Parking Occupied)

## Applications

* Smart Parking Management
* Vehicle Detection Systems
* Automated Parking Guidance
* IoT-Based Parking Solutions

## Future Improvements

* Multiple Parking Slot Monitoring
* LCD Display Integration
* Mobile App Notification
* Cloud-Based Parking Management
