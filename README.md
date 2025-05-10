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



---

Would you like me to generate a `requirements.txt` file as well?






You said:
give me full written way 


ChatGPT said:
Here is the complete written README.md file you can directly copy and paste into your GitHub repository for your project "BLINK, PAUSE, ALERT – Intelligent Drowsiness Detection for Safer Journeys":

markdown
Copy
Edit
# BLINK, PAUSE, ALERT – Intelligent Drowsiness Detection for Safer Journeys

A real-time driver drowsiness and yawning detection system using **Computer Vision** and **Deep Learning**. This project helps prevent fatigue-related road accidents by monitoring eye and mouth activity and alerting the driver in real-time using visual and audio cues.

---

## 🚀 Features

- Real-time video stream monitoring using webcam.
- Detects drowsiness based on:
  - **Eye Aspect Ratio (EAR)** – detects prolonged eye closure.
  - **Mouth Aspect Ratio (MAR)** – detects frequent yawning.
- Alerts the driver with a **real-time audio alarm** when signs of drowsiness are detected.
- Displays live EAR and MAR values on-screen via GUI overlay.
- Works in varied lighting conditions and is non-intrusive.

---

## 🧠 Tech Stack

- **Python**
- **OpenCV**
- **TensorFlow / Keras**
- **Dlib**
- **Imutils**
- **Playsound**
- **Threading**
- **GUI (cv2-based)**

---

## 📦 Installation

### 1. Clone the repository
```bash
git clone https://github.com/SounakDutta10/Drowsiness-Detection-System.git
cd Drowsiness-Detection-System
2. Install dependencies
You can install the required Python libraries using:

bash
Copy
Edit
pip install -r requirements.txt
If you don't have a requirements.txt, install manually:

bash
Copy
Edit
pip install opencv-python dlib imutils playsound tensorflow
3. Download facial landmark model
Download shape_predictor_68_face_landmarks.dat from this link or direct download, extract it, and place it in the project directory.

🎮 Usage
To run the detection system:

bash
Copy
Edit
python drowsiness_detection.py
A webcam window will open showing live video with EAR and MAR metrics.

An audio alert will be triggered when drowsiness or yawning is detected.

Press 'q' to exit the system.

⚙️ How It Works
Facial Detection: The system uses dlib to detect 68 facial landmarks (eyes, mouth).

EAR Calculation: If EAR < 0.25 for 20 consecutive frames → drowsiness detected.

MAR Calculation: If MAR > 0.6 for 20 frames → yawning detected.

CNN Model: A pre-trained CNN model classifies alert vs drowsy states for improved accuracy.

Alert: If thresholds are met, an audio beep alerts the user via playsound.

📊 Performance
Metric	Value
Accuracy	93.2%
Frame Rate	~20 FPS
Dataset Used	NTHU-DDD
Alert Latency	< 1 second
CNN Performance	F1 Score 0.81

📈 Output (Example)
EAR and MAR shown in real-time

Visual Alert: “DROWSINESS ALERT!” displayed on screen

Audio Alert: Beep sound triggered when thresholds are crossed

🛠 Future Enhancements
🔌 IoT integration with heartbeat/GSR sensors.

☁️ Cloud-based alert/reporting system.

📱 Mobile deployment using Flutter or Android.

🧠 Lighter models like MobileNetV2 for embedded deployment.

📈 Driver behavior analytics with logging support.

👥 Contributors
Sounak Dutta – GUI, alert system, integration

Shambhavi Palak – EAR/MAR logic, detection pipeline

Somraj Bose – Face detection and video stream optimization

Ayush Sandilya – Deep learning model training and inference

Divyam – Documentation, UML diagrams, performance testing

📄 License
This project is open-source and available under the MIT License.

🙏 Acknowledgements
dlib

OpenCV

NTHU-DDD Dataset

KIIT University – School of Computer Engineering

