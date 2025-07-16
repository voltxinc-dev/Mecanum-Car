# 🤖 Arduino-Powered Mecanum Car

A DIY Arduino-based Mecanum wheel robotic car that can move in all directions using two motor drivers and standard hardware. Built for flexibility, maneuverability, and learning!

## 🚗 Project Overview

This project involves building a four-wheeled Mecanum car powered by an **Arduino UNO/Nano**, controlled via **Bluetooth** or **RC**, and driven using **two motor drivers (L298N or similar)**. The Mecanum wheels allow **omnidirectional movement**, enabling the car to move forward, backward, strafe sideways, and rotate.

---

## 🧰 Components Used

| Component            | Quantity | Notes                                 |
|----------------------|----------|----------------------------------------|
| Arduino UNO/Nano     | 1        | Main controller                        |
| L298N Motor Driver   | 2        | Each driver controls 2 motors          |
| Mecanum Wheels       | 4        | Omnidirectional motion                 |
| DC Motors (Gear Motors) | 4     | Matched with Mecanum wheels            |
| Power Supply (Li-ion / Lipo Battery) | 1 | Ensure sufficient current for all motors |
| Bluetooth Module (HC-05/HC-06) | 1 | For remote control                    |
| Chassis              | 1        | Custom or prebuilt                     |
| Jumper Wires         | -        | For connections                        |
| Optional: Ultrasonic Sensor | 1 | For obstacle avoidance                 |
| Optional: MPU6050 Gyro | 1     | For orientation sensing                |

---

## ⚙️ Wiring Overview

- **Motor Driver 1** controls **Front Left** and **Rear Right** motors.
- **Motor Driver 2** controls **Front Right** and **Rear Left** motors.
- Each motor driver is connected to **Arduino PWM pins** for speed control.
- All grounds (motor drivers, Arduino, power source) must be connected.

> **Tip:** Use heat sinks and proper power regulation to prevent overheating.

---

## 🔌 Pin Configuration (Example)

| Arduino Pin | Connection            |
|-------------|------------------------|
| D3, D5      | Motor Driver 1 IN1/IN2 |
| D6, D9      | Motor Driver 1 IN3/IN4 |
| D10, D11    | Motor Driver 2 IN1/IN2 |
| D12, D13    | Motor Driver 2 IN3/IN4 |
| VIN/GND     | Power & Ground         |
| RX/TX       | Bluetooth Module       |

---

## 🧠 Software Logic

- Each wheel’s direction and speed is calculated based on input commands (e.g., forward, strafe, rotate).
- PWM signals control speed via the motor driver’s enable pins.
- Optional: Implement obstacle avoidance or sensor feedback.

---

## 🕹️ Control Options

- **Bluetooth App** (e.g., Arduino Bluetooth Controller on Android)
- **Serial Monitor**
- **RC Transmitter** (if using an interface)

---

## 📂 File Structure

