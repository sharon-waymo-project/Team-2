# Baseline models

This directory contains the python code for running the baseline models for the prediction of the acceleration.

The 2 baseline models that we have used here are Neural Network models. The description for each of the models is given below:

## Baseline 1: 
This model contains a very shallow deep neural network. This neural network just has 1 hidden layer consisting of 16 units. The input layer has 12 units (the number of input features), and the output layer has 3 units (to predict ax, ay and az). The activation function used for the hidden layer is ReLU, whereas the activation function used at the output layer is a sigmoid function to get the values of the predictions.

### Running the model:
Running this model is very easy as you just need to provide the path to the training and testing data to the pd.read_csv() function at the beginning of the file, and then you can simply run the entire code.

eg : path/train.csv

### Runtime of the model:
The runtime of the code is pretty fast, and it can be completed in about 1 minute.

### Dependencies:
There are multiple Python libraries that are necessary to run this model. They are:
1) Keras
2) Pandas
3) Numpy
4) Matplotlib
5) SciKit Learn
6) Seaborn

## Baseline 2:
This model is a bit deeper than the Baseline 1 model. This neural network model has 2 hidden layers. 1st hidden layer has 16 units with activation function as ReLU, the 2nd hidden layer has 4 hidden units with activation function as ReLU. The input layer has 12 units (for the number of features) and the output has 3 units (for predicting ax, ay, az). The activation function used at the output layer is Sigmoid, to calculate the predictions for the values of ax, ay and az.

### Running the model:
Running this model is very easy as you just need to provide the path to the training and testing data to the pd.read_csv() function at the beginning of the file, and then you can simply run the entire code.

### Runtime of the model:
The runtime of the code is pretty fast, and it can be completed in about 2 minutes.

### Dependencies:
There are multiple Python libraries that are necessary to run this model. They are:
1) Keras
2) Pandas
3) Numpy
4) Matplotlib
5) SciKit Learn
6) Seaborn
