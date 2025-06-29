# ✋ Hand Gesture-Based Volume and Mouse Control

A real-time hand gesture recognition system to control **system volume** and **mouse pointer** using only a webcam — built with **OpenCV**, **MediaPipe**, and **PyAutoGUI**.

---

## 🚀 Features

- 🎚️ **Volume Control**: Move thumb and index finger closer/farther to decrease/increase volume.
- 🖱️ **Mouse Movement**: Track index finger to move the mouse cursor on the screen.
- 🤏 **Click and Drag**: Use pinch gesture (thumb + index) for left-click or drag.
- 🎥 **Real-Time**: Fast, responsive system running at ~25–30 FPS using webcam input.

---

## 🛠️ Technologies Used

- **Python 3**
- **OpenCV** – for video processing and drawing
- **MediaPipe Hands** – for hand landmark detection
- **PyAutoGUI** – to control the system mouse and volume
- **NumPy** – for geometric calculations

---

## 🧠 How It Works

- Detects **21 hand landmarks** using MediaPipe.
- Calculates **Euclidean distance** between landmarks to trigger gestures.
- Maps hand coordinates to screen coordinates for accurate pointer control.
- Volume level is adjusted using distance between **thumb tip (id 4)** and **index tip (id 8)**.

---

## 📦 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hand-gesture-control.git
   cd hand-gesture-control
