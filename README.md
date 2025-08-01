# 📡 Network Anomaly Detection System

An advanced machine learning-based system that identifies anomalies in network traffic. Built for cybersecurity applications, this project combines unsupervised and supervised ML techniques to detect suspicious behavior in real-world network data.

---

## 📌 Table of Contents
- [Overview](#overview)
- [Tech Stack & Libraries](#tech-stack--libraries)
- [Features](#features)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Visualizations](#visualizations)
- [Deployment](#deployment)
- [License](#license)

---

## 🧠 Overview

This system leverages a hybrid approach to network anomaly detection, using:
- **DBSCAN** for unsupervised anomaly detection
- **KNN** for similarity-based filtering
- **Random Forest** for classification of traffic
- **PCA** for dimensionality reduction

Real-world network data was used to train and evaluate the model with a focus on detecting malicious or suspicious packets.

---

## 🛠️ Tech Stack & Libraries

- **Languages**: Python
- **ML Algorithms**: DBSCAN, KNN, Random Forest, PCA
- **Libraries**: 
  - `scikit-learn`
  - `pandas`, `numpy`
  - `matplotlib`, `seaborn` (for visualization)
- **Environment**: Jupyter Notebook
- **Platform**: Kaggle

---

## 🚀 Features

- 📊 **Unsupervised Anomaly Detection**: DBSCAN to detect clusters of suspicious traffic
- 🔁 **Pattern Similarity**: KNN used to flag packets with high deviation
- 🌲 **Traffic Classification**: Random Forest for multi-class prediction
- 📉 **Dimensionality Reduction**: PCA used to remove noise and redundancy
- 🎯 **Accuracy**: Achieved 97.2% with 10-fold cross-validation
- 📈 **Visual Analytics**: Used Seaborn and Matplotlib for clear network insights

---

## 📈 Results

- **Accuracy**: 97.2%
- **Precision**: High
- **Recall**: High
- **F1 Score**: High
- Used real-world network traffic datasets to train and validate

---

## 💻 Installation

```bash
git clone https://github.com/your-username/network-anomaly-detection.git
cd network-anomaly-detection
pip install -r requirements.txt
