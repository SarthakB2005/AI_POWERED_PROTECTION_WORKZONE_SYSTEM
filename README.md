# 🤖 AI Powered Robotic Protection Zone
### (AI + IoT Based Industrial Safety System)

---

## 📌 Overview
An intelligent safety system designed for industrial robotic zones that ensures:
- Only authorized personnel can enter
- Mandatory PPE compliance
- Automatic machinery shutdown when humans are inside

---

## ⚙️ Features

- AI-based PPE Detection (Helmet + Vest)
- Password Authentication using Keypad
- Automated Gate Control using Servo Motors
- IR Sensor for Entry Detection
- Automatic Machinery Shutdown System
- People Counting Mechanism (IN / OUT)
- LED Status Indicator (System ON / OFF)

---

## 🧠 System Working

### WORKING PROTOTYPE OF PROJECT :
[![Watch Demo](https://youtu.be/UqvlWyaQqJM.jpg)](https://youtu.be/UqvlWyaQqJM)

### 1. PPE Detection
- Camera captures the person
- Python AI model checks for helmet and safety vest

### 2. Authentication
- User enters password using keypad

### 3. Gate Access
- If PPE + Password are correct:
  - Gates open automatically

### 4. Entry Detection
- IR sensor detects entry
- Gates close immediately

### 5. Safety Shutdown
- Machinery turns OFF when a person enters the zone

### 6. Smart Restart Logic
- System tracks:
  - IN Count
  - OUT Count

System condition:
IN = OUT → System ON  
IN ≠ OUT → System OFF  

---

## 🔄 Flowchart

📌 Click below to view the complete system flowchart:

👉 [Open Flowchart](project/images/Working.jpeg)

##PIN CONFIGURATION in STM32 Cube IDE

📌 Click below to view the Pin configuration:

👉 [PIN_CONFIGURATION](project/images/Working.jpeg)





