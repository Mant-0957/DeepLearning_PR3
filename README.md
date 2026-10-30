# 🔥 Deep Learning PR 3 – Computer Vision & Object Detection

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenCV-5.0-green?logo=opencv&logoColor=white" />
  <img src="https://img.shields.io/badge/YOLOv8-Ultralytics-purple" />
  <img src="https://img.shields.io/badge/Deep%20Learning-Computer%20Vision-red" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter" />
</p>

## 📌 Project Overview

This project focuses on **Computer Vision and Deep Learning** using Python, OpenCV, YuNet Face Detection, and YOLOv8.

The objective is to understand and implement classical image-processing techniques and modern deep-learning-based detection models in a single integrated computer vision pipeline.

The project progresses from basic image manipulation to real-time face detection, object detection, and performance benchmarking.

**Institute:** Red & White Skill Education  
**Subject:** Deep Learning  
**Project:** PR 3  
**Project Type:** Practical Computer Vision Implementation

---

## 🎯 Project Objectives

- Understand morphological image-processing operations.
- Implement bitwise operations using binary masks.
- Analyze grayscale and colour image histograms.
- Perform brightness and contrast adjustments.
- Detect human faces using the pretrained YuNet model.
- Detect multiple objects using YOLOv8.
- Compare confidence and IoU thresholds.
- Build an integrated face and object detection pipeline.
- Measure and compare processing performance using FPS.

---

## 🛠️ Technologies & Libraries

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| OpenCV | Image processing and computer vision |
| NumPy | Numerical operations and image arrays |
| Matplotlib | Image visualization and plotting |
| Pandas | Data analysis and result tables |
| Ultralytics | YOLOv8 object detection |
| YuNet | Face detection |
| Jupyter Notebook | Project implementation |

---

## 📂 Project Structure

```text
DeepLearning_PR3/
│
├── DeepLearning_PR3.ipynb
│
├── data/
│   ├── images/
│   │   ├── lena.jpg
│   │   ├── baboon.jpg
│   │   ├── fruits.jpg
│   │   ├── bus.jpg
│   │   └── zidane.jpg
│   │
│   └── models/
│       └── face_detection_yunet_2023mar.onnx
│
├── plots/
│   ├── sample_image_pack.png
│   ├── original_vs_binary.png
│   ├── morphology_operations.png
│   ├── morphology_opening_kernel_grid.png
│   ├── morphology_closing_kernel_grid.png
│   ├── bitwise_operations.png
│   ├── histogram_comparison.png
│   ├── brightness_contrast_comparison.png
│   ├── face_detection_comparison.png
│   ├── yolo_detections.png
│   ├── yolo_confidence_iou_tuning.png
│   ├── yolo_per_class_summary.png
│   └── fps_comparison.png
│
├── requirements.txt
│
└── README.md
```

*Note: The data, model, and plots folders are created or populated when the notebook is executed. The structure above represents the recommended repository organization.*

---

## 📚 Project Tasks & Implementation

### 1️⃣ Morphological Operations

Implemented four fundamental morphological operations using OpenCV.

- **Erosion:** Removes small white noise and shrinks foreground objects.
- **Dilation:** Expands foreground objects and fills small gaps.
- **Opening:** Removes small bright noise while preserving the overall shape.
- **Closing:** Fills small dark holes and gaps.

**Additional Implementation:**
- Binary image thresholding.
- 5×5 rectangular kernel.
- RECT, ELLIPSE, and CROSS kernel comparison.
- 3×3, 5×5, and 9×9 kernel-size experiments.
- Opening and closing visualization grids.

### 2️⃣ Bitwise Operations & Image Histograms

Implemented image manipulation using binary masks.

**Bitwise Operations:**
- AND
- OR
- XOR
- NOT

**Image Histograms:**
- Grayscale histogram.
- Individual Blue, Green, and Red channel histograms.
- Brightness adjustment.
- Contrast adjustment.
- Histogram comparison before and after enhancement.

**Practical Applications:**
- Region of Interest (ROI) extraction.
- Image masking.
- Watermark overlay.
- Image intensity analysis.

### 3️⃣ Face Detection Using YuNet

Implemented pretrained YuNet face detection using OpenCV's `FaceDetectorYN` API.

**Key Features:**
- Face detection on multiple static images.
- Bounding-box visualization.
- Five facial landmark detection.
- Confidence score visualization.
- Score threshold comparison: 0.5, 0.7, and 0.9.
- Face-region Gaussian blur for privacy protection.
- Optional real-time webcam face detection.
- FPS measurement.

YuNet is a lightweight face-detection model available through the OpenCV Zoo.

### 4️⃣ Object Detection Using YOLOv8

Implemented pretrained YOLOv8 Nano (`yolov8n.pt`) for detecting everyday objects.

**Key Features:**
- Pretrained YOLOv8 model loading.
- Multiple object detection.
- Bounding boxes and class labels.
- Confidence score visualization.
- Static image detection.
- Optional real-time webcam detection.
- Confidence threshold comparison: 0.25, 0.50, and 0.75.
- IoU threshold comparison: 0.30, 0.50, and 0.70.
- Non-Maximum Suppression (NMS) analysis.
- Per-class detection summary.
- FPS measurement.

The model uses pretrained COCO weights covering 80 object categories.

### 5️⃣ Integrated Computer Vision Pipeline

Combined classical image processing and deep-learning-based detection into one pipeline.

**Implementation:**
- YuNet face detection.
- YOLOv8 object detection.
- Combined bounding-box visualization.
- Green boxes for face detection.
- Red boxes for YOLO object detection.
- Morphological pre-cleaning experiment.
- 100-frame performance benchmarking.
- FPS comparison visualization.
- Final technique comparison table.

---

## 📊 Results & Visualizations

The notebook generates multiple visualizations to understand the behaviour of each computer vision technique.

| Visualization | Description |
|---|---|
| Morphology Operations | Erosion, dilation, opening, closing |
| Kernel Comparison | Different shapes and sizes |
| Bitwise Operations | AND, OR, XOR, NOT |
| Image Histograms | Grayscale and RGB channels |
| Brightness & Contrast | Image enhancement comparison |
| YuNet Detection | Face boxes and landmarks |
| YOLO Detection | Object labels and confidence |
| Threshold Comparison | Confidence and IoU experiments |
| Per-Class Summary | Object detection counts |
| FPS Comparison | Processing performance |

All generated plots are saved in the `plots/` directory when the corresponding notebook cells execute.

---


## 📦 Dataset & Pretrained Model Sources

**Sample Images**

- OpenCV Sample Images: https://github.com/opencv/opencv/tree/master/samples/data
- Ultralytics Sample Images: https://github.com/ultralytics/assets

**Pretrained Face Detection Model**

- OpenCV Zoo – YuNet: https://github.com/opencv/opencv_zoo/tree/main/models/face_detection_yunet

**Object Detection Model**

- Ultralytics YOLOv8: https://docs.ultralytics.com/models/yolov8/

**Dataset for Object Detection**

- COCO Dataset: https://cocodataset.org/

---

## 📈 Final Learning Outcomes

After completing this project, I gained practical experience in:

- Image processing using OpenCV.
- Binary image operations and morphological transformations.
- Bitwise masking and ROI extraction.
- Image histogram analysis and enhancement.
- CNN-based face detection using YuNet.
- Deep-learning-based object detection using YOLOv8.
- Confidence threshold and IoU optimization.
- Non-Maximum Suppression concepts.
- Real-time computer vision applications.
- Performance measurement and FPS benchmarking.
- Integrating classical image processing with deep learning.

---

## 🚀 Applications

These computer vision techniques can be applied in:

- Smart surveillance systems.
- Face detection and privacy protection.
- Retail analytics.
- Object recognition systems.
- Automated monitoring.
- Traffic monitoring.
- Real-time security applications.

---

## 👨‍💻 Author

**Mant Sherasiya**

- GitHub: [@Mant-0957](https://github.com/Mant-0957)
- Project Repository: [DeepLearning_PR3](https://github.com/Mant-0957/DeepLearning_PR3)

---


<p align="center">
  <b>Learning Computer Vision | Exploring Deep Learning | Building Real-World AI Projects 🚀</b>
</p>
