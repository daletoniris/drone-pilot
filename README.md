# Drone Pilot

**Autonomous pilot software for companion computers -- MultiWii, Pixhawk, PX4 (2014)**

> Part of Daniel Dieser's robotics and drone research period (2012-2014) in Puerto Madryn, Patagonia.

---

## What Is This?

Drone Pilot is an autonomous flight control system that runs on companion computers (Raspberry Pi, laptops) alongside flight controllers. It bridges the gap between manual RC control and fully autonomous flight through **PID-based position controllers, neural network experiments, and computer vision**.

This project was a critical piece in Daniel's journey: it combined **hardware control, real-time algorithms, computer vision, and early neural network experiments** -- all running on a drone in the physical world.

## Features

- **MultiWii Serial Protocol** -- Direct communication with MultiWii flight controllers
- **Pixhawk/PX4 Support** -- DroneKit integration for advanced missions
- **Hover Controller** -- PID-based position hold using motion capture feedback
- **Height Controller** -- Altitude hold with sonar/barometer data
- **Neural Network Controller** -- Experimental flight control using trained neural nets
- **Joystick Control** -- UDP bridge from ground station (Matlab/Python) to flight controller
- **Waypoint Navigation** -- Autonomous multi-point flight paths
- **Computer Vision** -- OpenCV color tracking for visual navigation
- **Flight Data Logger** -- Black box recording of all flight parameters

## Scripts

| Script | Description |
|--------|-------------|
| `mw-hover-controller.py` | PID position hold -- the core autonomous flight algorithm |
| `mw-height-controller.py` | Altitude hold controller |
| `mw-neural.py` | Neural network flight controller -- experimental ML for flight |
| `mw-joystick.py` | UDP joystick commands from ground station to MultiWii |
| `mw-waypoint.py` | Autonomous waypoint navigation |
| `mw-logdata.py` | Flight data recording (IMU, RC, attitude) |
| `mw-simulink-controller.py` | Simulink integration for control design |
| `cli.py` | Command-line interface for drone operations |
| `flylab.py` | Laboratory flight experiments framework |
| `video.py` | Camera streaming and recording |

## Modules

| Module | Purpose |
|--------|---------|
| `modules/pyMultiwii.py` | MultiWii Serial Protocol implementation |
| `modules/vehicle.py` | Vehicle abstraction layer |
| `modules/vision.py` | OpenCV color tracking for visual navigation |
| `modules/pyrenn.py` | Neural network library for flight control |
| `modules/utils.py` | PID controllers, filters, utilities |
| `modules/UDPserver.py` | Ground station communication |

## The Neural Network Experiment

`mw-neural.py` is particularly significant -- it represents one of Daniel's earliest experiments combining **machine learning with physical hardware control**:

- Trained neural networks to predict optimal flight commands
- PID controllers as baseline with neural network augmentation
- Real-time inference on companion computer
- Precursor to the AI-driven systems he would build later

## Context in My Journey

The hover controller taught me PID tuning. The neural controller taught me ML can control physical systems. The vision module taught me computer vision. The waypoint system taught me autonomous navigation.

All of this converged years later into AI systems that autonomously navigate attack patterns instead of physical space.

## Credits

Based on the DronePilot project by Aldo Vargas. Extended with additional experiments for drone research in Patagonia.

## License

GPL v3

---

*Daniel Dieser -- Puerto Madryn, Patagonia, Argentina*
*Telegram: [@mrmoz33](https://t.me/mrmoz33)*
