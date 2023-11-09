# Deep-Learning

Over the last decade, so-called “deep learning” techniques have become very popular in various application domains such as computer vision, automatic speech recognition, natural language processing, and bio-informatics where they produce state-of-the-art results on various challenging tasks. A crucial success factor of deep neural networks is their ability to learn hierarchies of increasingly complex features from raw input data. Such representations often outperform traditionally hand-crafted features that require expensive human effort and expertise. But they do not come as a free lunch. Designing and training deep neural networks such that they actually learn meaningful and useful feature representations of data is an art itself. Mastering it requires practice and experience.

The programs in this repository corresponds to the work done throughout the curriculum "Introduction to Deep Learning" by Prof. Dr. Sebastian Stober at Otto-von-Guericke University, Magdeburg. These programs can be run on Jupyter notebook and uses Tensorflow and Keras for building, visualising and training deep neural networks.

## Deep MLP Model for MNIST dataset
MNIST is a collection of handwritten digits and a popular (now trivialized) benchmark for image classification models. Before building a deep neural network, a linear MLP was build to classify the MNIST images. This linear model was turned into a deep model by adding hidden layers and few experiments were performed by changing the hyperparameters such as - number of layers, number of units in a hidden layer, activation function, learning rate, etc.

## Visualisation and Datasets
Five simple MLP training scripts for MNIST were provided, which fail at training. The idea behind this exercise was to diagnose the underlying problem using visualisation. Tensorborad was used to visualise the computation graph of the model and the trainable variables. Along with the visualisation a way of handling datasets using tf.data was introduced. Tensorflow often uses the three operations shuffle, batch and repeat for handling of datasets. Some experiments were performed by changing the order of these operations and the most sensible order was recorded. The corresponding program is given in [Visualisation and Datasets](https://github.com/nishad-pawaskar/Deep-Learning/tree/10a4b1c8b8f3435c03462ed02acc403c2e71b429/Visualisation%20and%20Datasets). 

## Convolutional Neural Network

Convolutional networks, also known as Convolutional Neural Networks, or CNNs, are a specialized kind of neural network for processing data that has a known grid-like topology. Convolutional networks have been tremendously successful in practical applications. The name “convolutional neural network” indicates that the network employs a mathematical operation called convolution. Convolution is a specialized kind of linear operation. Convolutional networks are simply neural networks that use convolution in place of general matrix multiplication in at least one of their layers. The basic MLP programmed in [Deep MLP Model](https://github.com/nishad-pawaskar/Deep-Learning/tree/d603ad441c0e94befffdb7f4c5d29753e875e9d9/MNIST_Deep_Model) was modified by adding convolutional layers before the dense MLP layer for classification. These convolutional layers help in extracting and learning features using the convolutional kernel from the dataset. [Convolutional Neural Network (CNN)](https://github.com/nishad-pawaskar/Deep-Learning/tree/d603ad441c0e94befffdb7f4c5d29753e875e9d9/Convolutional%20Nueral%20Networks) trains the CNN model for classifying the FashionMNIST and CIFAR10 dataset.

=========