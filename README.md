# Drone Pilot

**Autonomous pilot software for companion computers — MultiWii, Pixhawk, PX4 (2014)**

> Part of Daniel Dieser's robotics and drone research period (2012-2014) in Puerto Madryn, Patagonia.

---

## What Is This?

Drone Pilot is an autonomous flight control system that runs on companion computers (Raspberry Pi, laptops) alongside flight controllers. It bridges the gap between manual RC control and fully autonomous flight through **PID-based position controllers, neural network experiments, and computer vision**.

This project was a critical piece in Daniel's journey: it combined **hardware control, real-time algorithms, computer vision, and early neural network experiments** — all running on a drone in the physical world.

## Features

- **MultiWii Serial Protocol** — Direct communication with MultiWii flight controllers
- **Pixhawk/PX4 Support** — DroneKit integration for advanced missions
- **Hover Controller** — PID-based position hold using motion capture feedback
- **Height Controller** — Altitude hold with sonar/barometer data
- **Neural Network Controller** — Experimental flight control using trained neural nets
- **Joystick Control** — UDP bridge from ground station (Matlab/Python) to flight controller
- **Waypoint Navigation** — Autonomous multi-point flight paths
- **Computer Vision** — OpenCV color tracking for visual navigation
- **Flight Data Logger** — Black box recording of all flight parameters

## Scripts

| Script | Description |
|--------|-------------|
|  | PID position hold — the core autonomous flight algorithm |
|  | Altitude hold controller |
|  | **Neural network flight controller** — experimental ML for flight |
|  | UDP joystick commands from ground station to MultiWii |
|  | Autonomous waypoint navigation |
|  | Flight data recording (IMU, RC, attitude) |
|  | Simulink integration for control design |
|  | Command-line interface for drone operations |
|  | Laboratory flight experiments framework |
|  | Camera streaming and recording |

## Architecture



## Modules

| Module | Purpose |
|--------|---------|
|  | MultiWii Serial Protocol implementation |
|  | Vehicle abstraction layer |
|  | OpenCV color tracking for visual navigation |
|  | Neural network library for flight control |
|  | PID controllers, filters, utilities |
|  | Ground station communication |

## The Neural Network Experiment

 is particularly significant — it represents one of Daniel's earliest experiments combining **machine learning with physical hardware control**:

- Trained neural networks to predict optimal flight commands
- PID controllers as baseline with neural network augmentation
- Real-time inference on companion computer
- Precursor to the AI-driven systems he would build later

## Context in My Journey



## Credits

Based on the DronePilot project by [Aldo Vargas](https://github.com/alduxvm). Extended with additional experiments for drone research in Patagonia.

## License

GPL v3

---

*Daniel Dieser — Puerto Madryn, Patagonia*
