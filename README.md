# DIY Laser XY Scanner

A low-cost DIY laser XY scanner built using Arduino, dual stepper motors, and custom control algorithms.

This project is capable of drawing geometric shapes and characters using a laser beam and two-axis stepper motor movement.

<p align="center">
  <img src="Images/heart.jpg" width="300">
  <img src="Images/square.jpg" width="300">
</p>

---

# Features

- Dual-axis laser scanning system
- Custom Arduino control software
- Python serial controller
- Real-time laser drawing
- Draws:
  - Square
  - Circle
  - Heart
  - L Character
  - V Character
  - A Character
- Manual WASD control
- Adjustable speed and drawing size
- Low-cost hardware design

---

# Project Overview

The system uses:

- Arduino
- 2x 28BYJ-48 stepper motors
- ULN2003 motor drivers
- Laser diode module
- Custom XY movement algorithms

The laser beam is redirected using two mirrors attached to stepper motors, creating a simple XY laser scanner.

Unlike traditional galvo systems, this setup is extremely low-cost and beginner-friendly.

---

# My Contribution

The mechanical design inspiration was taken from the following open-source project:

- Instructables Project:  
  https://www.instructables.com/Low-Cost-DIY-Stepper-Motor-Laser-XY-Scanner-Cutter/

- Original GitHub Repository:  
  https://github.com/ThingEngineer/Laser-XY-Scanner

I only used the 3D model/mechanical idea as inspiration.

All control software, movement logic, drawing algorithms, serial communication structure, and shape generation code were written and redesigned by me.

This project includes completely custom:
- Arduino firmware
- Motion logic
- Shape generation
- Serial command system
- Drawing routines

---

# Hardware

## Components

| Component | Quantity |
|---|---|
| Arduino Uno/Nano | 1 |
| 28BYJ-48 Stepper Motor | 2 |
| ULN2003 Driver Board | 2 |
| Laser Module | 1 |
| Mirrors | 2 |
| 3D Printed Parts | 1 Set |

---

# Software

## Arduino

- Language: C++
- Library:
  - AccelStepper

## Python

- Python 3
- pyserial

Install pyserial:

```bash
pip install pyserial
```

---

# Controls

| Command | Action |
|---|---|
| w | Move Up |
| s | Move Down |
| a | Move Left |
| d | Move Right |
| m | Save Center |
| 1 | Draw Square |
| 2 | Draw Circle |
| 3 | Draw Heart |
| 4 | Draw A |
| 5 | Draw L |
| 6 | Draw V |
| x | Stop |

---

# Project Images

## Heart Shape

<p align="center">
  <img src="Images/heart.jpg" width="350">
</p>

## Circle

<p align="center">
  <img src="Images/circle.jpg" width="350">
</p>

## Square

<p align="center">
  <img src="Images/square.jpg" width="350">
</p>

## L Character

<p align="center">
  <img src="Images/l.jpg" width="350">
</p>

---

# Future Improvements

- SVG drawing support
- G-code support
- Laser modulation (TTL)
- Higher-speed scanning
- Galvo mirror upgrade
- Image drawing support
- Joystick control
- WiFi control
- Mobile application

---

# Safety Warning

This project uses a laser diode.

Avoid direct eye exposure to the laser beam and always use proper laser safety precautions.

---

# License

This project is open-source.

Please give proper attribution if you use or modify this project.
