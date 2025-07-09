# 🐱 Cat Facial Emotion Detection

A real-time computer vision project that detects cat faces and classifies their emotions using a two-stage pipeline:

1. **YOLOv8** for cat face detection  
2. **EfficientNetB2 (Transfer Learning)** for emotion classification

---

## 🔧 Features

- 🧠 Transfer learning with EfficientNetB2 (or MobileNetV2 for lightweight inference)
- 🎯 YOLOv8 object detection for accurate face localization
- ⚡ Real-time inference using webcam
- 📉 Model optimizations: Early stopping, dropout, weight checkpointing
- 📦 Live predictions using OpenCV GUI

---

## 📁 Folder Structure

project/
│
├── best_model.h5 # Trained emotion classification model
├── runs/ # YOLOv8 training output (weights, logs)
├── images/ # Optional test images
├── app.py # Real-time detection and emotion classification
├── requirements.txt # All dependencies
└── README.md # You're reading this!


---

## 📦 Setup Instructions

```bash
# Create environment (optional)
conda create -n catEmotion python=3.10
conda activate catEmotion

# Install dependencies
pip install -r requirements.txt
