# 🤖 Bluetooth Controlled PipeBot

A compact, Arduino-powered robotic system designed for navigation in confined pipe environments. Controlled wirelessly via Bluetooth, the PipeBot is capable of precise movements including forward, backward, turning, and directional navigation.

---

## 📘 Project Overview

**Course:** Software Engineering 1  
**Team Name:** PIPEBOT  
**Student:** Akshit Singh

This project is a hardware-software integration assignment aimed at understanding real-time robotic control using Arduino and Bluetooth communication. The robot receives directional commands through a Bluetooth module and moves accordingly using dual motor control.

---

## 🧠 Features

- 🔄 Full-range movement: Forward, Backward, Left, Right
- 🎮 Real-time Bluetooth command control
- 🧭 Directional maneuvers: left/right forward, left/right backward
- 🛠️ Motor driver integration for smooth control

---

## 🔧 Technologies Used

- **Arduino UNO**
- **HC-05 Bluetooth Module**
- **L298N Motor Driver**
- **DC Motors**
- **Serial Communication (9600 baud rate)**

---

## 🗂️ Project Structure

```text
PipeBot/
├── PipeBot.ino         # Main Arduino source code
├── README.md           # Project documentation
└── wiring_diagram.png  # Optional: visual circuit layout
```

---

## 🔌 Wiring Configuration

| Component              | Arduino Pin |
|------------------------|-------------|
| Left Forward Motor     | D7          |
| Left Backward Motor    | D6          |
| Right Forward Motor    | D4          |
| Right Backward Motor   | D5          |
| Bluetooth TX → Arduino RX | D0 (RX) |
| Bluetooth RX ← Arduino TX | D1 (TX) |

Make sure to power the motors separately using a 9V or 12V source via the motor driver.

---

## 🎮 Control Commands

| Command | Action                     |
|---------|----------------------------|
| F       | Move Forward               |
| B       | Move Backward              |
| L       | Turn Left                  |
| R       | Turn Right                 |
| S       | Stop                       |
| G       | Left Forward Only          |
| H       | Left Backward Only         |
| I       | Right Forward Only         |
| J       | Right Backward Only        |

Use any Bluetooth terminal app (like **Serial Bluetooth Terminal**) to send these characters.

---

## 🚀 Getting Started

1. **Upload Code**  
   Open the `PipeBot.ino` file in the Arduino IDE and upload it to your Arduino board.

2. **Connect Bluetooth**  
   Pair your phone with the HC-05 module (default password: `1234` or `0000`).

3. **Control the Robot**  
   Open a Bluetooth terminal app and send the desired command characters.

---

## 🧾 References

- [pinMode() - Arduino Docs](https://www.arduino.cc/reference/en/language/functions/digital-io/pinmode/)
- [digitalWrite() - Arduino Docs](https://www.arduino.cc/reference/en/language/functions/digital-io/digitalwrite/)
- [Serial Communication - Arduino Docs](https://www.arduino.cc/en/Reference/Serial)


---

## 📌 Notes

- Always disconnect the Bluetooth module while uploading code to the Arduino.
- Ensure stable power supply for motors to avoid voltage drop.

