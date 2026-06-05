# ✋ Hand Gesture Browser Control

Control your browser using hand gestures detected through your webcam! This project uses **MediaPipe Hand Landmarker** and **OpenCV** to recognize finger gestures and perform actions like opening social media profiles or closing all browser windows.

##  Features

*  **1 Finger** → Open Portfolio Website
*  **2 Fingers** → Open GitHub Profile
*  **3 Fingers** → Open Instagram Profile
*  **4 Fingers** → Open LinkedIn Profile
*  **Fist Gesture** → Close Browsers
*  Real-time hand tracking using webcam
*  Gesture hold detection to avoid accidental triggers
*  Automatic MediaPipe model download

---

##  Technologies Used

* Python
* OpenCV
* MediaPipe Tasks API
* Webbrowser Module
* Subprocess Module

---

## 📦 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/anupamyadavanurag/Hand-Controller.git
cd Hand-Controller
```

### 2. Install Dependencies

```bash
pip install opencv-python mediapipe
```

---

## ▶️ Run the Project

```bash
python main.py
```

The application will automatically download the required MediaPipe hand model on first launch.

---

## 🎮 Gesture Controls

| Gesture      | Action             |
| ------------ | ------------------ |
| ☝️ 1 Finger  | Open Portfolio     |
| ✌️ 2 Fingers | Open GitHub        |
| 🤟 3 Fingers | Open Instagram     |
| 🖖 4 Fingers | Open LinkedIn      |
| ✊ Fist      | Close All Browsers |

Hold the gesture for a short duration to trigger the action.

---

## 📸 How It Works

1. Captures live video from webcam.
2. Detects hand landmarks using MediaPipe.
3. Counts raised fingers.
4. Maps finger count to predefined actions.
5. Executes browser commands after gesture confirmation.

---

## 📁 Project Structure

```text
├── main.py
├── hand_landmarker.task
├── README.md
```

---

## 🔧 Customization

You can modify the URLs inside the script:

```python
webbrowser.open_new_tab('YOUR_URL_HERE')
```

Replace them with your own portfolio, social media profiles, or any website.

---

## ⚠️ Requirements

* Python 3.9+
* Webcam
* Windows OS (browser-closing feature uses PowerShell)

---

## 👨‍💻 Author

**Anupam Yadav**

* Portfolio: https://anupamyadavanurag.github.io
* GitHub: https://github.com/anupamyadavanurag
* LinkedIn: https://www.linkedin.com/in/anupamyadavanurag
