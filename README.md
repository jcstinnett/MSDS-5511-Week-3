# MSDS-5511 Week 3: Histopathologic Cancer Detection
Kaggle Competition Histopathologic Cancer Detection

## Overview
This project uses deep learning techniques to identify cancerous tissue in histopathologic images as 
part of a Kaggle competition.

## Dataset
- Source: [Kaggle Competition](https://www.kaggle.com/competitions/histopathologic-cancer-detection)
- The dataset includes:
  - 220,025 `.tif` training images
  - 57,458 `.tif` testing images
  - A CSV file mapping image IDs to binary labels:
    - `0` = no cancer
    - `1` = cancer
  - A sample submission file for formatting test predictions
    
## Approach
- Conducted exploratory data analysis (EDA).
- Trained CNNs using ResNet50 and InceptionV3 architectures.
- Compared model performance using AUC, the official competition metric.

## Requirements
- Python 3.x
- TensorFlow / Keras
- Google Colab (recommended)
- `kaggle.json` file (for dataset access if using Kaggle API)

## How to Run
1. Upload `kaggle.json` manually in Colab
2. Run the notebook step-by-step
3. Fine-tune model and export predictions

## Results
- **ResNet50**: AUC = 0.8646 (after fine-tuning)
- **InceptionV3**: AUC = 0.9165 (no fine-tuning applied)
- InceptionV3 outperformed ResNet50 in this instance, even without additional tuning.








