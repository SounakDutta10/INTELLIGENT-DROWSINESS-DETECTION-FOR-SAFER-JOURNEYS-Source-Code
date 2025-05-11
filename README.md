# BLINK, PAUSE, ALERT – Intelligent Drowsiness Detection for Safer Journeys

A real-time driver drowsiness detection system using **Computer Vision** and **Deep Learning** to prevent road accidents by monitoring eye blinks and yawning patterns.

---

## 🚀 Features

- Real-time video stream analysis via webcam.
- Detects drowsiness using:
  - **Eye Aspect Ratio (EAR)** for blink detection.
  - **Mouth Aspect Ratio (MAR)** for yawning detection.
- Triggers an **audio alarm** when fatigue is detected.
- Lightweight and easily deployable.
- Displays live EAR and MAR values on screen with GUI overlay.

---

## 🧠 Tech Stack

- **Python**
- **OpenCV**
- **TensorFlow / Keras**
- **Dlib**
- **Imutils**
- **Playsound**
- **Threading**

---

## 🖼 Demo

![Drowsiness Detection Demo](https://your-demo-link-if-any.gif)

---

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/SounakDutta10/Drowsiness-Detection-System.git
   cd Drowsiness-Detection-System
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Download shape predictor

Download shape_predictor_68_face_landmarks.dat and place it in the root folder.

🔧 Usage
Run the script:

bash
Copy
Edit
python drowsiness_detection.py
Press 'q' to exit the application.

⚙️ How It Works
The system uses dlib to detect 68 facial landmarks.

EAR is calculated from the eye landmarks:

If EAR drops below 0.25 for 20+ consecutive frames, the driver is considered drowsy.

MAR is calculated from mouth landmarks:

If MAR exceeds 0.6 for 20+ frames, yawning is detected.

A CNN model is also integrated to validate state from facial cues.

📊 Performance
Metric	Value
Accuracy	93.2%
Dataset Used	NTHU-DDD
Real-time FPS	20+

📌 Future Work
Integrate physiological sensors (HRV, GSR).

Cloud-based alert system for fleet management.

Deploy to Raspberry Pi/Jetson Nano for edge computing.

Personalized EAR/MAR calibration per user.

🧑‍💻 Contributors

Sounak Dutta

Shambhavi Palak

Somraj Bose

Ayush Sandilya

Divyam

📄 License
This project is licensed under the MIT License. See the LICENSE file for details.



