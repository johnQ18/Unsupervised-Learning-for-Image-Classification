# 🖼️ Unsupervised Learning for Image Classification

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=flat&logo=PyTorch&logoColor=white)](https://pytorch.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An implementation of unsupervised and self-supervised learning pipelines for feature extraction, representation learning, and image clustering on standard vision datasets (e.g., MNIST, CIFAR-10).

---

## 📋 Table of Contents
- [Overview](#-overview)
- [Architecture & Approach](#-architecture--approach)
- [Project Structure](#-project-structure)
- [Environment Setup](#-environment-setup)
- [Execution Instructions](#-execution-instructions)
- [Evaluation & Metrics](#-evaluation--metrics)
- [Assumptions & Limitations](#-assumptions--limitations)

---

## 🔍 Overview
Supervised deep learning relies heavily on large-scale human-annotated datasets, which are often unavailable or prohibitively expensive in real-world domains. This project explores **unsupervised representation learning** to extract semantic visual features without manual labels, enabling downstream clustering and classification.

---

## 🏗️ Architecture & Approach

The pipeline consists of two primary phases:
1. **Unsupervised Feature Extraction:** 
   - Uses a Convolutional Autoencoder (or a self-supervised backbone like SimCLR) to project high-dimensional image inputs into a compact, low-dimensional latent embedding space.
   - Optimized via reconstruction loss (e.g., Mean Squared Error / Binary Cross-Entropy) or contrastive loss functions.
2. **Unsupervised Clustering & Evaluation:**
   - Applies clustering algorithms (e.g., K-Means, Gaussian Mixture Models) directly onto the extracted latent embeddings.
   - Evaluates cluster alignment against ground-truth class labels using unsupervised metrics.

---

## 📂 Project Structure

```text
Unsupervised-Learning-for-Image-Classification/
│
├── data/                  # Dataset directory (automatically downloaded if missing)
├── models/                # Network architectures (Encoder, Decoder, Autoencoder)
├── scripts/               # Executable entrypoints
│   ├── train.py           # Trains the unsupervised feature extractor
│   └── evaluate.py        # Generates embeddings and runs clustering evaluation
├── utils/                 # Helper utilities (preprocessing, metrics, visualization)
├── requirements.txt       # Python dependencies
└── README.md

´´´´
---
## ⚙️ Environment Setup

### Prerequisites
- Python 3.8 or higher
- CUDA-compatible GPU (recommended for training efficiency)

### Installation Steps

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/johnQ18/Unsupervised-Learning-for-Image-Classification.git](https://github.com/johnQ18/Unsupervised-Learning-for-Image-Classification.git)
   cd Unsupervised-Learning-for-Image-Classification

---
