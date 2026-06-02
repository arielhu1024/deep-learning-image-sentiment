# Transfer Learning for Visual Sentiment Analysis and Social Media Engagement Prediction

This project explores how deep learning and transfer learning techniques can be used to understand visual sentiment in social media images and examine the relationship between image sentiment and user engagement.

The project was conducted as part of a graduate-level deep learning research project at the University of Arizona. It combines computer vision, transfer learning, and marketing analytics to investigate how emotional signals embedded in visual content influence audience responses on social media platforms.

---

## Overview

Visual content plays an increasingly important role in shaping user behavior online. While advances in computer vision have significantly improved image recognition, understanding the emotional meaning conveyed by images remains a challenging problem.

This project develops and evaluates several deep learning frameworks for image sentiment classification. Both binary and multi-class sentiment settings are considered, and transfer learning approaches are compared against traditional convolutional neural network architectures.

The resulting sentiment predictions are further incorporated into an engagement analysis framework to study how emotional content influences user interactions on social media.

---

## Research Questions

* Can deep learning models accurately classify image sentiment?
* How does transfer learning compare with traditional CNN architectures for sentiment prediction?
* Does image sentiment significantly affect user engagement on social media platforms?

---

## Dataset

The study uses an image sentiment dataset derived from publicly available social media image collections.

### Binary Classification

* Positive (Happy)
* Negative (Angry, Sad, Melancholic)

### Multi-Class Classification

* Happy
* Angry
* Sad
* Melancholic

The original dataset is not redistributed through this repository.

---

## Methodology

### Data Preparation

* Image preprocessing and resizing
* Data augmentation
* Train / Validation / Test split
* Class balancing

### Deep Learning Models

* AlexNet
* ResNet50 Transfer Learning

### Engagement Analysis

Predicted image sentiment scores were incorporated into downstream engagement prediction models to evaluate how emotional content influences audience interactions.

---

## Repository Structure

```text
.
├── data/
│   └── README.md
│
├── docs/
│   └── Final_Project_Report.pdf
│
├── figures/
│   ├── study_design.png
│   ├── alexnet_binary_confusion_matrix.png
│   ├── resnet_binary_confusion_matrix.png
│   ├── alexnet_multiclass_confusion_matrix.png
│   └── resnet_multiclass_confusion_matrix.png
│
├── notebooks/
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_alexnet_binary_classification.ipynb
│   ├── 03_resnet50_binary_classification.ipynb
│   ├── 04_alexnet_multiclass_classification.ipynb
│   ├── 05_resnet50_multiclass_classification.ipynb
│   ├── 06_engagement_analysis.ipynb
│   └── README.md
│
├── results/
│   ├── binary_classification_results.csv
│   ├── multiclass_classification_results.csv
│   ├── engagement_regression_results.csv
│   └── README.md
│
└── README.md
```

---

## Main Findings

### Binary Classification

| Model    | Accuracy | Macro F1 |
| -------- | -------- | -------- |
| AlexNet  | 89.71%   | 0.87     |
| ResNet50 | 85.51%   | 0.80     |

### Multi-Class Classification

| Model    | Accuracy | Macro F1 |
| -------- | -------- | -------- |
| AlexNet  | 63.97%   | 0.64     |
| ResNet50 | 68.84%   | 0.68     |

The binary sentiment framework achieved substantially stronger predictive performance and was selected for subsequent engagement analyses.

---

## Technologies

* Python
* PyTorch
* Transfer Learning
* ResNet50
* AlexNet
* OpenCV
* NumPy
* Pandas
* Scikit-learn
* Matplotlib

---

## Report

The complete project report is available in:

```text
docs/Final_Project_Report.pdf
```

---
