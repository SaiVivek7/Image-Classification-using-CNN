# Cat vs Dog Image classification using CNN
This repository contains an implementation of a Convolutional Neural Network (CNN) for binary image classification to distinguish between images of cats and dogs. The model is built using TensorFlow's Keras library and trained on a labeled dataset of cat and dog images.

## Dataset
The dataset used for training and evaluation can be found here: https://bit.ly/ImgClsKeras. The data consists of labeled images of cats and dogs.

## Model Architecture

The CNN architecture used in this project consists of the following layers:

- `Conv2D Layer 1`: 32 filters of size `(3,3)` with ReLU activation, with an input shape of `(100, 100, 3)` for the first layer.
- `MaxPooling2D Layer 1`: Pooling layer with a `(2,2)` pool size.
- `Conv2D Layer 2`: 32 filters of size `(3,3)` with ReLU activation.
- `MaxPooling2D Layer 2`: Pooling layer with a `(2,2)` pool size.
- `Flatten`: Flattening the matrix to a vector for input to the dense layer.
- `Dense Layer 1`: Fully connected layer with 64 units and ReLU activation.
- `Dense Layer 2`: Fully connected layer with 1 unit and sigmoid activation for binary classification.

This architecture is designed to capture essential features in the images for binary classification between cats and dogs.
