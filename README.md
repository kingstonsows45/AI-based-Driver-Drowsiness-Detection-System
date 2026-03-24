# 😴 AI-Based Driver Drowsiness Detection System

## 📌 Overview

This project is an AI-based driver monitoring system that detects drowsiness in real time using computer vision techniques. It tracks eye movements using facial landmarks and calculates the Eye Aspect Ratio (EAR) to determine whether the driver's eyes are closed for a prolonged period.

---

## 🚀 Features

* Real-time face and eye detection
* Eye Aspect Ratio (EAR) based drowsiness detection
* Visual alert when drowsiness is detected
* Lightweight and runs on standard webcam
* Edge AI implementation (no cloud required)

---

## ⚙️ Technologies Used

* Python
* OpenCV
* dlib (Facial Landmark Detection)
* SciPy (Distance calculation)

---

## 🧠 Working Principle

### 👁️ Eye Aspect Ratio (EAR)

The system calculates EAR using eye landmarks:

EAR = (||p2 - p6|| + ||p3 - p5||) / (2 * ||p1 - p4||)

* If EAR is **low** → Eyes are closed
* If EAR is **high** → Eyes are open

---

### ⚠️ Drowsiness Detection Logic

* If EAR < threshold (0.25)
* For consecutive frames (>20)
  👉 System triggers **DROWSINESS ALERT**

---

## 📦 Installation

```bash
pip install opencv-python dlib scipy
```

---

## ▶️ Run the Project

```bash
python src/main.py
```

---

## 📷 Output

* Displays real-time EAR value
* Shows alert message when driver is drowsy

---

## 🌐 Applications

* Automotive safety systems
* Driver monitoring systems (DMS)
* Smart vehicles
* Accident prevention systems

---

## 🔮 Future Improvements

* Add buzzer or alarm system
* Integrate with IoT for remote alerts
* Use deep learning models for higher accuracy
* Add head pose detection

---

## 👨‍💻 Author

Sowgandh S
Embedded Systems & AI–IoT Developer
GitHub: https://github.com/kingstonsow45
