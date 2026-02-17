# 🖐️ Virtual-Canvas-With-ML

> A computer vision project implemented with **OpenCV** and **Machine Learning** using **MediaPipe**. Draw on a virtual canvas using just your hand gestures — no touch required!

## ✨ Features

- 🎨 Draw in **4 colors** — Blue, Green, Red, Yellow
- 🖐️ Real-time **hand tracking** using MediaPipe ML
- 🎙️ **Voice command** support — say *"screenshot"* to save your canvas
- 📸 Screenshots **auto-saved** with timestamp
- 🧹 **Clear canvas** with a gesture
- ⚡ Runs on **live webcam feed**

## 🛠️ Tech Stack

- **Python** — Core programming language
- **OpenCV** — Real-time video capture and drawing on frames
- **MediaPipe** — ML-based hand landmark detection
- **SpeechRecognition** — Listening and processing voice commands
- **PyAutoGUI** — Capturing and saving screenshots
- **Threading** — Running voice listener and canvas in parallel

## ⚙️ Installation

```
pip install opencv-python mediapipe SpeechRecognition pyautogui keyboard numpy
```

## ▶️ How to Use

1. **Run** the script:
   ```
   python virtual_canvas.py
   ```
2. Show your **index finger** to start drawing.
3. **Pinch** (bring thumb close to index finger) to lift the pen.
4. Point to the **color buttons** at the top to switch colors.
5. Point to **CLEAR** to wipe the canvas clean.
6. Say **"screenshot"** to save your drawing.
7. Press **`q`** to quit.

## 🖼️ How It Works

MediaPipe detects **21 hand landmarks** in real time through the webcam. The **index fingertip** (landmark 8) acts as the drawing pointer. When the **thumb and index finger come close**, drawing pauses — just like lifting a pen off paper. A separate thread continuously listens for voice commands in the background.

## 📁 Project Structure

```
Virtual-Canvas-OpenCV/
├── screenshots/                       # Auto-saved canvas screenshots
│   └── screenshot_YYYYMMDDHHMMSS.png
├── virtualcanvasopencv.py             
├── virtual_canvas.py                  
└── README.md
```

**Himali Barde**

- GitHub: https://github.com/himalibarde
- LinkedIn: www.linkedin.com/in/himali-barde-5b4b1a34a
- Email: himalibarde859@gmail.com

