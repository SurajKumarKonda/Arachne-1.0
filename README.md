# Arachne-1.0

A Quadruped Surveillance Bot for Challenging Terrains

Arachne 1.0 is a programmable quadruped robot designed for remote surveillance in rugged environments. With precise servo control and terrain-adaptive movement, it excels in military operations, disaster recovery, and environmental monitoring. This repository contains the Arduino firmware to control its locomotion and functionality.

Key Features
Quadruped Arm Design : Stability on uneven surfaces via 12 servos and adaptive gait sequences.
PWM Servo Control : Smooth motion using Adafruit PCA9685 driver.
Predefined Gaits : Efficient walking patterns for climbing, stepping, and obstacle negotiation.
Remote Operation : Compatible with web/mobile interfaces for real-time control.
Customizable Angles : Adjust servo positions dynamically for terrain-specific optimization.
Hardware Requirements
COMPONENT
SPECIFICATION
Microcontroller
Arduino Uno / Clone
Servo Controller
Adafruit PCA9685 PWM Driver
Servos
12x Digital/Analog Micro/Mid-Servos
Power
7.4V–12V Rechargeable Battery Pack
Chassis
Custom-built (Acrylic/Aluminum)
Extras
Jumper Cables, Screws, Zip Ties

Setup Instructions
1. Hardware Assembly
Connect servos to PCA9685 driver (refer to pinout diagram in /docs).
Link power supply to Arduino and PCA9685.
Secure chassis components: legs → body → electronics bay.
2. Software Installation
Install required libraries via Arduino IDE Library Manager:

Wire
Adafruit_PWMServoDriver
Clone the repository:

bash


1
git clone https://github.com/yourname/Arachne-1.0
Open Arachne_1_0.ino in Arduino IDE and upload to your board.

3. Calibrate Servo Angles
Modify setServoAngle() values in functions like leg1(), leg2(), or stance() for terrain-specific adjustments. Example:

cpp


1
2
void leg1Angles[] = {45, 60, 90}; // Customize angles for leg 1
void leg2Angles[] = {30, 75, 120}; // Customize angles for leg 2
Code Overview
Main Logic : The loop() function manages synchronized leg movements.
Gestures : Functions like hello() (wave) and stance() (posture reset) enable custom motions.
Expandability : Integrate sensors (ultrasonic, IMU) or ML models for autonomy.
Use Cases
Military Reconnaissance : Stealthy operations in hostile zones.
Disaster Response : Navigate debris to locate survivors.
Environmental Monitoring : Deploy in forests, deserts, or wetlands.
Contributing
Contributions are welcome! Fork the repository and submit pull requests for bug fixes, enhancements, or new features.

License
MIT License – see LICENSE for details.

Star ⭐ this repo to stay updated on improvements and community builds.

Arachne 1.0: Where Robotics Meets Resilience.
