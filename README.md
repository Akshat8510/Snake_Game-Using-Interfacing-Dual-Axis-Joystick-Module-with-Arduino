# 🐍 Arduino Snake: Dual-Axis Joystick Edition

![Arduino](https://img.shields.io/badge/Platform-Arduino-00979D.svg)
![C++](https://img.shields.io/badge/Language-C++-blue.svg)
![Hardware](https://img.shields.io/badge/Focus-Embedded%20Systems-orange.svg)

## 📌 Project Overview
This project is a classic "Snake" game built using an **Arduino Uno** and interfaced with a **Dual-Axis Joystick Module**. It demonstrates the fundamental concepts of embedded systems, including analog-to-digital signal processing, real-time coordinate mapping, and low-level display control.

## 🕹️ How it Works
The game logic is handled entirely by the Arduino. The **Joystick** provides two analog inputs (X and Y axes). The code converts these raw voltage values into directional commands (Up, Down, Left, Right) to guide the snake across an **8x8 LED Matrix (MAX7219)**.

## 🛠️ Hardware Components
- **Microcontroller:** Arduino Uno / Nano
- **Input:** Dual-Axis Joystick Module (KY-023)
- **Output:** 8x8 LED Matrix with MAX7219 Driver
- **Other:** Breadboard, Jumper Wires, 9V Battery/USB Power

## 🔌 Pin Connections
| Component | Pin (Arduino) | Description |
| :--- | :--- | :--- |
| **Joystick VRx** | A0 | X-Axis Analog Input |
| **Joystick VRy** | A1 | Y-Axis Analog Input |
| **Joystick SW** | D2 | Button Select (Reset/Start) |
| **Matrix DIN** | D12 | Data In |
| **Matrix CS**  | D10 | Chip Select |
| **Matrix CLK** | D11 | Clock |

## ✨ Features
- **Intuitive Controls:** Smooth movement using analog joystick thresholds.
- **Dynamic Speed:** The snake speed increases as you consume "food."
- **Collision Detection:** Logic for wall-bumping and self-intersection.
- **EEPROM Support:** (Optional) High-score saving even after power-off.

## 🚀 Getting Started
1. **Hardware Setup:** Connect the components according to the pin-out table above.
2. **Library Installation:** Ensure you have the `LedControl` or `MD_MAX72xx` library installed in your Arduino IDE.
3. **Upload:** Open `Snake_Game.ino`, select your COM port, and hit upload.
4. **Play:** Use the joystick to navigate. Don't hit the walls!

## 📸 Media
<img width="369" height="338" alt="image" src="https://github.com/user-attachments/assets/520ace02-1548-4074-8893-c52476d9bfc2" />



## 📂 Project Structure
```text
├── Snake_Game.ino       # Main Arduino source code
├── Schematics/          # Fritzing or hand-drawn circuit diagrams
└── README.md            # Project documentation
