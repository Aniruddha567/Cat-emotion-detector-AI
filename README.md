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
├── best_model.h5           # Trained emotion classification model
├── yolov8n.pt              # YOLOv8 model file
├── runs/                   # YOLOv8 training output (weights, logs)
├── dataset1/               # Training images (cat faces)
├── dataset2/               # Validation images (cat faces)
├── app.py                  # Real-time detection and emotion classification script
├── requirements.txt        # All dependencies
└── README.md               # Project documentation

---

## 📦 Setup Instructions

```bash
# Create environment (optional)
conda create -n catEmotion python=3.10
conda activate catEmotion

# Install dependencies
pip install -r requirements.txt
