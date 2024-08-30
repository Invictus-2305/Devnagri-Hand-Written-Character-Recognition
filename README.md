# Devnagri Handwritten Character Recognition

This project is focused on building a Handwritten Character Recognition (HWRC) system for Devnagri script using deep learning techniques. The model is trained using TensorFlow and Keras, leveraging the **[Devanagari Handwritten Character Dataset](https://archive.ics.uci.edu/dataset/389/devanagari+handwritten+character+dataset)**.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This project aims to recognize handwritten Devnagri characters. The system is built using a convolutional neural network (CNN) that classifies images of characters into 46 different classes.

## Dataset

The dataset used for this project was downloaded from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/389/devanagari+handwritten+character+dataset). It consists of:
- **Training Set**: 62,560 images
- **Test Set**: 15,640 images

The images are organized into 46 classes representing different Devnagri characters.

## Model Architecture

The model is built using TensorFlow and Keras, with the following architecture:

- **Input Layer**: Image data resized to 32x32 pixels
- **Convolutional Layers**: Several layers with ReLU activation and max-pooling
- **Dense Layers**: Fully connected layers with dropout regularization
- **Output Layer**: Softmax activation function for multi-class classification

## Training

The training process involves using an `ImageDataGenerator` for data augmentation, with a validation split of 20%. The model is trained on the training dataset, and validation is performed to monitor its performance.

### Key Training Parameters:
- **Batch Size**: 32
- **Image Size**: 32x32 pixels
- **Number of Classes**: 46

## Evaluation

The model's performance is evaluated using the test dataset. Metrics such as accuracy and loss are used to gauge the model's effectiveness in recognizing handwritten Devnagri characters.
## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for any bugs or feature requests.
