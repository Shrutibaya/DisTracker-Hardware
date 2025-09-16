# 📘 DisTracker – Distraction Monitoring Wristband  

## 📍 Project Overview  
This project was developed as part of the **WISH Mentorship Program at Texas Instruments**, by a team of 5 students.  
🔗 [Project Link](https://www.canva.com/design/DAGpgSCPiC4/OsMNQZafhaJAm09p1mCJew/edit)  

**Team Members:** Manvitha, Akhila, Nitisha, Anshu, Shruti  

The project focuses on tackling **smartphone and social media distractions** among students during study or work sessions. We designed a **wearable wristband** that detects distraction using physiological and motion signals, and provides subtle, real-time feedback to help regain focus.  

---

## 🎯 Problem Statement  
Students often get distracted by smartphones and social media, leading to:  
- Reduced focus and productivity  
- Higher stress and mental fatigue  
- Poor academic and work performance  

**Goal:** Build a **non-intrusive, wearable solution** that monitors focus, detects distractions, and gently nudges the user back to task.  

---

## 🛠️ Solution – DisTracker Wristband  
The **DisTracker** integrates hardware sensors, embedded processing, and TinyML models for **real-time distraction detection**.  

### Key Features:  
- **Physiological sensing**  
  - *EDA (Electrodermal Activity)* – stress/attention response  
  - *PPG (Photoplethysmography)* – heart rate and HRV  
  - *3-axis Accelerometer + Gyroscope* – motion/gesture detection  
- **Screen Monitoring (Android app)** for app usage analysis  
- **TinyML (1D CNN model)** for low-power, on-device distraction classification  
- **Feedback mechanisms:** vibration motor + LED indicators  

---

## ⚡ Prototype  
- **Hardware:** MCU + BLE, EDA & PPG sensors, onboard IMU, vibration motor, LiPo battery  
- **Software:** Embedded TinyML model, Android app integration  
- **Form Factor:** Compact wearable wristband  

---

## 💰 Cost Analysis  
Estimated prototype cost: **~₹3000**  
*(optimized further by sensor integration and chip-level packaging).*  

---

## 🚀 Testing & Validation  
- **EDA Tests:** dry vs. wet skin, stress/meditation experiments  
- **HRV Tests:** exercise, deep breathing  
- **Accelerometer Tests:** still, tilt, tap, shake  
- **Motor Tests:** standalone + sensor integration  
- **MCU Tests:** BLE, I²C, UART, onboard IMU  
- **TinyML Model Tests:** input feature validation, distraction classification, false positive rate  
- **Environmental Robustness:** temperature variation, sweat simulation  

🔗 [Testing Codes Link](https://docs.google.com/document/d/16yhCMC3rUK1BajkGnp0COPW4I09iADXiPK6Dr1_ApEE/edit?usp=sharing)  

---

## ⚖️ Challenges & Solutions  
- **High power use in screen monitoring** → filtered apps first, then selective monitoring  
- **Sensor variability (HRV/EDA)** → baseline personalization per user  
- **Cost concerns** → integration of multiple sensors in one chip  
- **Temperature effect on sensors** → added compensation sensor with ML adjustment  
- **False triggers in buttons** → implemented Schmitt Trigger debounce circuit  

---

## 📚 References  
- [TI Application Note on EDA sensing](https://www.ti.com/lit/ab/sbaa556/sbaa556.pdf)  
- [NCRI Glossary – eLORETA](https://www.thencri.org/glossary/eloreta/)  
- [Research paper on stress detection](https://pdfs.semanticscholar.org/b5f7/095bae46986a142c93f2890e6ce33624522c.pdf)  

---
