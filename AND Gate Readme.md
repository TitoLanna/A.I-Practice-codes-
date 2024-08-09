
# Simple Perceptron Logic Gate Implementation

This repository contains a basic implementation of a Perceptron-based logic gate in Python. The logic gate is designed to mimic the behavior of an AND gate, where the Perceptron is manually configured with specific weights and bias.

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project demonstrates a simple Perceptron model that performs binary classification, specifically simulating an AND logic gate. The implementation manually sets the weights and bias and evaluates the model’s performance on a small set of binary inputs.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/TitoLanna/A.I-Practice-codes-/blob/main/AND%20Gate%20-%20U15.ipynb
    ```
2. Navigate to the project directory:
    ```bash
    cd perceptron-logic-gate
    ```
3. Install the required dependencies:
    ```bash
    pip install pandas
    ```

## Usage

You can run the script to see the Perceptron in action and print out the results:
```bash
python perceptron_logic_gate.py
```

## Code Explanation

### Perceptron Weights and Bias

- `w1`, `w2`: Weights for the two inputs of the Perceptron, both set to `1`.
- `b`: Bias term, set to `-1.5` to correctly simulate an AND gate.

### Inputs and Correct Outputs

- `inputs`: A list of tuples representing all possible binary input combinations for a 2-input logic gate.
- `correct_outputs`: The expected output for each input pair, matching the behavior of an AND gate.

### Forward Pass and Output Calculation

The Perceptron calculates the output for each input pair by applying the weights and bias:
- `z = input[0]*w1 + input[1]*w2 + b`
- The output is determined by whether `z` is greater than or equal to `0`.

### Results Compilation

The script creates a list of outputs that includes:
- Input values
- Calculated `z` value
- Output prediction
- Whether the prediction was correct or not

### Displaying the Results

The results are displayed in a table format using `pandas.DataFrame` and printed to the console.

## Results

After running the script, the output should indicate whether all predictions are correct. For an AND gate, with the given weights and bias, the output should be as follows:

```python
All correct
 Input 1  Input 2    z  Out Is Correct?
       0        0 -1.5    0         Yes
       0        1 -0.5    0         Yes
       1        0 -0.5    0         Yes
       1        1  0.5    1         Yes
```

