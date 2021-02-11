# **CMPE 258 Assignment 1**
### **Part 2**

### Steps in brief:
* The ask: To build a neural network to classify the hand written digits into their 10 classes (0-9)
* Dataset: MNIST dataset, a collection of 60,000 labeled digits
* Process:
  * The training starts off as a single dense layer. It has 10 neurons to classify handwritten digits into 10 classes. It uses "softmax" activation because it is the last layer in a classifier, with a basic sgd optimizer and categorical_crossentropy as the loss function with accuracy as the metric.
  * Adding 2 more intermediate layers activated with the sigmoid function
  * Replacing all the sigmoid activation functions to relu activation function.
  * Replacing sgd optimizer with adam.
  * Increasing the learning rate from its default value of 0.001 to 0.01.
  * Increasing the depth of the model to 4 dense layers - number of neurons in the layers: 200, 100, 60, 10.
  * Adding dropout after each intermediate dense layer in the network (25% dropout rate)
  * Modifying the model into a convolutional model and removing all the dropouts.
  * Finally adding a dropout of 40% between the 2 dense layers in the network.
* Result: The validation loss will not increase further and the accuracy is much above 99%

### Please Note:
The details and explanations for each step has been given in the colab itself.

### Points to remember:
* batch or mini-batch: training is always performed on batches of training data and labels. Doing so helps the algorithm converge. The "batch" dimension is typically the first dimension of data tensors. For example a tensor of shape [100, 192, 192, 3] contains 100 images of 192x192 pixels with three values per pixel (RGB).
* cross-entropy loss: a special loss function often used in classifiers.
* dense layer: a layer of neurons where each neuron is connected to all the neurons in the previous layer.
* features: the inputs of a neural network are sometimes called "features". The art of figuring out which parts of a dataset (or combinations of parts) to feed into a neural network to get good predictions is called "feature engineering".
* labels: another name for "classes" or correct answers in a supervised classification problem
* learning rate: fraction of the gradient by which weights and biases are updated at each iteration of the training loop.
* logits: the outputs of a layer of neurons before the activation function is applied are called "logits". The term comes from the "logistic function" a.k.a. the "sigmoid function" which used to be the most popular activation function. "Neuron outputs before logistic function" was shortened to "logits".
* loss: the error function comparing neural network outputs to the correct answers
* neuron: computes the weighted sum of its inputs, adds a bias and feeds the result through an activation function.
* one-hot encoding: class 3 out of 5 is encoded as a vector of 5 elements, all zeros except the 3rd one which is 1.
* relu: rectified linear unit. A popular activation function for neurons.
* sigmoid: another activation function that used to be popular and is still useful in special cases.
* softmax: a special activation function that acts on a vector, increases the difference between the largest component and all others, and also normalizes the vector to have a sum of 1 so that it can be interpreted as a vector of probabilities. Used as the last step in classifiers.
* tensor: A "tensor" is like a matrix but with an arbitrary number of dimensions. A 1-dimensional tensor is a vector. A 2-dimensions tensor is a matrix. And then you can have tensors with 3, 4, 5 or more dimensions.

### Reference:
https://codelabs.developers.google.com/codelabs/cloud-tensorflow-mnist#0
