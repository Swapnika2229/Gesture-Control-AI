# 🖐️ Gesture Control AI

A real-time **AI-powered hand gesture recognition system** that allows users to control Google Slides presentations using hand gestures through a laptop webcam.

The project combines **Computer Vision, Hand Landmark Detection, and Python Automation** to create a touch-free presentation control system.

---

## 🚀 Features

* 🖐️ Real-time hand gesture detection
* 📷 Webcam-based interaction
* 🤖 AI-powered hand landmark tracking using MediaPipe
* 🎯 Gesture-to-action mapping
* 🎮 Hands-free Google Slides control
* ⚡ Real-time visual feedback
* 💻 No additional hardware required
* 🐍 Built entirely with Python

---

## 🧠 Gesture Controls

| Hand Gesture     | Detected Fingers | Action          |
| ---------------- | ---------------: | --------------- |
| ✋ Open Palm      |                4 | Next Slide      |
| 🤟 Three Fingers |                3 | Previous Slide  |
| ✌️ Two Fingers   |                2 | Start Slideshow |
| ✊ Fist           |                0 | Exit Slideshow  |

> **Note:** Gesture behavior may vary depending on the operating system and presentation environment.

---

## 🛠️ Technologies Used

* **Python**
* **OpenCV** – Webcam capture and image processing
* **MediaPipe** – Hand landmark detection
* **PyAutoGUI** – Keyboard automation
* **Computer Vision**
* **Real-Time Gesture Recognition**

---

## 📂 Project Structure

```text
Gesture-Control-AI/
│
├── main.py
├── setup_models.py
├── requirements.txt
├── README.md
├── .gitignore
│
└── models/
    └── hand_landmarker.task
```

The `models/` directory is generated when the MediaPipe hand landmark model is downloaded.

The model file is excluded from GitHub using `.gitignore`.

---

## ⚙️ How It Works

The application follows this workflow:

```text
Laptop Webcam
      ↓
OpenCV Frame Capture
      ↓
MediaPipe Hand Detection
      ↓
Hand Landmark Extraction
      ↓
Finger Position Detection
      ↓
Gesture Recognition
      ↓
Gesture → Keyboard Action
      ↓
Google Slides Control
```

### Processing Pipeline

1. The webcam captures the user's hand in real time.
2. OpenCV processes each camera frame.
3. MediaPipe detects the hand and its landmarks.
4. Finger positions are analyzed.
5. The number of raised fingers is used to identify the gesture.
6. The recognized gesture is mapped to a keyboard action.
7. PyAutoGUI sends the corresponding keyboard command.
8. Google Slides responds to the keyboard action.

---

# 📦 Installation

## 1. Clone the Repository

```bash
git clone https://github.com/Swapnika2229/Gesture-Control-AI.git
```

Move into the project directory:

```bash
cd Gesture-Control-AI
```

---

## 2. Create a Virtual Environment

### Windows

```bash
python -m venv venv
```

Activate it:

```bash
venv\Scripts\activate
```

### macOS / Linux

```bash
python3 -m venv venv
```

Activate it:

```bash
source venv/bin/activate
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

The project uses:

```text
mediapipe==0.10.35
opencv-python>=4.8.0
pyautogui>=0.9.54
```

---

## 4. Download the MediaPipe Hand Model

Run:

```bash
python setup_models.py
```

This creates the `models/` directory and downloads the required:

```text
hand_landmarker.task
```

The model is intentionally excluded from Git because it is a binary model file.

---

# ▶️ Running the Application

Start the application with:

```bash
python main.py
```

A webcam window will open and display the detected hand landmarks.

Show your hand in front of the camera and perform one of the supported gestures.

Press:

```text
Q
```

to close the application.

---

# 🎯 How to Use

1. Open a Google Slides presentation.
2. Start or prepare the presentation mode.
3. Make sure your webcam is available.
4. Run:

```bash
python main.py
```

5. Place your hand in front of the webcam.
6. Perform the supported gesture.
7. The system detects the gesture and sends the corresponding keyboard action.

---

# 📸 Demo

For the best results:

* Use good lighting.
* Keep your hand clearly visible.
* Maintain a moderate distance from the webcam.
* Avoid heavily cluttered backgrounds.
* Keep only one hand in view.

### Recommended Demo Setup

```text
             👋 Hand
                ↓
        ┌───────────────┐
        │    Webcam     │
        └───────┬───────┘
                ↓
       MediaPipe Detection
                ↓
       Gesture Recognition
                ↓
        PyAutoGUI Action
                ↓
       Google Slides 🎞️
```

---

# 💡 Example Use Case

### Touch-Free Presentation

Instead of using a keyboard or mouse, a presenter can use hand gestures to navigate through presentation slides.

This can be useful for:

* 🎓 College presentations
* 🧑‍🏫 Classroom demonstrations
* 💼 Business presentations
* 🏆 Hackathons
* 🤖 AI/Computer Vision demonstrations
* 🎤 Tech workshops

---

# 🔮 Future Improvements

The project can be extended with additional gesture-based controls such as:

* 👉 Swipe gestures for slide navigation
* 🔴 Gesture-controlled laser pointer
* 🔊 Volume control
* 🔍 Zoom in/out gestures
* ✋ Multi-hand gesture recognition
* 🎨 Custom gesture training
* 🧠 Machine-learning-based gesture classification
* 📊 Gesture statistics and analytics
* 🖥️ Support for PowerPoint and other presentation software

---

# 🧪 Current Limitations

* The system currently focuses on single-hand tracking.
* Gesture recognition is primarily based on finger positions.
* Recognition performance depends on lighting and camera quality.
* Keyboard shortcuts may differ between operating systems.
* Presentation software must be active for keyboard automation to have the intended effect.

---

# 📚 Learning Outcomes

This project provides practical experience with:

* Computer Vision
* Artificial Intelligence
* Hand Landmark Detection
* Real-Time Image Processing
* Human-Computer Interaction
* Python Automation
* Webcam Processing
* Gesture Recognition
* MediaPipe
* OpenCV

---

# 🔐 Privacy

The application processes webcam frames locally while it is running.

No cloud-based image upload is required for the hand tracking functionality.

---

# 👨‍💻 Author

**Swapnika Mohanty**

B.Tech – Computer Science and Engineering

---

## ⭐ Project Highlights

```text
AI + Computer Vision
        +
Real-Time Hand Tracking
        +
Gesture Recognition
        +
Python Automation
        =
Touch-Free Presentation Control
```

If you find this project useful, consider giving the repository a ⭐ on GitHub!

---

## 📄 License

This project is intended for educational and demonstration purposes.
