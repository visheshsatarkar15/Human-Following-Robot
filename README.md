# Human Following Robot

An Arduino-based robot that follows a person by using ultrasonic distance sensing and side sensors for direction correction. The robot detects a human or nearby object in front of it, keeps a safe following distance, and adjusts left or right when the target moves.

## Project Overview

This project demonstrates the basic working principle of a human-following robot using simple and affordable components. It is useful for learning robotics, embedded systems, motor control, obstacle sensing, and Arduino programming.

## Features

- Follows a person or object automatically
- Maintains a safe distance from the target
- Turns left or right based on side sensor input
- Stops when the target is too close or too far
- Uses commonly available Arduino components
- Beginner-friendly circuit and code

## Demo

Video - <video controls src="Demo Video.mp4" title="Title"></video>

## Components Required

Component - Quantity -> Purpose


1] Arduino Uno -- 1 --> Main controller 
2] L298N motor driver shield -- 1 --> Controls DC motors 
3] DC geared motors -- 4 --> Robot movement 
4] Robot chassis -- 1 --> Mechanical frame 
5] HC-SR04 ultrasonic sensor -- 1 --> Measures front distance 
6] IR sensors -- 2 --> Detects left/right target movement 
7] Battery pack -- 1 --> Robot power supply 
8] Jumper wires -- As needed --> Connections 
9] Wheels -- 4 --> Movement 
10] Switch -- 1 --> Power control 

## Working Principle

The robot uses an ultrasonic sensor to measure the distance between itself and the person in front of it.

- If the person is within the follow range, the robot moves forward.
- If the person is too close, the robot stops.
- If the person moves left, the left IR sensor helps the robot turn left.
- If the person moves right, the right IR sensor helps the robot turn right.
- If no person or object is detected in range, the robot stops.

## Circuit Connections

Circuit Diagram - ![alt text](<Circuit Diagram.jpeg>)

## How to Build

1. Assemble the robot chassis with motors and wheels.
2. Mount the ultrasonic sensor at the front of the robot.
3. Mount the left and right IR sensors on the front-left and front-right sides.
4. Connect the motor driver to the Arduino.
5. Connect the sensors according to the wiring table.
6. Upload the Arduino code.
7. Power the robot and test it in an open area.
8. Adjust the distance and speed values in the code if needed.

## Arduino Code

The main Arduino sketch is available here:

[text](<../../../../../../../../PROJECTS/HUMAN FOLLOWING ROBOT/Arduinocode.ino.txt>)



Increase or decrease these values based on your robot's motor speed, battery voltage, and sensor placement.


## Calibration Tips

- Keep the ultrasonic sensor straight and stable.
- Test the robot at low speed first.
- If the robot moves backward instead of forward, swap the motor wires or change motor direction logic in the code.
- If the robot turns the wrong way, swap left and right motor control logic.
- Use fresh batteries because weak batteries can cause unstable motor behavior.


## Future Improvements

- Add camera-based human detection
- Use Bluetooth or Wi-Fi control
- Add obstacle avoidance
- Add speed control using PWM
- Use PID control for smoother following
- Add a rechargeable battery system
- Design a custom PCB

## Applications

- Learning robotics
- Arduino projects
- College mini project
- Automation prototype
- Assistive carrying robot concept


## Author

Created by Vishesh Satarkar.
GitHub Handle - visheshsatarkar15
