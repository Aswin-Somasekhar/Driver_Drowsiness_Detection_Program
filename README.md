# 🛑 Driver Drowsiness Detection

## 🚗 Project Overview

This project is designed to help **prevent road accidents** caused by driver fatigue or drowsiness. Using real-time video from a webcam, the system monitors the user's eyes and triggers an alert if signs of drowsiness are detected.

---

## 🎯 Aim

To detect and alert when a driver is drowsy by monitoring eye activity and comparing it against normal blinking patterns, thereby enhancing road safety.

---

## 🧠 Methodology

- The system continuously captures live video feed using the **webcam**.
- It detects the **user’s eyes** and measures how long they remain closed.
- According to **Harvard’s database of useful biological numbers**, the typical blink lasts between **100–400 milliseconds**.
- If the eye remains closed for longer than the threshold, it is treated as a sign of drowsiness.
- In such cases, an **audio alert** is triggered, and a **visual message notification** is displayed on the screen to wake up the user.

---

## 🛠️ Technologies & Packages Used

| Package | Purpose |
|--------|---------|
| `opencv` | Capturing live video frames from the webcam |
| `dlib` | Facial landmark detection (predicting model) |
| `numpy` | Matrix and array operations |
| `pygame` | Playing audio alerts |
| `cmake` | Required to build dlib |
| `wheel` | Required to install dlib |

---

## 📁 Data Note

One data/model file used in this project (**shape predictor** `.dat` file) is not included in this repository due to its large size.  
You can manually download it from [dlib's official repository](http://dlib.net/files/) and place it in the project directory.

Example file:  
`shape_predictor_68_face_landmarks.dat`

---

## 🚀 Getting Started

1. Clone the repository
2. Install required packages:
  pip install opencv-python dlib numpy pygame cmake wheel
3.Download the required .dat file (see above)
4.Run the Python script:
  python drowsiness_detection.py
