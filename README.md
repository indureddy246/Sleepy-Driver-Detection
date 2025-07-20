
🛑 Sleepy Driver Detection
A real-time drowsiness and face recognition system built using OpenCV, Dlib, and Machine Learning. This project monitors a driver's eye activity to detect signs of sleep and identifies known faces, enhancing road safety by issuing visual alerts when drowsiness is detected.

🔧 Features
Sleep Detection: Uses eye landmark analysis to determine if the driver is sleepy.

Facial Recognition: Identifies known drivers using a reference image.

Machine Learning: Predicts eye state using a trained Linear Regression model.

Real-Time Alerts: Displays warning when drowsiness is detected for consecutive frames.

🧰 Technologies Used
Python

OpenCV

Dlib (with 68 face landmarks model)

face_recognition

scikit-learn

pandas

📁 Required Files
shape_predictor_68_face_landmarks.dat – Dlib model for face landmarks

dataset.csv – Dataset with facial distance measurements for training

celalresim.jpeg – Reference image for known face identification

📦 Installation
Install required libraries:

bash
Copy
Edit
pip install opencv-python dlib face_recognition pandas scikit-learn
🚀 How It Works
Captures live video using your webcam.

Detects face and facial landmarks.

Calculates distances between eye and nose landmarks.

Predicts eye state using a regression model.

If both eyes are closed for multiple frames, triggers a drowsiness alert.

Recognizes faces and displays name if matched with reference.

🖥️ Usage
Place all required files in the same directory.

Run the script:

bash
Copy
Edit
python sleepy_driver_detection.py
Press q to exit the application.

📌 Output Meaning
✅ Green Box – Known face and awake

🔷 Blue Box – Unknown face

❌ Red Box – Sleepy face with “ATTENTION” warning

🔄 Future Enhancements
Add sound or vibration alerts

Support for multiple known drivers

Improve accuracy using CNN or deep learning models
