# Project Overview

This project is a study of transfer learning in image classification with a specialized
focus on binary classification of chest X-ray images. 

It involves:

- Training a ResNet-18 model without freezing any layers.

- Addressing overfitting and poor accuracy using data augmentation, L2 regularization, and learning rate adjustment.

- Experimenting with Particle Swarm Optimization (PSO) to determine the optimal number of layers to freeze.

# Dataset
The dataset is downloaded from this link.

https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia/data

It consists of labeled images of pneumonia and normal X-rays. 

# Initial Training

Model              : ResNet-18

Data Augumentation : Randomly flip horizontaly, randomly rotate images.

Training           : All layers were trainable with pretrained weights.

Optimizer          : Adam with learning rate 0.001 for 50 epochs.

Issues             : poor accuracy, flutuation, and overfitting.

# Improvements

Data Augmentation: Applied more data augementattion method to increase the diversity of the training data (color variation and randomly crop).

L2 Regularization: Added to the loss function to penalize large weights.

Learning Rate Adjustment: learning rate was reduced by 10% every 10 epchs.


# PSO for Layer Freezing

Objective: Determine the optimal number of layers to freeze using Particle Swarm Optimization.

Outcome: This approach did not yield significant improvements.

# Results

Initial Model: Poor accuracy and overfitting.

Improved Model: Better accuracy and reduced overfitting after implementing data augmentation, L2 regularization, and learning rate adjustment.

PSO Experiment: No significant improvement in model performance.


  
