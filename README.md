# **Student Depression Predictor**

This repository contains the source code, the dataset, and other files for the CMSE 202 Honors Project that aims to build a model to determine whether or not a student is diagnosed with depression, given data regarding the student's academic, professional, and personal circumstances and habits. This goal of this project is to combine the widespread issue of the increasing mental health concerns among students with Machine Learning techniques such as Principal Component Analysis and Deep Learning to promote awareness and hopefully build a model that can help confused students understand themselves and their state of mind better. This is a binary classification problem where an observation is classified as positive if the model predicts that the observation represents a student diagnosed with depression, and negative otherwise.

**IMPORTANT:** Please do NOT rely on this or any Artificial Intelligence model to diagnose depression or other mental health conditions. If you believe that you are in need of support, please arrange a psychological evaluation with a Therapist or other licensed professionals.

## **Principal Component Analysis (PCA)**
- In this project, we use PCA to compress the input features to a lower dimensionality before running them through a neural network.
- PCA allows us to derive orthogonal components that can be used to translate an input feature vector to a space where the different patterns between the two classes are more distinct.
- PCA may also reduce the computational cost of training our neural network, since the input's reduced dimensionality and a more distinct variance between the principal components of the two classes may lower the need for a more complex network architecture.

## **Deep Learning**
- For the purpose of this project, we will be using `PyTorch` to build, train, and test our network.
- We create a simple architecture of eight neurons in the input layer, two neurons in the output layer, with the hidden layers having one less neuron than their previous layer.
- All layers, except for the output layer, will undergo `ReLU` activation before passing onto the next layer.
- Our neural network is found to correctly classify observations with approximately **80%** accuracy.
