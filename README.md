# ⏰ Arduino Digital Clock with LCD

A simple **digital clock system** built using an Arduino and a 16x2 LCD display. This project allows users to view and manually adjust time using push buttons.

---

## 📌 Features

- Real-time clock using `millis()` (no RTC module required)
- 16x2 LCD display output
- Manual time adjustment:
  - Set **Hours**
  - Set **Minutes**
- Simple button-based interface
- Auto time rollover (seconds → minutes → hours)

---

## 🛠️ Components Required

- Arduino Board (e.g., Arduino Uno)
- 16x2 LCD Display
- Push Buttons × 2
- Resistors (optional for buttons)
- Breadboard & Jumper Wires

---

## 🔌 Pin Configuration

### LCD Connections

| LCD Pin | Arduino Pin |
|--------|------------|
| RS     | 12         |
| EN     | 11         |
| D4     | 5          |
| D5     | 4          |
| D6     | 3          |
| D7     | 2          |

### Buttons

| Button        | Arduino Pin |
|--------------|------------|
| Hour Button  | A0         |
| Minute Button| A1         |

> Buttons use `INPUT_PULLUP`, so no external resistors are required.

---

## ⚙️ How It Works

- The clock updates every second using `millis()`.
- Time variables:
  - `h` → hours
  - `m` → minutes
  - `s` → seconds
- Buttons:
  - Press **Hour Button** → Increases hour
  - Press **Minute Button** → Increases minute
- Debouncing handled using a simple `delay(200)`.

---


---

## 🚀 Getting Started

1. Connect all components as per the wiring diagram.
2. Open Arduino IDE.
3. Install required library:
   - `LiquidCrystal` (usually pre-installed)
4. Upload the code to your Arduino board.
5. Power the board and enjoy your digital clock!

---

## ⚡ Future Improvements

- Add **RTC module (DS3231)** for accurate timekeeping
- Add **AM/PM format**
- Add **alarm feature**
- Replace buttons with **touch or rotary encoder**
- Add **date display**

---

## 🧠 Concepts Used

- Embedded Systems Basics  
- Arduino GPIO & Digital Input  
- LCD Interfacing  
- Time handling using `millis()`  
- Debouncing  

---

## 📷 Project Idea

This project is great for:
- Beginners learning Arduino
- Embedded systems mini-projects
- University practical assignments

---

## 📄 License

This project is open-source and free to use for learning purposes.
