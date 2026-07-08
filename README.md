# 🌍 Planetary Rockfall Detection using Deep Learning

A deep learning-based computer vision project for automated rockfall detection on high-resolution satellite imagery of **Mars** and the **Moon** using Convolutional Neural Networks (CNNs).

This project was developed to investigate the application of deep learning for planetary surface analysis by identifying and classifying rockfall regions from orbital imagery. Automated rockfall detection can support geological studies, planetary exploration, and reduce the effort required for manual image inspection.

---

## 📖 Project Overview

Planetary rockfall detection is a challenging computer vision task due to the small size of rockfall features and the large volume of satellite imagery that must be analyzed.

In this project, a deep learning pipeline was developed to automatically identify rockfall regions on high-resolution images of the Moon and Mars. The workflow includes image preprocessing, data augmentation, CNN-based model training, and performance evaluation on two planetary datasets.

The project demonstrates how deep learning techniques can be applied to planetary science for automated geological feature detection, reducing manual effort while enabling scalable analysis of planetary surfaces.

---

## 🎯 Objectives

- Detect rockfall regions from planetary satellite images.
- Develop a complete preprocessing pipeline for image preparation.
- Train and evaluate a CNN model for rockfall classification.
- Compare model performance on Mars and Moon datasets.

---
## 📂 Dataset

This project uses the **RMaM-2020 (Rockfall Mars Moon 2020)** dataset, a publicly available benchmark dataset for automated rockfall detection in planetary satellite imagery.

The dataset consists of high-resolution orbital images from **Mars** and the **Moon**, with manually annotated rockfall regions. It was developed to support research in deep learning-based rockfall detection and planetary surface analysis.

### Why Rockfall Detection?

Rockfalls are geological features formed when large rocks move down a slope due to events such as impacts, moonquakes, marsquakes, or erosion. From satellite imagery, they appear as a combination of a displaced boulder and the track left behind during its movement.

Automatically detecting these features is important because it helps researchers:

- Understand planetary surface evolution
- Study erosion and geological activity
- Estimate surface properties remotely
- Support future robotic and human exploration missions
- Reduce the need for time-consuming manual image inspection

### Dataset Characteristics

- 🌕 Moon and 🔴 Mars imagery
- **2,822 manually labelled rockfall instances**
- Balanced across different terrains, illumination conditions, and spatial resolutions
- Designed specifically for deep learning and computer vision applications

### Preprocessing

Before training, the following preprocessing steps were applied:

- Image resizing
- Duplicate image handling
- Missing value removal
- Bounding box generation
- Coordinate normalization
- Gaussian blur for noise reduction
- Data augmentation

### Dataset Sources

- Mars Dataset (Kaggle)
- Moon Dataset (Kaggle)

The original RMaM-2020 dataset was introduced by Bickel et al. for deep learning-based planetary rockfall detection.
---

## 🏗️ Project Pipeline

```
Satellite Images
        │
        ▼
Image Preprocessing
        │
        ▼
Bounding Box Generation
        │
        ▼
Data Augmentation
        │
        ▼
CNN Model Training
        │
        ▼
Prediction
        │
        ▼
Performance Evaluation
```

---

## 🛠️ Tech Stack

- Python
- TensorFlow
- NumPy
- Pandas
- OpenCV
- Matplotlib
- Google Colab
- Kaggle

---

## 🧠 Model

A Sequential Convolutional Neural Network (CNN) was implemented using TensorFlow for binary rockfall classification.

The workflow consists of:

- Image preprocessing
- Dataset preparation
- CNN training
- Model evaluation
- Prediction on unseen images

The Sequential CNN architecture was selected after experimentation and achieved better performance than the VGG16 baseline for this dataset.

---

## 📊 Results

| Dataset | Accuracy |
|----------|----------|
| 🌕 Moon | **94.00%** |
| 🔴 Mars | **80.13%** |

The model demonstrated strong performance on Moon imagery and achieved satisfactory results on the more challenging Mars dataset.

---

## 📁 Repository Structure

```
planetary-rockfall-detection/
│
├── notebooks/
├── src/
├── data/
├── models/
├── results/
├── images/
├── README.md
├── requirements.txt
└── LICENSE
```

---

## 🚀 Future Improvements

Possible extensions include:

- Transfer Learning using EfficientNet or ResNet
- YOLO-based object detection
- Vision Transformers (ViT)
- Semantic segmentation with U-Net
- Hyperparameter optimization
- Model deployment using FastAPI
- Docker containerization

---

## 📚 References

- Bickel et al., *Deep Learning-Driven Detection and Mapping of Rockfalls on Mars*, IEEE JSTARS, 2020.
- Bickel et al., *A Labelled Image Dataset for Deep Learning-Driven Rockfall Detection on the Moon and Mars*, Frontiers in Remote Sensing, 2021.

---

## 👩‍💻 Author

**Sakshi Singh**

M.Sc. Computer Science  
Paderborn University, Germany

**Areas of Interest**

- Machine Learning
- Computer Vision
- Data Science
- Data Engineering
- Trustworthy AI
