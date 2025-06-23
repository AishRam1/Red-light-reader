# Red-light-reader

**Red Light Reader** is an intelligent, real-time facial tracking system designed to improve screen-time ergonomics and user focus. It leverages your webcam and facial landmark recognition to detect your presence and attention while you use your computer. If the system detects that you're not paying attention or you've left the screen, it will **dim the brightness** and **play an alert sound**, encouraging healthier and more conscious digital habits.

---

## 📌 Problem Statement

In today’s digital age, people often spend long hours staring at screens without taking breaks, leading to eye strain, fatigue, and decreased productivity. Moreover, prolonged distraction can result in missed meetings, paused video lectures, or unsaved progress. There’s a need for a **smart attention-awareness system** that can assist in managing screen time and reducing unnecessary eye strain.

---

## ✅ Solution

Red Light Reader uses **MediaPipe FaceMesh** to track facial landmarks through your webcam. If it doesn’t detect a user or senses the face is turned away for a prolonged time, it performs two actions:
- Dims the screen brightness using `screen-brightness-control`
- Plays a warning tone (via `winsound`) to regain user focus

This tool functions like a **“digital guardian”** to help reduce unhealthy screen habits.

---

## ✨ Features

- 🧠 **Real-Time Facial Tracking**: Uses machine learning to identify and track 468 facial landmarks.
- 💤 **Distraction Detection**: Recognizes when you're away or not paying attention.
- 💡 **Auto Brightness Control**: Dims the screen when you're distracted, increases when you're back.
- 🔔 **Audio Alerts**: Plays a warning sound when you're inattentive.
- 📊 **Customizable Thresholds**: Modify delay, brightness levels, and detection sensitivity.
- 📷 **Non-intrusive Monitoring**: Uses only your webcam and runs locally for privacy.

---

## 🛠️ Tech Stack

| Component | Description |
|----------|-------------|
| Python 3 | Programming language |
| OpenCV   | For accessing and displaying webcam frames |
| MediaPipe | FaceMesh for facial landmark tracking |
| NumPy | For numerical operations |
| screen-brightness-control | Adjusts monitor brightness on Windows |
| winsound | Plays system beep sounds |
| PIL | For displaying processed frames inside notebooks (optional) |
