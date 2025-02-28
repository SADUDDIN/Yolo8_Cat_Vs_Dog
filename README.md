# YOLOv8 Image Classification 🚀

## 📌 Overview
This project trains a **YOLOv8 classification model** on a custom dataset and evaluates its performance.

## 📂 Dataset
- Images are stored in `/content/drive/MyDrive/PetImagesYOLO/`
- Classes: `Dogs 🐶`, `Cats 🐱` (example)

## 🔥 Training
Trained using:
```python
from ultralytics import YOLO
model = YOLO("yolov8n-cls.pt")  # Load YOLOv8 classification model
model.train(data="/content/drive/MyDrive/PetImagesYOLO", epochs=5, plots=True)
