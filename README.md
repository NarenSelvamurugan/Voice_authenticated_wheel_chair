# Voice-Controlled Wheelchair Using Arduino

## Project Overview

This project aims to implement a smart, voice-controlled wheelchair using Arduino to assist people with both upper and lower limb disabilities. The system is implemented using an Arduino Uno, a Bluetooth module (HC-05) connected to a mobile device through an application, and a motor driver (L298N) to control the direction and speed of DC motors. An Arduino microcontroller processes voice commands from the speech recognition module and controls the motor movement of the wheelchair. The Bluetooth module receives voice commands from the mobile application in the form of strings and transfers them to the Arduino board for further processing. Depending on the input given, the wheelchair can move forward, backward, and in any desired direction. The overall cost of the prototype was kept low to make it affordable.

## Features

- **Voice Control**: Commands like "forward", "backward", "left", "right", "speed", and "stop" control the wheelchair's movement.
- **Obstacle Detection**: An ultrasonic sensor stops the wheelchair if an obstacle is detected within a 20 cm threshold.
- **Light Detection**: A photoresistor activates a buzzer when light levels are low (below a threshold of 100).
- **Affordable Design**: The prototype is designed to be cost-effective for wider accessibility.

## Requirements

- **Motor Driver**: L298N
- **Microcontroller**: Arduino Uno
- **Bluetooth Module**: HC-05
- **Ultrasonic Sensor**: For obstacle detection

## Hardware Setup

1. **Arduino Uno**: The main microcontroller that processes voice commands and controls the motors.
2. **L298N Motor Driver**: Controls the direction and speed of the DC motors for the wheelchair.
3. **HC-05 Bluetooth Module**: Connects to a mobile application to receive voice commands.
4. **Ultrasonic Sensor**: Measures distance to detect obstacles and stop the wheelchair if necessary.
5. **Photoresistor**: Connected to analog pin A0 to detect light levels and activate a buzzer.
6. **Buzzer**: Connected to pin 5, activated when light levels are low.
7. **LED**: Connected to pin 4, lights up when an obstacle is detected.
8. **DC Motors**: Connected to the L298N motor driver for wheelchair movement.

### Pin Configuration

- **Ultrasonic Sensor**:
  - Trigger Pin: 2
  - Echo Pin: 3
- **LED Pin**: 4
- **Buzzer Pin**: 5
- **Motor Driver Pins**:
  - IN1: 9
  - IN2: 8
  - Enable Pin 1: 10
  - IN3: 11
  - IN4: 12
  - Enable Pin 2: 13
- **Photoresistor**: Analog pin A0

**Feel free to add any improvements**
