# 🦾 SO-ARM101 Follower Arm — Desktop Controller

> 6-DOF arm · Feetech STS3215 servos · Click-and-drag GUI over serial

![Status](https://img.shields.io/badge/status-in%20progress-yellow)
![Servos](https://img.shields.io/badge/servos-Feetech%20STS3215-orange)

<!-- TODO: arm photo -> media/hero.jpg -->
<!-- TODO: GUI screen recording -> media/gui-demo.gif -->

## Overview

A SO-ARM101 follower arm (from the LeRobot / TheRobotStudio design) that I assembled myself, plus a desktop app to control it. The app shows the arm on screen. You click and drag a joint, and the app sends the matching commands to the Feetech bus servo controller over serial.

## Hardware

| Part | Detail |
|---|---|
| Arm | SO-ARM101 follower, 3D printed |
| Servos | 6 × Feetech STS3215 |
| Controller | Feetech bus servo controller board (USB serial) |

## Servo IDs

| ID | Joint |
|---|---|
| 1 | Base |
| 2–5 | Shoulder → wrist (bottom to top) |
| 6 | Gripper |

Angle limits are written into each servo's EEPROM as a hardware safety stop.

<!-- TODO: diagram: GUI → serial → controller board → servo bus -> media/control-flow.png -->

## Roadmap

- [x] Assemble arm, set servo IDs and angle limits
- [ ] v1 GUI: drag joints, live servo commands (Windows)
- [ ] Read back servo positions
- [ ] LeRobot calibration and leader–follower teleoperation

## Author

**Jasin Jesin** · [LinkedIn](https://www.linkedin.com/in/jasinjesin/)
