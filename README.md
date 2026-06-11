# 🖐️ Hand Gesture Based Volume Control

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0097A7?style=flat)
![Platform](https://img.shields.io/badge/Platform-Windows-blue)

> Control your system volume using just your hand — no keyboard, no mouse.

---

## 🎯 Overview

An AI-powered computer vision application that lets you control your PC's 
volume using hand gestures via webcam. By tracking the distance between 
your **thumb and index finger**, the system adjusts volume in real time — 
perfect for presentations, clean rooms, or accessibility use cases.

---

## 🚀 How It Works

1. Webcam captures live video feed
2. **MediaPipe** detects and tracks hand landmarks
3. Euclidean distance between thumb tip & index tip is calculated
4. Distance is mapped (interpolated) to volume range 0–100%
5. **pycaw** applies the volume change to Windows master audio
6. **OpenCV** overlays visual feedback: fingertip circles, volume bar, FPS

---

## 🛠️ Tech Stack

| Library | Purpose |
|---|---|
| OpenCV | Video capture & visual overlay |
| MediaPipe | Hand landmark detection |
| pycaw | Windows audio control |
| NumPy | Distance calculation & interpolation |

---

## ⚙️ Installation

```bash
git clone https://github.com/Amaldaskm1234/Hand-Gesture-Based-Volume-Control-.git
cd Hand-Gesture-Based-Volume-Control-
pip install -r requirements.txt
python "Hand Gesture-Based System Volume Controller.py"
```

---

## 📋 Requirements

```
opencv-python
mediapipe
pycaw
numpy
comtypes
```

---

## 🎮 Usage

- 👌 **Pinch fingers together** → Volume decreases
- 🤏 **Spread fingers apart** → Volume increases
- Real-time volume bar and percentage shown on screen

---

## 👤 Author

**Amaldas K M** — [LinkedIn](https://linkedin.com/in/amaldaskm) | [GitHub](https://github.com/Amaldaskm1234)
