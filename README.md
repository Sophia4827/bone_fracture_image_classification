# Bone Fracture Image Classification

This repo contains the code, training results, and final presentation for an image classification project that detects and classifies bone fractures in X-ray images using YOLO. The model was trained on a publicly available fracture dataset with data augmentation and transfer learning to improve generalization.

Here are the different components:

- [Classification Notebook](./Final_Project): Full pipeline including data preprocessing, annotation, model training, hyperparameter tuning, and evaluation
- [Training Results](./results.csv): Per-epoch training and validation metrics (loss, precision, recall, mAP50)
- [Final Presentation](./Final_Presentation.pdf): Project overview, methodology, and findings

## Overview

Accurate and automated fracture detection from X-rays has significant potential to support clinical decision-making. This project builds a YOLO-based object detection pipeline to classify bone fractures, evaluated using precision, recall, and mAP metrics.

- Developed an image classification pipeline using **YOLO** for X-ray bone fracture detection
- Achieved **84% precision** and **48% recall** on the test set
- Applied **data augmentation** (flipping, rotation, brightness variation) to reduce overfitting and improve generalization
- Used **transfer learning** by fine-tuning a pretrained YOLO model on fracture-specific data
- Collaborated with domain experts to validate model predictions and ensure clinically relevant classifications
- Evaluated model performance using precision, recall, F1, and mAP50

## Results

| Metric | Score |
|--------|-------|
| Precision | 84% |
| Recall | 48% |
| Model | YOLO |

Training metrics per epoch are available in [results.csv](./results.csv).

## Dataset

The bone fracture dataset is publicly available on Figshare:  
[https://figshare.com/articles/dataset/The_dataset/22363012](https://figshare.com/articles/dataset/The_dataset/22363012)

## Requirements

- Python 3.x
- Jupyter Notebook

## Dependencies

- ultralytics
- torch
- pandas
- numpy
- matplotlib
- opencv-python

## Authors

Sophia Huang · McKenzie Skrastins · Mimmy Mei · Charlotte Li  
Binghamton University MS Data Analytics · Fall 2024
