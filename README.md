<div align="center">

# 🦁 YOLOv8 Wildlife Detection & Tracking

### Animal Detection, Tracking & Activity Heatmap Generation from Wildlife Videos

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![YOLOv8](https://img.shields.io/badge/YOLOv8-Ultralytics-red)
![OpenCV](https://img.shields.io/badge/OpenCV-ComputerVision-green)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Status](https://img.shields.io/badge/Project-Active-success)

</div>

---

# 📌 Overview

This project implements a **wildlife monitoring system** that detects, tracks, and analyzes animals in wildlife videos using **YOLOv8 and Computer Vision**.

The system automatically:

* Detects animals in video frames
* Assigns **unique tracking IDs**
* Monitors **movement behavior**
* Detects **inactive animals**
* Generates **movement heatmaps** showing high-activity regions

This project demonstrates the use of **object detection and computer vision techniques for wildlife monitoring and conservation research**.

---

# 🚀 Key Features

✔️ Wildlife Detection using **YOLOv8**
✔️ Multi-Object Tracking with **Unique IDs**
✔️ Animal Activity Monitoring (**Active / Idle**)
✔️ **Inactive Animal Alerts**
✔️ **Movement Heatmap Generation**
✔️ Batch Processing of Multiple Videos
✔️ High-Quality Annotated Output Videos

---

# 🧠 Technologies Used

* Python
* YOLOv8 (Ultralytics)
* OpenCV
* NumPy
* Google Colab
* Computer Vision

---

# 🏗 System Workflow

```text
Input Wildlife Video
        ↓
YOLOv8 Object Detection
        ↓
Multi-Object Tracking
        ↓
Movement Analysis
        ↓
Active / Idle Behavior Detection
        ↓
Heatmap Generation
        ↓
Annotated Output Video
```

---

# 📥 Download YOLOv8 Model

The trained model is **not included in this repository** because GitHub restricts large files.

You can download the model from:

https://github.com/shibi27/animal-detection-yolov8

After downloading, place the model file here:

```
YoloModels/best.pt
```

Update the model path in the notebook:

```python
model = YOLO("/content/drive/MyDrive/YoloModels/best.pt")
```

---

# ⚠️ Important: Run in Google Colab

It is recommended to run this project in **Google Colab** to avoid environment or dependency errors.

Running locally may cause issues such as:

* CUDA / GPU configuration problems
* Library compatibility issues
* Missing dependencies

Running the notebook in **Google Colab ensures smooth execution**.

---

# 🚀 Run in Google Colab

Open the notebook using the badge below.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1oOON6wvW28es_HYmYb2QgqeEvCYan7Nu?usp=sharing)

---

# ⚙️ Setup in Google Colab

### 1️⃣ Mount Google Drive

```python
from google.colab import drive
drive.mount('/content/drive')
```

---

### 2️⃣ Install Required Libraries

```python
!pip install ultralytics opencv-python numpy
```

---

### 3️⃣ Place Files in Google Drive

Example structure:

```
MyDrive
│
├── YoloModels
│   └── best.pt
│
├── Yolov8_Input_Videos
│   └── test_video.mp4
│
└── Yolov8_Videos_Results
```

---

### 4️⃣ Update Paths in the Notebook

```
/content/drive/MyDrive/YoloModels/best.pt
/content/drive/MyDrive/Yolov8_Input_Videos
/content/drive/MyDrive/Yolov8_Videos_Results
```


# 📊 Output

The system generates:

### 🎥 Annotated Output Video

* Bounding boxes
* Animal species labels
* Tracking IDs
* Activity state (Active / Idle)

### 🔥 Wildlife Activity Heatmap

Heatmaps visualize **areas where animals move the most**.

---

# 🌍 Applications

* Wildlife Monitoring
* Forest Surveillance
* Animal Behavior Studies
* Biodiversity Tracking
* Conservation Research

---

# 🔮 Future Improvements

* Real-time wildlife camera monitoring
* Web dashboard for analysis
* Edge deployment on Jetson / Raspberry Pi
* Improved species classification

---
