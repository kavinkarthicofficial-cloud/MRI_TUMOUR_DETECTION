# 🧠 MRI Brain Tumor Detection using CNN

A deep learning–based system for detecting brain tumors from MRI images using Convolutional Neural Networks (CNN).  
The project focuses on accurate classification of MRI scans into tumor and non-tumor (or multi-class tumor types) using medical imaging datasets.

---

## 📌 Problem Statement

Brain tumor diagnosis using MRI scans is time-consuming and requires expert radiologists.  
This project aims to assist medical professionals by providing an automated system that can:

- Analyze MRI images
- Detect presence of tumor
- Classify tumor categories (if multi-class)

---

## 🎯 Objectives

- Preprocess and normalize MRI images
- Train a CNN model for tumor detection
- Evaluate performance using medical metrics
- Visualize predictions and confidence scores

---

## 📊 Dataset

Datasets used:
- 🧠 **BraTS (Brain Tumor Segmentation Dataset)**
- 📁 Kaggle MRI Brain Tumor Dataset

### Dataset Characteristics
- MRI modalities: T1, T2, FLAIR (depending on dataset)
- Image format: `.jpg` / `.png` / medical slices
- Classes:
  - Tumor
  - No Tumor  
  *(or multi-class: Glioma, Meningioma, Pituitary)*

---

## 🧠 Methodology

### 1. Data Preprocessing
- Image resizing to fixed dimensions
- Pixel normalization (0–1 scaling)
- Noise reduction
- Data augmentation:
  - Rotation
  - Flipping
  - Zoom

### 2. CNN Architecture

Typical layers used:
- Convolution Layers (ReLU)
- Max Pooling
- Dropout (to prevent overfitting)
- Fully Connected Dense Layers
- Softmax / Sigmoid Output Layer

Architecture optimized for:
- Small medical datasets
- High generalization

---

## ⚙️ Training Details

- Framework: TensorFlow / PyTorch
- Loss Function: Binary Cross-Entropy / Categorical Cross-Entropy
- Optimizer: Adam
- Batch Size: 16 / 32
- Epochs: 20–50

---

## 📈 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

These metrics help ensure:
- Low false negatives (important in medical diagnosis)
- Stable generalization across unseen MRI scans

---

## 🖥️ System Architecture

