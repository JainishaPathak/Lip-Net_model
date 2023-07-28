# Lip Reading AI Model - LipNet

## Lip Reading AI
**Introduction**

This repository contains the implementation of a Lip Reading AI model based on the LipNet research paper. The model is capable of converting lip movements from videos into corresponding text.

**Installation**

To run the code, please make sure you have the following dependencies installed:

- OpenCV-Python
- Matplotlib
- ImageIO
- gdown
- TensorFlow

You can install these dependencies using the following pip command:

```bash
pip install opencv-python matplotlib imageio gdown tensorflow
## Data Loading and Preprocessing

The notebook `LipNet.ipynb` contains code to load and preprocess data. It includes functions to extract video frames, convert frames to grayscale, and perform necessary data transformations.

## Data Pipeline

We have created a data pipeline to efficiently handle the data. The dataset is split into training and testing sets. The `ProduceExample` callback generates predictions and prints the original and predicted text after each epoch during training.

## Deep Neural Network Architecture

The Lip Reading AI model architecture consists of 3D convolutional layers, LSTM layers, and dense layers. The model is designed to process video frames and predict corresponding text sequences.

## Training and Evaluation

The model is trained using the CTC (Connectionist Temporal Classification) loss and the Adam optimizer. A learning rate scheduler is employed to optimize the training process. The training and validation results are evaluated using the test set.


