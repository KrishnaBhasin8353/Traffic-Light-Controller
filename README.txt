# 🚦 Traffic Light Controller with Object Detection

## 📌 Objective
To design and implement a smart traffic light controller using Arduino, 555 Timer IC, and a shift register, simulating real-world traffic signal operations with pedestrian safety enhancement.

---

## 📝 Project Overview
This project demonstrates a miniature traffic light control system built using:
- **555 Timer IC** (Astable Mode) – Generates clock pulses
- **Shift Register** – Controls LED sequence
- **Arduino Uno** – Processes IR sensor input and controls buzzer
- **IR Sensor** – Detects object/motion
- **Buzzer** – Provides warning during red-light violation

The system enhances pedestrian safety by triggering a buzzer alert when an object is detected during the red-light phase.

---

## ⚙️ Working Principle

- The **555 Timer IC** generates timing pulses.
- The **Shift Register (Q0–Q9)** controls LED sequencing:
  - Q0–Q3 → 🔴 Red (4s)
  - Q4 → 🔴🟡 Red + Yellow (1s)
  - Q5–Q8 → 🟢 Green (4s)
  - Q9 → 🟡 Yellow (1s)
- The cycle repeats continuously.
- During the **Red phase**, if the **IR sensor detects motion**, the Arduino activates the buzzer.

---

## 🔧 Hardware Components

- Arduino Uno  
- 555 Timer IC  
- Shift Register  
- IR Sensor  
- Buzzer  
- LEDs (Red, Yellow, Green)  
- Resistors (10kΩ, 100kΩ variable)  
- Capacitor (100µF)  
- PN Junction Diodes  
- Zener Diode  
- 9V Battery  

---

## ⏱ Timing Formula
