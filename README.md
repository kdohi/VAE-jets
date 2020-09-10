# VAE-jets

This repository contains all the code to. The paper demonstrates the use of variational autoencoders (VAE) as powerful tools for jet simulation. With the growing popularity and success of generative adversarial networks (GAN) in high energy physics, we explore variational autoencoders for calorimeter response simulation and compare it to the Location-Aware Generative Adversarial Network (LAGAN). 

## Notebooks

### CNN for Feature Perceptual Loss
The model we propose utilizes the feature perceptual loss to produce the sparse features of jet images. The feature perceptual loss is the mean squared error of the hidden layers of two images. In this case, we take the feature perceptual loss between the input and output image of the variational autoencoder. These hidden features are calculated from a prettrained convolutional neural network (CNN) classifier. The CNN model is shown in this notebook.

### CVAE Convolutional First Layer
This notebook contains the code for the actual VAE model. We load the prettrained CNN model and use it to calculate the loss along with the Bernoulli and KL divergence loss. More detail on the model is found in the notebook.



