---
title: "Machine Learning for Atmospheric Blocking Detection"
summary: "Bachelor thesis evaluating the potential for supervised learning in the detection of atmospheric blocking events in satellite data. Train and fine-tune multiple different architectures and conduct a large-scale hyperparameter search to establish the new SOTA in blocking detection accuracy."
date: 2024-07-26
tags: ["CNN", "Cloud", "Machine Learning", "Research"]
image: "path/to/atmospheric-blocking-image.png"
grade: "4.0 GPA (Equivalent German 1.0)"
---

Bachelor thesis is available here [bachelor-thesis.pdf](/projects/bachelor/machine-learning-atmospheric-blocking-tobias-leibrock.pdf)


---

![Bachelor Transfer Learning](/projects/bachelor/transfer-learning.png)

## About the Thesis

Blocking events are a major indicator for extreme weather events such as droughts or heat waves, which involves huge humanitarian and economical damages. To increase state-of-the-art detection accuracy this thesis aims at evaluating the detection of atmospheric blocking events using supervised learning algorithms, specifically random forest classification and convolutional neural networks.

Using multiple data preprocessing and augmentation steps this thesis successfully demonstrates the potential for future research and applications into the detection of atmospheric blocking events on multiple meteorological variables including geopotential height and mean sea level pressure. The thesis also proposes a new architecture aimed at integrating detection methods easier and faster into applications.

---

# Technologies Used
- Convolutional Neural Networks (CNN) + Random Forest Classification
- Propulate (Large Scale Hyperparameter Search)
- Pytorch
- Data Augmentation ([Albumentations](https://albumentations.ai/))
- Satellite Data ERA5 + UKESM
- Compute Cluster & AI Training at Scale

---

![bachelor-thesis-performance.png](/projects/bachelor/bachelor-thesis-performance.png)

![cv-setup.png](/projects/bachelor/cv-setup.png)