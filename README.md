# Fashion MNIST Neural Network — From Scratch

A fully-connected neural network trained on the [Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist) dataset, implemented from scratch using only NumPy. No PyTorch. No TensorFlow. Every forward pass, activation, and backpropagation step is written by hand.

---

## Overview

This project builds a multi-layer perceptron (MLP) from the ground up to classify 10 categories of clothing and accessories. The goal was to develop deep intuition for how neural networks actually work gradients, weight updates, and all rather than relying on autograd frameworks to abstract it away.

**Dataset:** Fashion MNIST — 70,000 grayscale 28×28 images across 10 classes  
**Framework:** Pure NumPy  
**Accuracy:** 70~75% on the test set

---

## What's Implemented

- **Forward pass**: linear layers with manual matrix multiplication
- **Activation functions**: ReLU (hidden layers), Softmax (output layer)
- **Loss function**: Cross-entropy loss
- **Backpropagation**: full gradient computation by hand
- **Parameter updates**: gradient descent with configurable learning rate
- **Data preprocessing**: normalization and one-hot encoding

---

## Architecture

```
Input (784)  →  Dense (128, ReLU)  →  Dense (64, ReLU)  →  Output (10, Softmax)
```

---

## Getting Started

**Requirements**
```
numpy
pandas
matplotlib
```

Install with:
```bash
pip install numpy pandas matplotlib
```

**Run**

Open `Fashion_MNIST_classifier_from_scratch.ipynb` in Jupyter and run all cells. The dataset is loaded directly from the Kaggle CSV format — download it [here](https://www.kaggle.com/datasets/zalando-research/fashionmnist).

---

## Classes

| Label | Class |
|-------|-------|
| 0 | T-shirt/top |
| 1 | Trouser |
| 2 | Pullover |
| 3 | Dress |
| 4 | Coat |
| 5 | Sandal |
| 6 | Shirt |
| 7 | Sneaker |
| 8 | Bag |
| 9 | Ankle boot |

---

## References

- [Neural Networks from Scratch — Samson Zhang](https://www.youtube.com/watch?v=w8yWXqWQYmU)
- [Simple MNIST NN from Scratch (NumPy)](https://www.kaggle.com/code/wwsalmon/simple-mnist-nn-from-scratch-numpy-no-tf-keras)
- [Fashion MNIST Dataset — Zalando Research](https://www.kaggle.com/datasets/zalando-research/fashionmnist)
- [Fashion MNIST Paper — Xiao et al., 2017](https://arxiv.org/pdf/1802.01528)
- [Neural Networks and Deep Learning — Michael Nielsen](http://neuralnetworksanddeeplearning.com/index.html)
- [An Introduction to Deep Learning — Guilhoto](https://math.uchicago.edu/~may/REU2018/REUPapers/Guilhoto.pdf)
