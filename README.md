# Neural-Network-from-Scratch-using-Numpy
Libraries you need are:
- Numpy
- Matplotlib for graphs and curves
- TSNE for plot
- Sklearn Shuffle function

# Single Perceptron File
In this file we are provided with the dataset which is randomly generated with 0 and 1 labels. Our task is to made a custom neural network with one neuron. The dataset has some distribution (Visualizations in Notebook)

The data is divided into training, validation and testing. I have appended the feature with a column of ones that help me to add bias in a weight vector instead of separately finding derivative with respect to bias as well. The weight vector has dimension (input size+1, number of output). Sigmoid is used for the decision because it’s a binary classification problem and other activation function not perform well. So sigmoid help us to give us probability values. As in this task we have to find accuracy by ourself. Instead of using skearn building formula. So I take a threshold and divide my prediction to 0 and 1 to find the accuracy.
The learning curve and accuracy for both training and validations are shown in file. Epoch = 5000 and Learning rate = 0.0001

# Single hidden layer Network File
In this notebook we are provided with the sklearn dataset with 0 and 1 labels. Our task is to made a custom neural network with 3 input, 2 hidden and 1 output layer neuron. The dataset has some distribution shown in file
The data is again divided into training, validation and testing. I have appended the feature with a column of ones that help me to add bias in a weight vector for input layer but bias for the hidden layer should be added separately and we will find its derivative with respect to cross entropy loss function. The weight vector has dimension (input size+1, number of output). In this task we have to use different activation function and check their accuracies. But the Sigmoid is used for the decision at the output layer because it’s a binary classification problem and other activation function not perform well.

Here are some useful results that need to consider.
- Epoch = 5000 and Learning rate = 0.0001 (for Sigmoid on hidden layer)
- Epoch = 5000 and Learning rate = 0.0001 (for Tanh on hidden layer)
- Epoch = 5000 and Learning rate = 0.0001 (for Relu on hidden layer)

Accuracy scores are:
- Train = 100, Validation = 100, testing = 100 (for Sigmoid on hidden layer)
- Train = 100, Validation = 98, testing = 99 (for Tanh on hidden layer)
- Train = 90, Validation = 88, testing = 88 (for Relu on hidden layer)

# Multiple Hidden Layer Network File
In this task we are provided with the MNIST dataset. For this firstly I did preprocessing on the data. I did mean subtraction method and in this task we have two hidden and and output layer with 10 neurons. As this is a multiclass problem so here we are using softmax activation function.
Here are some useful results that need to consider.
Epoch = 100 and Learning rate = 0.1
- training Loss: 1.0160077930881226 validation Loss: 1.1539617413967806 train accuracy 76.536 valid accuracy 73.76
- Testing Accuracy = 75.04

Model files are also attached in the repository
