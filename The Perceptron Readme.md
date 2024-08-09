
# Perceptron Classifier with NumPy

This repository contains a simple implementation of a Perceptron Classifier using NumPy. The Perceptron is a basic binary classifier, ideal for understanding the foundations of neural networks.

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project demonstrates a Perceptron model trained on a synthetic dataset. The data is generated and visualized using `matplotlib`, and the Perceptron is implemented from scratch with `NumPy`.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/TitoLanna/A.I-Practice-codes-/blob/main/The%20Perceptron%20(DL).ipynb
    ```
2. Navigate to the project directory:
    ```bash
    cd perceptron-numpy
    ```
3. Install the required dependencies:
    ```bash
    pip install numpy matplotlib
    ```

## Usage

You can run the script to train the Perceptron model on the synthetic dataset and view the results:
```bash
python perceptron.py
```

## Code Explanation

### Data Generation

The script starts by generating a simple dataset:

- Two features `x1` and `x2` are initialized as arrays.
- Labels `y` are also created as an array.
- The data is repeated and random noise is added to create a more realistic dataset.

### Shuffling and Splitting Data

The data is shuffled using a pseudo-random number generator to ensure randomness. It is then split into training and testing datasets.

### Normalization

The features are normalized (zero mean, unit variance) to improve the training process.

### Perceptron Implementation

The `Perceptron` class is implemented with the following methods:

- `__init__`: Initializes the weights and bias.
- `forward`: Computes the linear combination and applies a step function to make predictions.
- `backward`: Calculates errors between predictions and actual labels.
- `train`: Trains the model using the Perceptron learning rule.
- `evaluate`: Evaluates the model's accuracy on a given dataset.

### Training and Evaluation

The model is trained on the training dataset and the final model parameters (weights and bias) are printed.

## Results

After training, the model’s weights and bias are outputted. The accuracy of the model can be evaluated on a test dataset.

```python
Model parameters: 
Weights: [[0.88756605]
 [1.83900746]]
Bias [0]
```

