# ⚛️ Quantum Convolutional Neural Network (QCNN) for MNIST Digit Classification

> A fully trainable Quantum Convolutional Neural Network (QCNN) implemented using PennyLane and TensorFlow for multi-class handwritten digit classification on the MNIST dataset.

![Python](https://img.shields.io/badge/Python-3.10-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![PennyLane](https://img.shields.io/badge/PennyLane-Quantum-purple)
![Quantum Computing](https://img.shields.io/badge/Quantum-ML-success)
![License](https://img.shields.io/badge/License-MIT-green)

---

# 📖 Overview

This project implements a **Quantum Convolutional Neural Network (QCNN)** for **10-class handwritten digit classification** using the MNIST dataset.

Unlike classical convolutional neural networks, the model performs feature extraction using trainable **quantum convolution** and **quantum pooling** layers. Classical image patches are encoded into quantum states through **Amplitude Embedding**, processed by variational quantum circuits, and measured to classify handwritten digits.

The model is trained end-to-end using **TensorFlow** and **PennyLane**.

---

# 🚀 Features

- ⚛️ Fully Trainable QCNN
- 🧠 Quantum Convolution Layers
- 🔄 Quantum Pooling Layers
- 🎯 Amplitude Embedding
- 🔗 Quantum Entanglement using CNOT Gates
- 📦 Variational Quantum Circuits
- 🔟 Multi-Class MNIST Classification (0–9)
- ⚡ TensorFlow + PennyLane Integration
- 💾 Checkpoint Saving & Loading
- 📝 Custom Handwritten Digit Prediction

---

# 🏗️ Model Architecture

```text
Input Image (28×28)
        │
        ▼
Resize to 8×8
        │
        ▼
Split into Four 4×4 Patches
        │
        ▼
Amplitude Embedding
        │
        ▼
Quantum Convolution Block 1
        │
        ▼
Quantum Pooling Block 1
        │
        ▼
Quantum Convolution Block 2
        │
        ▼
Expectation Value Measurements
        │
        ▼
Fully Connected Layer
        │
        ▼
10-Class Digit Prediction
```

---

# ⚛️ Quantum Circuit

Each **4×4 image patch (16 pixels)** is encoded into a **4-qubit quantum circuit** using **Amplitude Embedding**.

The QCNN consists of:

- Amplitude Embedding
- Trainable RY Gates
- Trainable RZ Gates
- CNOT Entanglement
- CRZ Pooling
- Pauli-X Operations
- Pauli-Z Expectation Measurements

All quantum parameters are optimized using TensorFlow's automatic differentiation.

---

# 📊 Dataset

**Dataset:** MNIST Handwritten Digits

- Classes: 0–9
- Original Image Size: 28×28
- Resized Image Size: 8×8
- Patch Size: 4×4
- Number of Qubits: 4

---

# 🛠️ Technologies Used

- Python
- PennyLane
- TensorFlow
- NumPy
- OpenCV
- Matplotlib
- Google Colab

---

# 📂 Repository Structure

```text
QCNN-MNIST-10Class/
│
├── QCNN_MNIST_10Class.ipynb
├── README.md
├── requirements.txt
├── LICENSE
├── .gitignore
└── images/
    ├── architecture.png
    ├── accuracy.png
    ├── loss.png
```

---

# 🔄 Workflow

1. Load the MNIST dataset
2. Normalize and resize images to 8×8
3. Split each image into four 4×4 patches
4. Encode patches using Amplitude Embedding
5. Apply Quantum Convolution Block
6. Apply Quantum Pooling Block
7. Measure quantum states
8. Concatenate quantum features
9. Train the QCNN using TensorFlow
10. Predict one of the 10 digit classes

---

# 📈 Results

The QCNN successfully learns quantum representations for handwritten digits and performs multi-class classification.

| Metric | Value |
|---------|-------|
| Training Accuracy | 64% |
| Test Accuracy | 49 % |
| Epochs | 10 |

> Replace the values with your experimental results.

---

# 📷 Results

## Training Accuracy

```markdown
![Accuracy](images/accuracy.png)
```

## Training Loss

```markdown
![Loss](images/loss.png)
```

## Confusion Matrix

```markdown
![Confusion Matrix](images/confusion_matrix.png)
```

## Sample Predictions

```markdown
![Predictions](images/predictions.png)
```

---

# 🌟 Highlights

- Fully trainable Quantum Convolutional Neural Network
- Amplitude Embedding for quantum state preparation
- Trainable quantum convolution and pooling
- Multi-class handwritten digit classification
- TensorFlow backpropagation through quantum circuits
- Checkpoint saving and recovery
- Custom handwritten digit prediction pipeline

---

# 🔮 Future Work

- Increase the number of qubits
- Deeper QCNN architectures
- Hyperparameter optimization
- Evaluation on real quantum hardware
- Fashion-MNIST classification
- CIFAR-10 quantum image classification

---

# 📚 References

- Cong, Choi & Lukin (2019) – *Quantum Convolutional Neural Networks*
- PennyLane Documentation
- TensorFlow Documentation

---

# 👩‍💻 Author

**Prakriti**

B.Tech – Computer Science Engineering

**Research Interests**

- Quantum Machine Learning
- Quantum Computing
- Deep Learning
- Artificial Intelligence
- Computer Vision

---

# ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.
