# Arachne 1.0  
**A Quadruped Surveillance Bot for Challenging Terrains**

Arachne 1.0 is a programmable quadruped robot designed for remote surveillance in rugged environments. With precise servo control and terrain-adaptive movement, it excels in military operations, disaster recovery, and environmental monitoring. This repository contains the Arduino firmware to control its locomotion and functionality.

---

## Key Features
- **Quadruped Arm Design**: Stability on uneven surfaces via 12 servos and adaptive gait sequences.  
- **PWM Servo Control**: Smooth motion using Adafruit PCA9685 driver.  
- **Predefined Gaits**: Efficient walking patterns for climbing, stepping, and obstacle negotiation.  
- **Remote Operation**: Compatible with web/mobile interfaces for real-time control.  
- **Customizable Angles**: Adjust servo positions dynamically for terrain-specific optimization.

---

## Hardware Requirements

| Component            | Specification                                |
|---------------------|----------------------------------------------|
| Microcontroller      | Arduino Uno                          |
| Servo Controller     | Adafruit PCA9685 PWM Driver                  |
| Servos               | 12x Servos          |
| Power                | 7.4V–12V Rechargeable Battery Pack           |
| Chassis              | Custom 3D-printed             |
| Extras               | Jumper Cables, Screws, Zip Ties              |

---

## Setup Instructions

### 1. Hardware Assembly
- Connect servos to PCA9685 driver (refer to pinout diagram in `/docs`).
- Link the power supply to Arduino and PCA9685.
- Secure chassis components: legs → body → electronics bay.

### 2. Software Installation
Install required libraries via Arduino IDE Library Manager:
- `Wire`  
- `Adafruit_PWMServoDriver`

### 3. Clone the repository
Clone the repository:
```bash
git clone https://github.com/SurajKumarKonda/Arachne-1.0/tree/main
```
- Open the Arduino IDE and include `arachne1.cpp` into a new sketch.

## Contributing

Contributions are welcome! Fork the repository and submit pull requests for bug fixes, enhancements, or new features.

---

## License

MIT License – see [LICENSE](LICENSE) for details.

---

**Arachne 1.0**: *Where Robotics Meets Resilience.*
