# Threat Detection
Threat Detection is a real-time AI-powered system that detects harmful weapons like guns and knives using the YOLOv5 object detection model. Designed to enhance public and private security, the system processes live video streams from a web camera and identifies potential threats with high accuracy. It leverages deep learning, computer vision, and open-source tools like OpenCV and PyTorch, and is trained on a custom dataset from Roboflow. This project aims to assist security personnel with faster and more accurate threat identification in sensitive environments such as airports, schools, malls, and events.

# 🔍 Threat Detection – Real-Time Weapon Detection System

![YOLOv5](https://img.shields.io/badge/YOLOv5-Object%20Detection-blue)
![Python](https://img.shields.io/badge/Python-3.x-yellow)
![OpenCV](https://img.shields.io/badge/OpenCV-RealTime-green)
![PyTorch](https://img.shields.io/badge/PyTorch-DeepLearning-red)

## 💡 Overview

Threat Detection is a real-time weapon detection system that uses deep learning to identify harmful weapons such as guns and knives in live video streams. Powered by the YOLOv5 model, this system is built for proactive security surveillance, reducing the need for manual monitoring and improving response time to potential threats.

## 🚀 Features

- 🔫 Detects guns and knives in real time
- 📹 Integrates with live webcam feeds
- 🎯 High accuracy with mAP > 90%
- 💻 Lightweight and optimized for performance
- 🔄 Real-time frame-by-frame analysis
- 🛠️ Custom-trained model on diverse datasets

## 🧰 Technologies Used

- **Python**
- **YOLOv5**
- **PyTorch**
- **OpenCV**
- **Roboflow** (Dataset)
- **Google Colab** (Training environment)
- **Webcam** (Real-time input)

## 🧪 How It Works

1. **Data Collection & Preprocessing**
   - Collected labeled weapon images from Roboflow.
   - Applied resizing, augmentation, and normalization.

2. **Model Training**
   - Trained a YOLOv5 model using PyTorch and Google Colab.
   - Evaluated with high mAP and low false positives/negatives.

3. **Real-Time Integration**
   - Integrated the model with a webcam using OpenCV.
   - Live video frames are processed with bounding boxes for threats.

4. **Optimization**
   - Techniques like frame skipping and model compression used for faster performance (~20 FPS).

## 📈 Results

- 🔍 **High Precision & Recall**: mAP > 90%
- ⚡ **Fast Inference**: ~20 FPS after optimization
- ✅ **Reliable Detection**: Consistent performance in different environments

## 📌 Future Scope

- Add detection for explosives and more weapon types
- Integrate emergency alert systems (SMS/Alarm)
- Mobile & cloud deployment
- Advanced AI models with lower latency
- GUI for ease of use

## 🛠️ Setup Instructions

```bash
# Clone the repo
git clone https://github.com/your-username/threat-detection.git
cd threat-detection

# Install dependencies
pip install -r requirements.txt

# Run detection script
python detect.py --source 0 --weights best.pt --conf 0.


