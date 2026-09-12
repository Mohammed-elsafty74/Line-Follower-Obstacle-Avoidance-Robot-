Line Follower & Obstacle Avoidance Robot

Project Overview

This project presents an autonomous mobile robot that can:

 ● Follow a predefined path (line following)

 ● Detect obstacles and choose the best path to avoid them

The robot uses IR sensors for line detection and ultrasonic sensor for obstacle avoidance, making intelligent decisions to navigate safely.
_______________________________________________________________________________________________________________________________________________
Objectives

● Implement a line follower algorithm using IR sensors

● Implement obstacle detection and avoidance using an ultrasonic sensor

● Use a simple decision-making logic for obstacle avoidance

● Combine both behaviors into a single autonomous system
_______________________________________________________________________________________________________________________________________________
Hardware Components

● Arduino Uno / Nano

● IR Line Sensors

● Ultrasonic Sensor (HC-SR04)

● DC Motors
                            
● Motor Driver (L298N / L293D)

● Wheels & Chassis

● Power Supply (Battery)
__________________________________________________________________________________________________________________________________________
Software & Tools

● Arduino IDE

● Embedded C / C++

● Serial Monitor (for debugging)
__________________________________________________________________________________________________________________________________________
System Functionality

1. Line Following Mode

 ● IR sensors detect the line.

 ● Motors are adjusted to keep the robot following the line.

2. Obstacle Avoidance Mode

 ● Ultrasonic sensor scans left, front, and right.

 ● Robot compares distances:

    ● Moves toward the side with more space.

 ● Returns to line-following mode after avoiding the obstacle.      
__________________________________________________________________________________________________________________________________________
Control Logic

 ● Continuously monitor line and obstacle sensors.

 ● If an obstacle is detected:

    1. Check distance on left and right.

    2. Move to the side with more free space.

    3. Return to the line.

 ● Priority is always obstacle avoidance over line following.
__________________________________________________________________________________________________________________________________________
Demonstration

Video: https://drive.google.com/file/d/10ywGYlCo1AMOZtAOg7_ATJkgfmt0OfiW/view?usp=sharing
__________________________________________________________________________________________________________________________________________
Future Improvements

 ● Implement PID control for smoother line following

 ● Bluetooth/Wi-Fi monitoring

 ● More advanced path planning
__________________________________________________________________________________________________________________________________________
Author

Mohaned Mostafa
Faculty of Computers and Artificial Intelligence
Benha University
__________________________________________________________________________________________________________________________________________
License

MIT License
