# ☀️ Solar Tracker using Arduino

This project implements a **dual-axis solar tracking system** using **four LDR sensors and servo motors** to dynamically align a solar panel for maximum sunlight exposure.

The system continuously analyzes real-time light intensity and adjusts the panel orientation to improve overall solar energy efficiency.

This project was developed as part of an academic embedded systems project at **University School of Information, Communication & Technology (USICT)**.

---

## 🧠 Project Overview

- Uses **4 Light Dependent Resistors (LDRs)** to detect sunlight direction  
- Controls **horizontal and vertical servo motors** - Automatically aligns the solar panel toward maximum light intensity  
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
```

* **Top vs Bottom LDRs** → Vertical movement
* **Left vs Right LDRs** → Horizontal movement
* Servo movement occurs only when light difference exceeds tolerance

---

## 🔌 Hardware Components Required

* Arduino Board (UNO / Nano / compatible)
* 4 × LDR sensors
* 2 × Servo motors (Horizontal & Vertical)
* Solar panel (prototype mount)
* 4 × Resistors (for LDR voltage divider)
* Breadboard
* Jumper wires
* External power supply (recommended for servos)

---

## 📂 Project Structure

```text
solar-tracker/
├── solar_tracker.ino
└── README.md
```

---

## ▶️ How to Run the Project

### Step 1: Install Arduino IDE

Download and install Arduino IDE from:
[https://www.arduino.cc/en/software](https://www.arduino.cc/en/software)

---

### Step 2: Make Hardware Connections

**LDR Connections (Analog Inputs)**

| LDR Position | Arduino Pin |
| ------------ | ----------- |
| Top-Left     | A2          |
| Top-Right    | A1          |
| Bottom-Left  | A3          |
| Bottom-Right | A0          |

Each LDR must be connected using a **voltage divider circuit** with a resistor.

**Servo Connections**

| Servo            | Arduino Pin    |
| ---------------- | -------------- |
| Horizontal Servo | Digital Pin 2  |
| Vertical Servo   | Digital Pin 13 |

⚠️ **Note:** Use an external 5V power supply for servos to prevent Arduino resets.

---

### Step 3: Upload the Code

1. Open **Arduino IDE**
2. Open `solar_tracker.ino`
3. Select:
   * **Board:** Arduino UNO (or your board)
   * **Port:** Correct COM port
4. Click **Upload**

---

### Step 4: Test the System

1. Place the solar panel under sunlight or a bright lamp
2. Move the light source in different directions
3. Observe:
   * Horizontal servo moves left/right
   * Vertical servo moves up/down
4. The panel automatically aligns toward maximum light

---

## 📌 Key Features

* Dual-axis solar tracking
* Real-time light intensity analysis
* Analog signal processing using LDRs
* Servo limit protection
* Low-cost and efficient design

---

## 📈 Skills Demonstrated

* Embedded systems programming
* Arduino & sensor interfacing
* Analog signal processing
* Control logic implementation
* Renewable energy optimization

---

## 🔮 Future Enhancements

* PID control for smoother tracking
* LCD display for light values and angles
* Data logging for efficiency analysis
* Weather-aware tracking algorithm
* ESP32-based implementation

---

## 📜 License

MIT License

---

## 👤 Author

Developed as an academic project focusing on renewable energy optimization using embedded systems.
