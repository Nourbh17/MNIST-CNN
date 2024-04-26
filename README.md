# MNIST-CNN

## Dataset 

The MNIST database (Modified National Institute of Standards and Technology database) is a large database of handwritten digits that is commonly used for training various image processing systems. The MNIST database of handwritten digits, has a training set of 60,000 28x28 grayscale images of the 10 digits, and a test set of 10,000 examples. It is a subset of a larger set available from NIST. The digits have been size-normalized and centered in a fixed-size image.
Sample images from MNIST test dataset:

![1](https://github.com/Nourbh17/MNIST-CNN/assets/92574404/3798f2f7-5d63-4a15-897a-fb3c532e9502)

## Models :

### Small Model:

Composed of two convolutional layers followed by a flattening layer and a dense layer:

The first convolutional layer has 64 filters with a kernel size of 3x3, ReLU activation, and same padding.

The second convolutional layer has 32 filters with a kernel size of 3x3, ReLU activation, and same padding.

The output of the last convolutional layer is flattened to be fed into a dense layer with 10 units and a softmax activation function for classification.

### Medium Model:

Composed of a convolutional layer, a max pooling layer, a dropout layer, a flattening layer, and two dense layers:

The convolutional layer has 32 filters with a kernel size of 5x5, ReLU activation, and same padding.

The max pooling layer reduces the spatial dimensions of the output by a factor of 2 in both width and height.

The dropout layer randomly sets a fraction of input units to zero during training to prevent overfitting.

The output is then flattened and passed through a dense layer with 128 units and ReLU activation, followed by another dense layer with 10 units and softmax activation for classification.

### Large Model:

Composed of two convolutional layers, a max pooling layer, a dropout layer, flattening layer, and three dense layers:

The first convolutional layer has 30 filters with a kernel size of 5x5, ReLU activation, and same padding.

The max pooling layer reduces the spatial dimensions of the output by a factor of 2 in both width and height.

The second convolutional layer has 15 filters with a kernel size of 3x3, ReLU activation, and same padding.

The dropout layer helps in preventing overfitting by randomly setting a fraction of input units to zero.

The output is then flattened and passed through three dense layers with ReLU activation, consisting of 128 units, 50 units, and finally 10 units with softmax activation for classification.

These models vary in their architecture complexity, with the small model being the simplest and the large model being the most complex. Each model is designed to extract features from input images and classify them into one of the ten classes (digits 0 through 9) in the MNIST dataset.

## Keras implementation Test accuracy : 

Small model : 96.64%

Medium model: 95.41%

Large model : 96.95%




