# A.I Practice Codes

This repository contains practice code for various AI models. It features a collection of AI projects implemented in Python and Jupyter Notebooks, showcasing fundamental and advanced concepts such as perceptrons, neural networks, regression analysis, and transformers.

## Table of Contents

- [1. AND Gate Simulation](#1-and-gate-simulation)
- [2. California Housing Price Prediction using Linear Regression](#2-california-housing-price-prediction-using-linear-regression)
- [3. Multi-Layer Perceptron](#3-multi-layer-perceptron)
- [4. The Perceptron](#4-the-perceptron)
- [5. The VGG16 Model](#5-the-vgg16-model)
- [6. Video Classification Transformer](#6-video-classification-transformer)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Overview

### 1. AND Gate Simulation

This project simulates the operation of a basic AND gate using Python. It demonstrates how a simple neural network can be trained to mimic the logic of an AND gate. The project covers:

- Implementing a simple perceptron.
- Training the perceptron to learn the AND logic.
- Evaluating the model’s performance.

**Files:**
- [AND Gate Readme.md](./AND%20Gate%20Readme.md)
- [The Perceptron (DL).ipynb](./The%20Perceptron%20(DL).ipynb)

---

### 2. California Housing Price Prediction using Linear Regression

This project uses the California Housing dataset to predict housing prices based on various features such as median income, house age, and more. A linear regression model is trained and evaluated using performance metrics like Mean Squared Error (MSE) and R² score.

**Files:**
- [California Housing Price Prediction using Linear Regression Readme.md](./California%20Housing%20Price%20Prediction%20using%20Linear%20Regression%20Readme.md)
- [Code LR California Housing Price.ipynb](./Code%20LR%20California%20Housing%20Price.ipynb)

---

### 3. Multi-Layer Perceptron

This project demonstrates the implementation of a multi-layer perceptron (MLP) using Python. The MLP is trained on a dataset to perform classification tasks. The project illustrates:

- Building a feedforward neural network.
- Training the network using backpropagation.
- Assessing the model’s accuracy and performance.

**Files:**
- [Multi-Layer Perceptron ReadMe.md](./Multi-Layer%20Perceptron%20ReadMe.md)
- [Multi-Layer Perceptron.ipynb](./Multi-Layer%20Perceptron.ipynb)

---

### 4. The Perceptron

This project focuses on the implementation of a single-layer perceptron for binary classification. It includes:

- Understanding the perceptron algorithm.
- Training the perceptron on a dataset.
- Visualizing the decision boundary and evaluating the model’s performance.

**Files:**
- [The Perceptron Readme.md](./The%20Perceptron%20Readme.md)
- [The Perceptron (DL).ipynb](./The%20Perceptron%20(DL).ipynb)

---

### 5. The VGG16 Model

This project implements the VGG16 convolutional neural network architecture, a deep learning model widely used for image classification tasks. The implementation follows the original VGG16 paper, comprising 13 convolutional layers and 3 fully connected layers.

Key features of the project include:

- Implementation of convolutional blocks with ReLU activations.
- Pooling layers to reduce the spatial dimensions of the feature maps.
- Fully connected layers for feature extraction and classification.
- Support for customizing the number of classes in the output.

**Files:**
- [VGG16 Implementation](VGG16_model_1.ipynb)

---

### 6. Video Classification Transformer

This project adapts the Video Vision Transformer (ViViT) for sports action recognition tasks. The ViViT architecture processes video data by splitting frames into patches and applying a transformer encoder for spatiotemporal feature extraction.

Key features include:

- Preprocessing video data into patch embeddings.
- Implementation of self-attention for spatiotemporal modeling.
- Fine-tuning ViViT for sports action datasets.
- Evaluating performance using classification metrics.

**Files:**
- [ViViT_Transformer.ipynb](Video_Classification_with_Transformers.ipynb)

---

## Installation

To run these projects, clone the repository and install the required dependencies:

```bash
git clone https://github.com/TitoLanna/A.I-Practice-codes-/tree/main
cd A.I-Practice-codes-
pip install -r requirements.txt
