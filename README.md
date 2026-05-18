<h1 align="center">✋ HandTrackingModule</h1>

<div align="center">

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green?style=for-the-badge&logo=opencv)
![MediaPipe](https://img.shields.io/badge/MediaPipe-Hand%20Tracking-orange?style=for-the-badge&logo=google)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

### 🚀 Reusable Hand Tracking Module using OpenCV & MediaPipe

A professional and reusable computer vision module for real-time hand detection, hand landmark tracking, and gesture-based AI applications.

</div>

---

#  📌 Features

✅ Real-time Hand Detection  
✅ 21 Hand Landmark Tracking  
✅ Multi-Hand Support  
✅ FPS Counter  
✅ Easy-to-Import Modular Architecture  
✅ OpenCV + MediaPipe Integration  
✅ Beginner Friendly  
✅ Reusable in Future AI Projects  

---

#  🖼️ Hand Landmark Reference

## MediaPipe Hand Landmark Mapping

<p align="center">
  <img src="hand_landmarks.png" width="900">
</p>

---

#  📂 Project Structure

```bash
HandTrackingModule/
│
├── HandTrackingModule.py
├── HandTrackingGame.py
├── HandTrackingMin.py
├── hand_landmarks.png
├── requirements.txt
├── README.md
└── .gitignore
```

---

# ⚙️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| OpenCV | Computer Vision |
| MediaPipe | Hand Tracking |
| NumPy | Numerical Operations |

---

#  📦 Installation 

## 1️⃣ Clone Repository

```bash
git clone https://github.com/Prajjwalsen/HandTrackingModule.git
```

---

## 2️⃣ Open Project Folder

```bash
cd HandTrackingModule
```

---

## 3️⃣ Create Virtual Environment

```bash
python -m venv .venv
```

---

## 4️⃣ Activate Virtual Environment

### Windows

```bash
.venv\Scripts\activate
```

### Linux / Mac

```bash
source .venv/bin/activate
```

---

## 5️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Usage

## Basic Hand Tracking

```python
import cv2
import HandTrackingModule as htm

cap = cv2.VideoCapture(0)

detector = htm.handDetector()

while True:
    success, img = cap.read()

    img = detector.findHands(img)
    lmList = detector.findPosition(img)

    if len(lmList) != 0:
        print(lmList[4])

    cv2.imshow("Image", img)
    cv2.waitKey(1)
```

---

# 🧠 Hand Landmark IDs

| Finger | Landmark IDs |
|---|---|
| Thumb | 1, 2, 3, 4 |
| Index Finger | 5, 6, 7, 8 |
| Middle Finger | 9, 10, 11, 12 |
| Ring Finger | 13, 14, 15, 16 |
| Pinky Finger | 17, 18, 19, 20 |

---

# 🚀 Future Projects Using This Module

This module can be used in:

- 🎮 Gesture Controlled Games
- 🖱️ AI Virtual Mouse
- 🔊 Finger Volume Control
- 🎨 Air Drawing System
- 🤖 Jarvis Gesture Commands
- ✍️ Sign Language Recognition
- 🧠 AI Gesture Automation

---

# 📈 Future Improvements

- Finger Counting
- Gesture Recognition
- AI Mouse Control
- Dynamic Gesture Detection
- Hand Distance Measurement
- Gesture-Based Shortcuts

---

# 🤝 Contributing

Contributions are welcome!

If you'd like to improve this project:

1. Fork the repository
2. Create a new branch
3. Commit changes
4. Push the branch
5. Create a Pull Request

---

# ⭐ Support

If you found this project useful:

🌟 Star the repository  
🍴 Fork the project  
📢 Share with others  

---

# 👨‍💻 Author

## Prajjwal Sen

Computer Science Engineer | AI & Data Science Enthusiast | Computer Vision Developer

GitHub:  
https://github.com/Prajjwalsen

---

# 📜 License

This project is licensed under the MIT License.
