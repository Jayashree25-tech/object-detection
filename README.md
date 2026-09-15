## Traffic Light & Road Object Detection using YOLO11s

A computer vision object detection project built with Ultralytics **YOLO11s**, trained on a custom multi-class dataset targeting traffic lights, signals, vehicles, and road obstacles.

---

## 📌 Project Overview

This repository contains end-to-end code for dataset gathering, stratified splitting, model training with advanced augmentations, evaluation, and inference output generation using Google Colab and Ultralytics YOLO11.

---

## 🚀 Key Features

* **Multi-Class Detection:** Detects 13 custom road and traffic categories.
* **Stratified Split:** 70% Train, 20% Validation, and 10% Test split guaranteeing balanced class distribution across splits.
* **Advanced Augmentations:** Optimized training pipeline utilizing Mosaic (0.8) and MixUp (0.15) augmentations for robust feature learning.
* **YOLO Architecture:** Uses `yolo11s.pt` (YOLO11 Small) for high-accuracy, real-time object detection.

---

## 🏷️ Dataset Classes

The dataset comprises 13 distinct object categories:

| Class ID | Class Name | Class ID | Class Name |
| :---: | :--- | :---: | :--- |
| **0** | Traffic Cone | **7** | Yellow Signal |
| **1** | Obstacle | **8** | Two-Wheeler |
| **2** | Cow | **9** | Speed Limit 10 Sign |
| **3** | Pedestrian | **10** | General Traffic Sign |
| **4** | Bicycle | **11** | Speed Limit 30 Sign |
| **5** | Red Signal | **12** | Vehicle |
| **6** | Green Signal | | |

---

## 📂 Dataset & Project Directory Structure

```text
├── data_cone/
├── data_obstacle/
├── data_cow/
├── data_pedestrian/
├── data_bicycle/
├── data_red/
├── data_green/
├── data_yellow/
├── data_twowheeler/
├── data_sign10/
├── data_trafficsign/
├── data_sign30/
├── data_vehicle/
├── yolo_dataset/
│   ├── data.yaml
│   ├── images/
│   │   ├── train/
│   │   ├── val/
│   │   └── test/
│   └── labels/
│       ├── train/
│       ├── val/
│       └── test/
├── my_predictions/
│   └── light_results/
├── main_pipeline.ipynb
└── README.md
