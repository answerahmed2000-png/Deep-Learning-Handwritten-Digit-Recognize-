# Deep-Learning-Handwritten-Digit-Recognize-
# 🧠 CNN MNIST Classification Project (with BatchNorm + Early Stopping)

## 📌 Project Overview
This project implements a Convolutional Neural Network (CNN) using PyTorch to classify handwritten digits from the MNIST dataset (0–9).

The model includes:
- Convolutional Neural Network (CNN)
- Batch Normalization
- Dropout Regularization
- Early Stopping
- Comparison between Adam and SGD optimizers
- Training vs Validation evaluation
- Visualization of results

---

## 📊 Dataset
- Dataset: MNIST
- Classes: 10 (digits 0–9)
- Image size: 28×28 grayscale images

---

## 🏗️ Model Architecture

The CNN consists of:

- Conv Layer 1: 1 → 16 filters (3×3)
- Batch Normalization
- ReLU Activation
- MaxPooling (2×2)

- Conv Layer 2: 16 → 32 filters (3×3)
- Batch Normalization
- ReLU Activation
- MaxPooling (2×2)

- Fully Connected Layer: 32×5×5 → 128 neurons
- Dropout (0.5)
- Output Layer: 128 → 10 classes

---

## ⚙️ Training Details

- Loss Function: CrossEntropyLoss
- Optimizers:
  - Adam (lr = 0.001)
  - SGD (lr = 0.01)
- Batch Size: 64
- Epochs: up to 10
- Early Stopping: patience = 2

---

## 🔁 Training Process

Each training step includes:
1. Forward pass
2. Loss calculation
3. Backpropagation
4. Optimizer update

Validation is performed after each epoch to monitor performance.

---

## 🛑 Early Stopping

Training stops automatically if validation loss does not improve for 2 consecutive epochs to prevent overfitting.

---

## 📈 Evaluation Metrics

The model is evaluated using:
- Accuracy (% correct predictions)
- Loss (error measurement)

Both training and validation results are recorded.

---

## 📊 Visualization

The project includes:
- Accuracy comparison between Adam and SGD
- Loss comparison between Adam and SGD

---

## 🧪 Results

Final results are displayed in a table comparing:
- Training Accuracy
- Validation Accuracy
- Training Loss
- Validation Loss

---

## 🚀 How to Run

### 1. Install dependencies
```bash
pip install torch torchvision matplotlib pandas
