
# Intelligent Braking System for Electric Vehicles (EV)

## Overview

The Intelligent Braking System is a simple obstacle detection and speed control system designed for electric vehicles. The system uses an ultrasonic sensor to measure the distance between the vehicle and an obstacle. Based on the measured distance, the motor speed is automatically adjusted to reduce the risk of collision.

This project demonstrates the basic concept of Advanced Driver Assistance Systems (ADAS) and automatic braking used in modern vehicles.

## Features

* Real-time obstacle detection
* Automatic motor speed adjustment
* Gradual braking based on obstacle distance
* Complete stop when an obstacle is too close
* Low-cost and easy-to-build prototype

## Components Used

* Arduino Nano
* HC-SR04 Ultrasonic Sensor
* L298N Motor Driver Module
* 2 DC Motors
* Battery Supply
* Jumper Wires
* Chassis (Optional)

## Working Principle

1. The ultrasonic sensor continuously measures the distance to nearby obstacles.
2. The Arduino processes the distance data.
3. Based on the detected distance:

   * Distance > 50 cm → Full Speed
   * Distance 30–50 cm → Medium Speed
   * Distance 15–30 cm → Low Speed
   * Distance < 15 cm → Motor Stop
4. The motor driver receives PWM signals from the Arduino and controls the motor speed accordingly.

## Pin Connections

### Ultrasonic Sensor

| HC-SR04 | Arduino Nano |
| ------- | ------------ |
| VCC     | 5V           |
| GND     | GND          |
| TRIG    | D9           |
| ECHO    | D10          |

### Motor Driver

| L298N | Arduino Nano |
| ----- | ------------ |
| ENA   | D5           |
| IN1   | D2           |
| IN2   | D3           |
| ENB   | D6           |
| IN3   | D4           |
| IN4   | D7           |

### Motors

* Motor A → OUT1 and OUT2
* Motor B → OUT3 and OUT4

## Applications

* Electric Vehicles
* Collision Avoidance Systems
* Autonomous Robot Cars
* Smart Transportation Systems
* Driver Assistance Systems

## Future Improvements

* Dynamic braking using proportional control
* Multiple ultrasonic sensors
* Emergency buzzer alert
* LCD/OLED distance display
* Bluetooth monitoring
* Integration with regenerative braking systems

## Outcome

The project successfully demonstrates automatic speed control and obstacle-based braking using an Arduino Nano, ultrasonic sensor, and motor driver. The system reduces vehicle speed as obstacles get closer and stops the vehicle when a critical distance is reached.

## Author

PATHANGI SHIVAJI RAO

EMBEDDED SYSTEMS | VLSI | FPGA | MATLAB AND SIMULINK | Intelligent Braking System for Electric Vehicles (EV) |
