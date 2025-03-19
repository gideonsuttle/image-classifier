# Fashion MNIST Classifier

A deep learning model built with TensorFlow that classifies fashion items (clothing, accessories) using both simple neural networks and CNN architectures, trained on the Fashion MNIST dataset.

## Project Overview

This project implements two different neural network architectures to classify fashion items:
1. A simple feedforward neural network
2. A Convolutional Neural Network (CNN)

## Models Architecture

### Simple Neural Network
- Flatten layer
- Dense layer (128 units, ReLU activation)
- Dense layer (10 units, Softmax activation)

### CNN Model
- Conv2D (64 filters, 3x3 kernel, ReLU activation)
- MaxPooling2D (2x2)
- Conv2D (64 filters, 3x3 kernel, ReLU activation)
- MaxPooling2D (2x2)
- Flatten layer
- Dense layer (128 units, ReLU activation)
- Dense layer (10 units, Softmax activation)

## Dataset

Uses the Fashion MNIST dataset which includes:
- T-shirts
- Trousers
- Pullovers
- Dresses
- Coats
- Sandals
- Shirts
- Sneakers
- Bags
- Ankle boots

## Training Details

- Input: 28x28 grayscale images
- Data preprocessing: Pixel values normalized to [0,1]
- Optimizer: Adam
- Loss function: Sparse Categorical Crossentropy
- Simple NN: 20 epochs
- CNN: 10 epochs

## Results

### Simple Neural Network
- Training loss: 0.1820
- Test loss: 0.3608

### CNN Model
- Training loss: 0.0765
- Test loss: 0.2996

## Requirements

- TensorFlow
- Keras
- NumPy
- Matplotlib

## Usage

The model includes functions for:
- Loading and preprocessing the Fashion MNIST dataset
- Training both neural network architectures
- Making predictions on test images
- Visualizing results with matplotlib

## Visualization

Includes functionality to display images with their predicted labels and confidence scores.
