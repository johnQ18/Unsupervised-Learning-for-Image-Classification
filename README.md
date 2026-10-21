# 🖼️ Unsupervised Learning for Image Classification

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=flat&logo=PyTorch&logoColor=white)](https://pytorch.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An implementation of unsupervised learning techniques for image representation learning, clustering, and classification without relying on manual labels.

---

## 📌 Table of Contents
- [About The Project](#-about-the-project)
- [Key Features](#-key-features)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#-usage)
  - [1. Feature Extraction / Training](#1-feature-extraction--training)
  - [2. Clustering / Evaluation](#2-clustering--evaluation)
- [Results & Performance](#-results--performance)
- [Contributing](#-contributing)
- [License](#-license)

---

## 📖 About The Project
Supervised deep learning models require vast amounts of manually annotated data, which can be expensive and time-consuming to obtain. This repository explores **unsupervised and self-supervised learning** pipelines to discover meaningful patterns and representations from unlabeled image datasets, ultimately enabling effective image clustering and classification.

---

## ✨ Key Features
- **Unsupervised Feature Extraction:** Leverage architectures like Autoencoders, Convolutional Autoencoders, or self-supervised frameworks (e.g., SimCLR/BYOL) to learn rich visual embeddings.
- **Clustering Algorithms:** Apply clustering techniques (e.g., K-Means, Gaussian Mixture Models, DBSCAN) on extracted latent spaces.
- **Evaluation Metrics:** Assess clustering and classification quality using metrics such as Accuracy, Normalized Mutual Information (NMI), and Adjusted Rand Index (ARI).
- **Modular Pipeline:** Clean, structured codebase designed for easy experimentation with different datasets and models.

---

## 📂 Project Structure
```text
Unsupervised-Learning-for-Image-Classification/
│
├── data/                  # Dataset directory (ignored in git)
├── models/                # Model architectures (Autoencoders, encoders, etc.)
├── notebooks/             # Jupyter notebooks for exploratory data analysis & visualization
├── scripts/               # Training and evaluation scripts
│   ├── train.py           # Main training script
│   └── evaluate.py        # Evaluation & clustering script
│
├── utils/                 # Helper functions (preprocessing, metrics, visualization)
├── requirements.dev.txt   # Dependencies
├── .gitignore
└── README.md
