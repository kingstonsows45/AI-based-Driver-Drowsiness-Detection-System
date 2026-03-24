# 😴 AI-Based Driver Drowsiness Detection System

## 📌 Overview

This project is an AI-based real-time driver drowsiness detection system using MediaPipe Face Mesh running on Raspberry Pi. It detects eye closure using Eye Aspect Ratio (EAR) and triggers alerts through a buzzer and Telegram notifications.

---

## 🚀 Features

* Real-time eye tracking using MediaPipe
* Drowsiness detection using EAR (Eye Aspect Ratio)
* Buzzer alert system (GPIO)
* Instant Telegram notification
* Edge AI processing (Raspberry Pi)
* Blink vs Drowsiness differentiation

---

## ⚙️ Hardware Used

* Raspberry Pi
* USB Camera
* Buzzer (GPIO Pin 17)

---

## 💻 Software & Technologies

* Python
* OpenCV
* MediaPipe
* RPi.GPIO
* Telegram Bot API
* Requests Library

---

## 🧠 Detection Logic

### 👁️ Eye Aspect Ratio (EAR)

Drowsiness is detected based on eye closure duration:

* If EAR < threshold → eyes closed
* If closed for multiple frames → DROWSINESS detected

---

## 🔌 Working Principle

1. Camera captures live video
2. MediaPipe detects facial landmarks
3. Eye landmarks are extracted
4. EAR is calculated
5. If EAR < threshold for continuous frames:

   * Buzzer turns ON
   * Telegram alert is sent
6. If eyes open:

   * System resets
   * Buzzer OFF

---

## 📱 Telegram Alert

When drowsiness is detected:

```text
⚠️ Drowsiness Detected! Please take a break.
```

---

## 📦 Installation

```bash
pip install opencv-python mediapipe RPi.GPIO requests
```

---

## ▶️ Run the Project

```bash
python src/main.py
```

---

## 🌐 Applications

* Driver safety systems
* Automotive ADAS systems
* Smart vehicle monitoring
* Fleet management systems

---

## 🔮 Future Improvements

* Add face recognition (driver identification)
* Integrate GPS alert system
* Cloud dashboard for monitoring
* AI fatigue prediction model

---

## 👨‍💻 Author

Sowgandh S
Embedded Systems & AI–IoT Developer
GitHub: https://github.com/kingstonsow45
