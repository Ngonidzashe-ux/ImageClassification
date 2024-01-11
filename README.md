# Image Classification with MobileNet vs. Custom CNN
This repository contains two implementations for image classification using the MNIST Fashion dataset. The first implementation utilizes a custom Convolutional Neural Network (CNN) built from scratch, while the second one employs a pre-trained MobileNetV2 model.

## Custom CNN Implementation - [MNIST Fashion - FromScratchDraft.ipynb]
## Overview
### Loading and Normalizing Data:

The MNIST Fashion dataset is loaded and divided into training and test sets.
Images are normalized by scaling pixel values to the range [0, 1].
### Data Visualization:

Demonstrates reshaping and visualization of images using matplotlib and OpenCV.
### Model Architecture:

Defines a custom CNN architecture with convolutional, max-pooling, and dense layers.
Utilizes the ReLU activation function for non-linearity and sparse categorical crossentropy loss.
### Training the Model:

Compiles the model using the Adam optimizer.
Displays the model architecture.
Trains the model on the training set for 5 epochs.

## MobileNetV2 Implementation - [MNIST Fashion - MobileNetDraft.ipynb]
## Overview
### Loading and Normalizing Data:

Loads the MNIST Fashion dataset and normalizes pixel values to [0, 1].
### Data Visualization:

Displays a grid of images from the training set.
### Preprocessing for MobileNetV2:

Resizes images to a target size (96x96) and converts them to RGB format.
### Data Generator and Model Building:

Implements a data generator for training with preprocessed images.
Builds a MobileNetV2-based model with additional dense layers for classification.
### Training the Model:

Compiles the model with categorical crossentropy loss.
Trains the model using a data generator for 2 epochs.
## Important Note
The fit_generator and evaluate_generator methods are deprecated. The recommended methods are fit and evaluate, which support generators. Consider updating your code accordingly.
## Instructions for Running the Code
Ensure you have the necessary dependencies installed, such as TensorFlow and Keras.
Run the code in the provided Jupyter notebooks (MNIST Fashion - FromScratchDraft.ipynb and MNIST Fashion - MobileNetDraft.ipynb).
Review the results, model architectures, and any visualizations generated during the execution.
Feel free to explore and compare the performances of the custom CNN and MobileNetV2-based models for image classification on the MNIST Fashion dataset.
