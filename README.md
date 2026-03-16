# Coral Reef Health Classification

YOLOv8 + EfficientNetB0 deep learning model to classify coral reef 
health from images — trained using transfer learning and fine-tuning.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mdrizvi-106/coral-reef-classification/blob/main/Coral_Reef_Health_Classification.ipynb)

## Problem
Coral reef health is difficult to monitor at scale manually. 
This model automates classification from image data, enabling 
low-cost reef health monitoring pipelines.

## Data
- ~1,000 labelled images across 3 classes: **healthy, bleached, dead**
- Source: Kaggle (aneeshdighe)

## Method
- Backbone: EfficientNetB0 (ImageNet pretrained) — transfer learning → fine-tuning
- Framework: YOLOv8
- Image augmentation to address class imbalance
- Two-stage training: frozen backbone first, then full fine-tuning

## Results
- **80–90% classification accuracy** across all 3 categories

## Business Relevance
Accuracy at this level indicates viability for automated reef health 
monitoring pipelines — a scalable, low-cost alternative to manual 
field surveys. Applicable to environmental monitoring, conservation 
NGOs, and marine research institutions.

## Tech Stack
Python · YOLOv8 · EfficientNetB0 · Keras · Kaggle API · Google Colab
