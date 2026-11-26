# Experiment 5 : Multilayer Perceptron (MLP) Neural Network

## Aim

To implement a Multilayer Perceptron (MLP) neural network for
handwritten digit classification using Python and evaluate its
performance on the test dataset.

> **Note:** The source page contains an inconsistent aim statement
> mentioning K-Means clustering. The experiment title and algorithm
> steps describe an MLP neural network, so this README follows the MLP
> experiment.

## Overview

A **Multilayer Perceptron (MLP)** is a feed-forward artificial neural
network consisting of an input layer, one or more hidden layers, and an
output layer. It learns patterns in data by adjusting weights and biases
during training using backpropagation.

In this experiment, the MLP model is trained on the **Digits dataset**
available in scikit-learn. Each sample is an 8 × 8 image of a
handwritten digit (0--9). The pixel values are used as input features,
and the model predicts the corresponding digit.

## Algorithm

1.  **Start.**
2.  Load the Digits dataset and separate the input features and target
    labels.
3.  Split the dataset into training and testing sets.
4.  Standardize the input features.
5.  Create an MLP classifier with the specified hidden-layer structure.
6.  Train the model using the training data.
7.  Predict the labels for the test data.
8.  Evaluate the model using test accuracy and a classification report.
9.  Plot the training loss curve.
10. **Stop.**
ry slightly with changes to the train-test split,
    random seed, or model parameters.


## Program
import numpy as np

import pandas as pd

import matplotlib.pyplot as plt

from statsmodels.tsa.arima.model import ARIMA

from statsmodels.tsa.stattools import adfuller

#(Reusing the synthetic series from previous experiment)

np.random.seed(42)

periods = 120

time = pd.date_range(start='2015-01-01', periods=periods,

freq='M')

trend = np.linspace(10, 50, periods)

seasonal=5* np.sin(2* np.pi* time.month/12)

noise = np.random.normal(0, 2, periods)

series = pd.Series(trend + seasonal + noise, index=time)

# Difference once to remove trend (d=1)




## output



## Result

