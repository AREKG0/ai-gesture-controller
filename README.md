# AI Hand Gesture Controller

Control your computer with hand gestures in real time — no mouse, no keyboard.

Built with Python, MediaPipe and OpenCV as a solo project by a 2nd year CS student.

![Python](https://img.shields.io/badge/Python-3.11-blue)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0.10.32-green)
![OpenCV](https://img.shields.io/badge/OpenCV-4.9-orange)

---

## Demo

> Point your hand at the webcam and control your entire computer with gestures.

| Gesture | Action |
|---|---|
| ☝ Index finger only | Move mouse cursor |
| ✌ Peace sign | Volume up |
| ✊ Fist | Play / Pause media |
| 🖐 Open hand | Take screenshot |
| 👍 Thumbs up | Previous (left arrow) |
| 🤙 Pinky only | Next (right arrow) |
| 🤏 Pinch | Left click |

---

## How it works

1. Webcam captures live video feed
2. MediaPipe detects 21 hand landmarks in real time
3. Finger states calculated by comparing tip vs base coordinates
4. Gesture matched to an action
5. PyAutoGUI performs the system action instantly

---

## Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.11 | Core language |
| MediaPipe 0.10.32 | Hand landmark detection |
| OpenCV | Webcam feed + display |
| PyAutoGUI | System control (mouse, keyboard) |
| NumPy | Coordinate mapping |

---

## Setup & Run

### 1. Clone the repo
```bash
git clone https://github.com/AREKG0/ai-gesture-controller.git
cd ai-gesture-controller
```

### 2. Create virtual environment
```bash
python -m venv venv
venv\Scripts\activate        # Windows
source venv/bin/activate     # Mac/Linux
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run
```bash
python gesture_controller.py
```

Press **Q** to quit.

---

## Project Structure

```
ai-gesture-controller/
├── gesture_controller.py   # main application
├── requirements.txt        # dependencies
└── README.md
```

---

## What I learned

- Real-time computer vision with MediaPipe
- Hand landmark geometry and finger state detection
- System-level automation with PyAutoGUI
- Debugging library version conflicts across Python versions
- Git version control and GitHub portfolio management

---

## Future improvements

- Add more custom gestures
- Two-hand gesture support
- Volume bar visualisation on screen
- Package as a Windows .exe with PyInstaller
- Add voice commands with SpeechRecognition

---

## Author

**AREKG0** — 2nd year Computer Science student  
Building AI and MLOps projects from scratch.  
[GitHub](https://github.com/AREKG0)
