# 🚗 YOLO Surveillance Models ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

YOLO_Surveillance_Models/
│
├── plate_detector/             # Detect cars + plates (Iran regular + free zone)
│   ├── train.py
│   ├── data/
│   └── yolovX_plate.pt
│
├── char_recognizer/            # Recognize characters inside license plates
│   ├── train.py
│   ├── data/
│   └── yolovX_char.pt
│
├── car_type_classifier/        # Recognize 150 car types
│   ├── train.py
│   ├── data/
│   └── yolovX_type.pt
│
├── README.md
└── requirements.txt

This repository contains a set of YOLO-based models developed for an end-to-end car surveillance system, including car detection, license plate reading, and vehicle type classification.

## 🔧 Models Overview

- **1. Plate Detector (`plate_detector/`)**
  - Detects vehicles and license plates in a frame.
  - Handles two types of Iranian plates:
    - 🇮🇷 Regular Iranian plates
    - Free Zone (license-free) plates

- **2. Character Recognizer (`char_recognizer/`)**
  - Detects and recognizes individual characters within a license plate region.
  - Optimized for real-time plate reading.

- **3. Car Type Classifier (`car_type_classifier/`)**
  - Identifies car types and brands.
  - Trained on a dataset of 150+ vehicle classes.

## 🚀 Tech Stack

- YOLOv11
- Python, PyTorch
- Custom datasets with annotated labels
- Exported `.pt` model files for deployment

## 📂 Folder Structure

Each subfolder includes:
- `train.py`: Model training script
- `data/`: Sample dataset or annotation format
- `.pt`: Trained YOLO model weights.

