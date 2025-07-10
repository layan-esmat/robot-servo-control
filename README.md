# robot-servo-control
# Humanoid Robot Servo Control – Arduino Project

This project demonstrates how to control four servo motors using an Arduino board. The servos perform an initial sweeping motion for two seconds, after which they hold position at 90 degrees. The project serves as a basic framework for developing walking behavior in a humanoid robot.

## Hardware Requirements

- 1x Arduino Uno (or compatible board)
- 4x Servo motors (e.g., SG90 or MG996R)
- External 5V power supply (recommended: 5V 2A or 5V 5A)
- Jumper wires
- Breadboard (optional)

## Wiring Instructions

| Servo Part       | Connects To                        |
|------------------|------------------------------------|
| Signal (Orange)  | Arduino Digital Pins (D9, D10, D11, D12) |
| VCC (Red)        | External 5V Power Supply           |
| GND (Brown/Black)| External GND and Arduino GND       |



## Code Overview

The project uses the `Servo` library to control servo angles. Each servo moves in a sweep from 0 to 180 degrees and back for two seconds. After this period, all servos move to and hold a position of 90 degrees.

### Behavior Summary

- All four servos perform a sweep motion (0–180–0 degrees) for 2 seconds.
- After 2 seconds, all servos are set to 90 degrees and remain there.

The full code is available in the `servo_sweep_and_hold.ino` file.

## Future Improvements

- Add a gyroscope module (e.g., MPU6050) for balance detection.
- Use inverse kinematics for more precise motion.
- Expand to more servos for full leg and arm articulation.

## License

This project is open-source and available under the MIT License.
