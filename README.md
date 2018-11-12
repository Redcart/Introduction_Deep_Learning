# Introduction to Deep Learning for Computer Vision

This repository intends to introduce to some basic understanding of deep learning. The code is written in Python using Keras API through TensorFlow as backend.

## Data

In this project we use different kinds of sources of data:
- Hand-written digits from MNIST
- Clothes images from MNIST Fashion

All datasets are in the following shape: (n_samples, n_heigth, n_width, n_channels) In the case of greyscale images (0 ==> white, 255 ==> black; inverse of the initial scale), n_channels will be equal to one.

## Models

Our goal is to create machine learning algorithms in order to predict for any image to which class it belongs. Thus, we deal with a classification task in the field of computer vision. That is why, we will focus mainly on Convolutionnal Neural Networks (CNN). We will basically use three kinds of layers:

- Convolutionnal (Conv2D in Keras)
- Max Pooling (MaxPoooling2D in Keras)
- Fully Connected (Dense in Keras)

Before applying the last fully-connected layers, we will flatten the output of Max Pooling (Flatten() in Keras).

## Scripts

In each script, we present different models relying on famous neural networks architectures:

- Script_01 ==> Basic Multi Layer Perceptron
- Script_02 ==> Basic CNN
- Script_03 ==> **LeNet-5**
- Script_04 ==> **AlexNet**
- Script_05 ==> **VGG16**

These architectures are adapted to the dimensions of the input images (28x28x1). 
Indeed, LeNet-5 was trained on 32x32x1, AlexNet was trained on 227x227x3, VGG-16 was trained on 224x224x3 images.
