# Line Following Robot Without Microcontroller

## Overview
This repository contains the complete project report, circuit simulation, and hardware implementation details for an autonomous **Line Following Robot built without any microcontroller**. The decision-making is powered entirely by analog electronic circuits using IR sensors, operational amplifier comparators, and motor driver ICs[cite: 2].

---

## 🛠 Hardware & Components
- **IR Proximity Sensors** (Infrared Detection)[cite: 2]
- **LM358 IC** (Operational Amplifier / Comparator)[cite: 2]
- **L293D IC** (Dual H-Bridge Motor Driver)[cite: 2]
- **7805 Voltage Regulator**[cite: 2]
- **BO Motors & Wheels**[cite: 2]
- **9V Battery Power Supply**[cite: 2]

---

## ⚡ Working Logic & Truth Table

| Left Sensor | Right Sensor | Left Motor | Right Motor | Robot Movement |
| :---: | :---: | :---: | :---: | :---: |
| **0 (White)** | **0 (White)** | ON | ON | **Moves Forward** |
| **0 (White)** | **1 (Black)** | OFF | ON | **Turns Right** |
| **1 (Black)** | **0 (White)** | ON | OFF | **Turns Left** |
| **1 (Black)** | **1 (Black)** | OFF | OFF | **Stops** |

---

## 📐 Key Mathematical Formulas Included in Report
1. **Voltage Divider Equation:** Calculates output voltage based on sensor resistance variations[cite: 2].
   $$V_{out} = V_{in} \times \frac{R_{LDR}}{R + R_{LDR}}$$[cite: 2]

2. **DC Motor Speed Relation:**
   $$N = \frac{V - I_a R_a}{K \Phi}$$

---

## 🚀 Key Highlights & Future Improvements
- **Zero Software Dependency:** Pure hardware automation[cite: 2].
- **Cost Effective & Simple:** Ideal baseline architecture for learning basic robotics[cite: 2].
- **Future Enhancements:** Integration of PWM speed control, Arduino/microcontroller intelligence, and ultrasonic obstacle avoidance[cite: 2].
