# Neural Network Approximation using TensorFlow and Keras
## Introduction
This repository contains the implementation of a Neural Network using TensorFlow and Keras to approximate a target function. The target function to be approximated is given by:

f(x) = sin(x) * sin(0.4 * x) * sin(2 * x)

The network architecture and training parameters have been carefully chosen and experimented with to closely approximate the target function.

## Files Included
train.csv: This file contains 10,000 comma-separated examples. Each example consists of an x value (ranging from 0 to 10) and the corresponding y value generated by the target function.
eval.csv: This file contains 300 randomly generated x values (ranging from 0 to 10) along with their corresponding target (expected) y values.
train.ipynb: A Jupyter notebook containing template code for network training.
evaluate.ipynb: A Jupyter notebook containing code for evaluating the trained network.

## Network Architecture
The network architecture consists of one input layer and one output layer. As the target function generates a y value for each x value, the network has one input and one output. To capture the non-linearities of the target function, ReLU activation functions are used for the hidden layers. The output layer has no activation function, ensuring a linear output.

## Experimentation
To produce a trained model that closely approximates the target function, the following network parameters were experimented with:

Number of hidden layers and number of nodes on each layer
Choice of optimizer (SGD or Adam)
Learning rate
Momentum term (SGD only)
Number of training epochs
The weights of the network vary with different parameters and optimization algorithms. Therefore, the average network accuracy over several training runs (~10) was calculated.
