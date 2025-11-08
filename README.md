# YOLO Heart Rate Detector

A real-time heart rate detection system using YOLOv8 Face Detection and rPPG (remote Photoplethysmography) from a webcam or USB camera.

## 📌 Features
- Detects your face in real time using YOLOv8.
- Calculates heart rate (BPM) from subtle color changes in skin (rPPG signal).
- Uses multiple facial ROIs — forehead and under-eyes for improved accuracy.
- Automatic camera fallback: USB → Webcam if external camera is disconnected.
- Works on both Windows & Linux (tested with Conda environment).

## ⚙️ Setup Instructions

1. Clone the repository
   git clone https://github.com/<your-username>/YOLO_HeartRate_Detector.git
   cd YOLO_HeartRate_Detector

2. Create and activate Conda environment
   conda create -n yolov8hr python=3.10 -y
   conda activate yolov8hr

3. Install dependencies
   pip install -r requirements.txt

4. Download YOLOv8-Face model
   Download the ONNX model file and place it inside the models/ folder.
   Link: https://github.com/derronqi/yolov8-face/releases

## ▶️ Run the Project
   python multi_rot_test.py

   - Connect your USB camera (e.g., DroidCam or Iriun) before running.
   - If the external camera isn’t detected, the system automatically switches to your webcam.


## 👨‍💻 Author
Developed by K S Nauman Ahmed .
