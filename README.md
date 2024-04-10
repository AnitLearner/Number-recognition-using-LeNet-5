# Number-recognition-using-LeNet-5
Used the MNIST dataset to train the model using LeNet Architecture
This project implements the LeNet-5 convolutional neural network architecture for the task of digit recognition using the MNIST dataset. LeNet-5 is a classical CNN architecture proposed by Yann LeCun et al. in 1998, which was one of the pioneering works in the field of deep learning.

Introduction
The MNIST dataset consists of 28x28 grayscale images of handwritten digits (0-9) along with their corresponding labels. The goal of this project is to train a deep learning model to accurately classify these digits.

Getting Started
Prerequisites
Make sure you have the following prerequisites installed:

Python 3.x
TensorFlow
NumPy
Matplotlib


Loading and Preprocessing the Dataset
The MNIST dataset is automatically downloaded and preprocessed using the TensorFlow Keras library. It is split into training and testing sets, and the pixel values are normalized to the range [0, 1].

Model Architecture
The LeNet-5 architecture used in this project consists of the following layers:

Convolutional Layer 1: 6 filters with a kernel size of 5x5 and ReLU activation.
Average Pooling Layer 1: 2x2 pooling window.
Convolutional Layer 2: 16 filters with a kernel size of 5x5 and ReLU activation.
Average Pooling Layer 2: 2x2 pooling window.
Flatten Layer.
Fully Connected Layer 1: 120 neurons with ReLU activation.
Fully Connected Layer 2: 84 neurons with ReLU activation.
Output Layer: 10 neurons with softmax activation.
Training the Model
The model is compiled using the Adam optimizer and categorical cross-entropy loss function. It is trained for 10 epochs with a batch size of 128. Training and validation accuracies are monitored throughout the training process.

Results
After training the model for 10 epochs, the validation accuracy achieved is approximately 98.64%.

Visualization
Training and validation accuracies and losses are plotted using Matplotlib to visualize the training progress and model performance.
