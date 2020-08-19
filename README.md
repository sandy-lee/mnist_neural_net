# How to train neural networks for image classification

Image classification is a hot topic in data science with the past few years seeing huge improvements in many areas. It has a lot of applications everywhere including SEO. But how is this done?

A deep neural network is a network of artificial neurons organised into layers (via software). With each layer connected to the next and each connection having a weight that helps determine how much the artificial neuron fires. This firing helps determine how strong the connections are between layers, and in general neurons that fire together have stronger connections. Just like with biological neurons.

How strong these connections are is determined by how the network is trained on the data you put into it. These networks are trained via a process called backpropagation which works to feed data into the network and then measures the network’s performance. This error is measured using a loss function.

Backpropagation works by using gradient descent to measure the rate-of-change of the loss function with respect to the weighting of each connection, and the gradient descent step is used to make sure the error rate for each connection is reduced as close to zero as possible. The network should eventually converge on a solution where the overall error is minimised.

The rate at which the network learns is called the learning-rate and this is another hyperparameter that can be tuned when training neural networks. If the learning rate is too small, the network can take too long to converge on a solution, and conversely, if the learning rate is too large then the network will ‘bounce around’ and never really converge on an optimum solution.

There are different types of layers in neural networks, and each one transforms data differently. The most basic type is a dense layer, which is where all neurons are connected. Other types include convoluted layers which are primarily used for image processing tasks and recurrent layers which are used to process time-series data. There are others, but these are the most common types.

In this article, I will be focusing on how to implement a simple image classifier using a series of dense layers using in using Keras as part of Tensorflow. As mentioned above, convoluted neural networks usually work better for image classification tasks and I will talk about these in part 2 of this series. As my primary area of interest is Search Engine Optimisation, I will tie all of this together in part 3 for how neural networks are used in search.