# MNIST

This repo includes R scripts used for the dimensionality reduction of MNIST handwritten digits data set.
Multi-layer perceptron neural networks are used to train auto-encoder networks to reduce the dimensionality of the data.

An auto-encoder network is applied to the dataset digit_pixels.txt (which is a data set of handwritten digits in pixel form represented by 196 values in one row per digit), along with a dataset digit_characters.txt (which is the dataset that represents the pixel's true identity). The goal is to reduce the dataset digit_pixels.txt using a multi-layer perceptron neural network with 3 hidden layers to two dimensions. This will be done through an appropriate choice of learning rates and iterations on the digit_characters.txt dataset in order to arrive a low squared error. The two dimensions (hidden unit values) obtained from the appropriate iteration are plotted on a scatterplot with the real identity of its character (0-9) displayed over it. 
The idea is that we want clusters of handwritten digits that are easily identifiable and look separated from one another (ex. zeros in one area of the scatterplot, and 2's in another part of the plot).



# Navigating the files

The MNIST_functions file contains functions that were used to develop the neural network, such as the calculation of the gradient, the forward network computation for the calculation of the hidden unit inputs, and the fit of the multi-layer perceptron network using gradient descent. 

THe MNIST_scripts file contains the parameters I used to train the network using the functions from MNIST_functions. I trained the network many times trying out different iterations and learning rates until I got a suitable outcome for the classifying the handwritten digits on a 2-D scatterplot. 

Finally, the Word document file represents my findings, my writeup as well as any associated plots of training errors across iteration choices and the scatterplots of the digits (after dimensionality reduction) as well.
