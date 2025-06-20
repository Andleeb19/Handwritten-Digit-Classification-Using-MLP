# Handwritten Digit Classification Using MLP

This project implements a Multilayer Perceptron (MLP) from scratch using TensorFlow/Keras to classify handwritten digits (0–9) from the MNIST dataset.

## 📌 Problem Statement

Train an MLP to classify grayscale images of handwritten digits from the MNIST dataset.

- **Dataset:** MNIST (28x28 grayscale images)
- **Task:** Image classification (10 classes: digits 0–9)
- **Framework:** TensorFlow/Keras

## 🚀 Objectives

- Flatten the 28x28 pixel images into 784-dimensional input vectors.
- Build a deep MLP with:
  - 2–4 hidden layers
  - ReLU activation functions
  - Softmax output layer (10 neurons for 10 digit classes)
- Train using:
  - Cross-entropy loss
  - Adam optimizer
- Evaluate using:
  - Accuracy vs. Epochs plot
  - Confusion Matrix
  - Classification Report
  - Sample predictions

## 📁 Files

- `mnist_mlp.py` - Main code file to run the model.
- `report.md` - Technical report of the experiment.
- `README.md` - This file.

## 📊 Results

- **Test Accuracy:** ~97.5%
- High performance across all digit classes (precision/recall ~0.98)
- Clear separation in the confusion matrix

## 🧠 Model Architecture

- **Input Layer:** 784 (flattened from 28x28)
- **Hidden Layers:**
  - Dense(256, ReLU)
  - Dense(128, ReLU)
  - Dense(64, ReLU)
- **Output Layer:** Dense(10, Softmax)

## 📈 Visualization

- Accuracy over Epochs
- Confusion Matrix (heatmap)
- Sample Predictions

## 🔧 Installation

```bash
pip install tensorflow matplotlib seaborn scikit-learn
🧪 Run the Model
bash
Copy
Edit
python mnist_mlp.py
📌 Dataset
Available via Keras: from tensorflow.keras.datasets import mnist
