# ☀️ Solar Tracker using Arduino

This project implements a **dual-axis solar tracking system** using **four LDR sensors and servo motors** to dynamically align a solar panel for maximum sunlight exposure.

The system continuously analyzes real-time light intensity and adjusts the panel orientation to improve overall solar energy efficiency.

This project was developed as part of an academic embedded systems project at **University School of Information, Communication & Technology (USICT)**.

---

## 🧠 Project Overview

- Uses **4 Light Dependent Resistors (LDRs)** to detect sunlight direction
- Controls **horizontal and vertical servo motors**
- Automatically aligns the solar panel toward maximum light intensity
- Includes an **electrical model** to simulate and verify tracking accuracy
- Demonstrates real-time analog signal processing

---

## 🛠️ Tech Stack

- **Microcontroller:** Arduino (UNO / compatible)
- **Programming Language:** C (Arduino)
- **IDE:** Arduino IDE
- **Actuators:** Servo motors
- **Sensors:** LDRs (Analog input)

---

## ⚙️ Working Principle

```text
Sunlight
   ↓
LDR Sensors (4 Quadrants)
   ↓
Analog Signal Processing
   ↓
Light Intensity Comparison
   ↓
Servo Motor Adjustment
   ↓
Optimized Solar Panel Alignment
