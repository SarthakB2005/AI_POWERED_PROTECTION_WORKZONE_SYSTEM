# 🔌 Hardware Components & Setup

This document describes all the hardware components used in the project and their purpose.

---

## 🧩 Components Used

### 1. STM32F103 Microcontroller
- Acts as the main controller
- Controls gates, sensors, and system logic
- Link : https://www.amazon.in/STM32F103C8T6-Minimum-Development-Electronic-Components/dp/B08TVVSK4K 

---

### 2. Laptop Camera
- Used for AI-based PPE detection
- Connected to Python model

---

### 3. USB - TTL Converter
- Used to communicate between the pyton file and the STM32
- The python file will provide signal to STm32 i.e. the PPE kit is detected , the only the other functioning of the STM32 will come in prograss according to the program
- Link : https://www.amazon.in/REES52-Module-Serial-Converter-Replace/dp/B01I6MXWV2

---

### 4. Servo Motors
- Used to control entry/exit gates
- Opens and closes gates automatically
- Link : https://www.amazon.in/Generic-servo-Motor/dp/B0GP77GC4H

---

### 5. Keypad Module
- Used for password authentication
- Adds an extra layer of security
- Link : https://www.amazon.in/Robodo-MO14-Matrix-Membrane-Arduino/dp/B073Q33R6K?th=1

---

### 6. IR Sensors
- Detect entry and exit of person
- Used for counting IN and OUT
- Link : https://www.amazon.in/Circuit-components-Infrared-Obstacle-Avoidance/dp/B09P8VGPVC

---

### 7. LED Indicator
- Shows system status:
  - ON → System Active
  - OFF → System Shutdown

---

### 8. Power Supply
- Provides power to STM32 and components
- 9V supply
- Link : https://www.amazon.in/Electronic-Spices-COMBO-Battery-Connector/dp/B088FQJ5N4/ref=sr_1_1?dib=eyJ2IjoiMSJ9.SioRcMXfJMJRYvIclv6FGLBF-3VQTTugwRXeYoejB03GgprAtCQRSLRi7IkjIzO_SUSGY4RXOVgJl5UjhuygY_W9PlsKrImvcoEFwxi2lJ1xHJtdB0j7j3azjU-wGVZvXi-0LzpkaVvEySo8SNGe7cZBwhP4YD_i5dp_NRh7_R_wwlSiE_o3emuY0lh-gmJ_yvqxnfET0sABzI9anXDoLKXcY5F12Y-FzOJWH2jou24.h_hDfPnoAsGB5i9QnW4UkP6SzRqIddjRRlZjh6OAtKk&dib_tag=se&keywords=hw+battery&qid=1774979372&sr=8-1
---

### 9.Buck converter
- Helpful in supplying powersupply to all devices
- It basically converts the 9V supply to 5V for sensors
- Link : https://www.amazon.in/LM2596S-DC-DC-Converter-Supply-Module/dp/B0FLF6GYJN

## ⚙️ Working Integration

- Camera detects PPE using AI
- Keypad verifies password
- STM32 processes authentication
- Servo motors control gates
- IR sensors track entry/exit
- System shuts down machinery when person enters

---

## 🧠 Special Feature

### 🔴 Safety Shutdown Mechanism

- System turns OFF when a person enters
- Remains OFF until:

IN Count = OUT Count

- Ensures no human is inside during machine operation

---

## 📌 Notes

- Ensure proper wiring of sensors
- Use stable power supply
- Calibrate IR sensors correctly
