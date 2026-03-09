# 📡 Arduino-based Ultrasonic Radar System

A hardware-software hybrid system that detects objects within a 180-degree radius and visualizes them on a real-time radar interface.

---

## 🚀 How it Works
1. **The Sensor:** An HC-SR04 Ultrasonic sensor is mounted on a SG90 Servo motor.
2. **The Sweep:** The Arduino rotates the servo from 15° to 165° and back.
3. **The Logic:** The sensor sends out sound waves; the time taken for the echo to return is used to calculate the distance.
4. **The Visuals:** Data is sent via Serial communication to a **Processing** sketch, which renders a green radar-style display on your computer screen.

---

## 📸 Circuit Layout
![Circuit Diagram](Circuit%20diagram.jpeg)

---

## 🔌 Circuit Connections
Referencing the diagram above:

| Component | Component Pin | Arduino Pin |
| :--- | :--- | :--- |
| **Servo Motor** | Signal (Blue/Yellow) | Digital Pin 11 |
| **Servo Motor** | VCC (Red) | 5V |
| **Servo Motor** | GND (Black/Brown) | GND |
| **HC-SR04** | Trig (Yellow) | Digital Pin 8 |
| **HC-SR04** | Echo (Green) | Digital Pin 9 |
| **HC-SR04** | VCC (Red) | 5V |
| **HC-SR04** | GND (Black) | GND |

---

## 🛠️ Components Used
* **Microcontroller:** Arduino Uno R3
* **Sensor:** HC-SR04 Ultrasonic Sensor
* **Actuator:** SG90 Servo Motor
* **Prototyping:** Breadboard and Jumper Wires

---

## 📂 Project Files
* `radar1__ino.ino`: The source code to be uploaded to your Arduino.
* `sketch_260306a.pde`: The Processing code to run on your PC for the radar visualization.
* `Circuit diagram.jpeg`: The wiring schematic for the hardware setup.

---

## 🖥️ Getting Started
1. **Hardware:** Connect the components as shown in the circuit diagram.
2. **Arduino:** Open `radar1__ino.ino` in the Arduino IDE and upload it to your board.
3. **Processing:** Open `sketch_260306a.pde` in the Processing IDE. 
   - *Note: Ensure the Serial Port in the Processing code matches your Arduino's COM port.*
4. **Run:** Execute the Processing sketch to see your radar in action!

---
**Developed by Manoj Kumar PV** *Building intelligent systems @ Chaman Bhartiya School*
