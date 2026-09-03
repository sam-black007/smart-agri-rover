# 🌾 Smart Agri Rover

The **Smart Agri Rover** is an agricultural rover designed for automated farming tasks. It combines an **earth hogger**, a **robotic arm for planting saplings**, and a **soil plow** on a single mobile platform, controlled using an Arduino Mega 2560 and dual-axis joystick modules.

---

## 📷 Project Photo

![Smart Agri Rover with robotic arm mounted on the rover](images/arm_on_rover.jpg)

---

## 🚜 What It Does

The rover is a low-cost, educational prototype tailored for precision agriculture:

- **Earth Hogger** – digs and loosens the soil to prepare the ground for planting.
- **Robotic Sapping Arm** – a 4-DOF arm that places saplings into prepared holes.
- **Soil Plow** – plows the soil to till the land before sowing.

The **rover** handles locomotion and is driven by its own controller / receiver, while the **robotic arm** is operated separately using its own Arduino Mega 2560 and joystick modules. This keeps each subsystem modular and independently controllable.

---

## 📌 Features

- 4-DOF robotic arm movement (gripper, wrist, elbow, and base) for sapling placement
- Earth hogger and soil plow attachments for tillage and planting preparation
- EEPROM-based memory to store last servo positions
- Joystick-controlled real-time servo movement
- Simple and reproducible hardware design using SG90 servos

---

## 🧠 Technologies Used

- **Hardware**: Arduino Mega 2560, SG90 Servo Motors, Dual Axis Joysticks
- **Software**: Arduino Programming (C/C++), EEPROM Library, Servo Library
- **Tools**: Arduino IDE / VS Code with PlatformIO, Git/GitHub

---

## 🛠️ How to Use

### 1. Requirements
- Arduino Mega 2560
- 4x SG90 Servo Motors
- 2x Dual Axis Joystick Modules
- Jumper wires
- Power Supply (12V adapter)
- Rover chassis with earth hogger and plow attachments

### 2. Setup Instructions
1. Clone this repo:
   ```bash
   git clone https://github.com/sam-black007/smart-agri-rover.git
   cd smart-agri-rover
   ```
2. Open `robotic_arm.ino` in Arduino IDE or VS Code (with PlatformIO).
3. Connect components as per circuit diagram.
4. Upload the code to the Arduino board.
5. Use the joysticks to control the robotic arm in real time. Drive the rover separately to till, hog, and plant.

---

## 🔌 Circuit Connections

### Joystick to Arduino
| Joystick Pin | Arduino Pin |
|--------------|-------------|
| 5V           | 5V          |
| GND          | GND         |
| VRX (J1)     | A0          |
| VRY (J1)     | A1          |
| VRX (J2)     | A2          |
| VRY (J2)     | A3          |

### Servo to Arduino
| Servo        | Arduino Pin |
|--------------|-------------|
| Gripper      | D6          |
| Up/Down      | D9          |
| Front/Back   | D11         |
| Neck         | D10         |

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).

---
