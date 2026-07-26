# ECG Signal Analysis with Unsupervised Learning

> An unsupervised machine learning framework for ECG denoising, feature extraction, and arrhythmia visualization.

## Overview

This project presents an end-to-end unsupervised learning pipeline for electrocardiogram (ECG) signal analysis using the MIT-BIH Arrhythmia Database.

The framework combines signal processing and deep learning techniques to remove noise, identify informative frequency bands, learn compact latent representations, and visualize abnormal heartbeat distributions without supervised classification.

---

## Pipeline

```
MIT-BIH ECG
      │
      ▼
 ICA Denoising
      │
      ▼
 Frequency Analysis (PCA)
      │
      ▼
 Convolutional Autoencoder
      │
      ▼
 GHA Latent Feature Ranking
      │
      ▼
 t-SNE Visualization
      │
      ▼
 Arrhythmia Clustering
```

---

## Features

- ECG denoising using Independent Component Analysis (ICA)
- Frequency band analysis using Principal Component Analysis (PCA)
- Feature learning with Convolutional Autoencoder (CAE)
- Latent feature ranking via GHA regularization
- Two-dimensional visualization using t-SNE
- Unsupervised separation of abnormal heartbeat patterns

---

## Dataset

**MIT-BIH Arrhythmia Database**

- 48 ECG recordings
- 110,000+ annotated heartbeats
- Five heartbeat categories
- Sampling frequency: 360 Hz

---

## Results

- ECG dimension reduced from **187 → 32 → 2**
- Improved separation of abnormal heartbeat types
- Calinski-Harabasz Index improved from **443.35** to **527.14**
- Demonstrated effective unsupervised feature learning for ECG representation

---

## Tech Stack

- Python
- PyTorch
- NumPy
- Scikit-learn
- Matplotlib

---

## Citation

If you use this project in your research, please cite the corresponding report or repository.
