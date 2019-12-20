# NN-KerasRegressor

This directory contains the python code for running the NN-KerasRegressor model
.
This type of model uses both, a neural network and regression for the prediction of the acceleration.

### Description: 
We tried applying a unique approach of applying regression after sending the data as an input to a Neural Network first. The main aim of having a neural network before applying regression is that the neural network will transform the input features on its own and this can help for better values for the regression model.

The neural network that we used consisted of 3 hidden layers. 1st hidden layer consisted of 20 units, 2nd hidden layer consisted of 10 units, 3rd hidden layer consisted of 5 units. All these layers had ReLU as their activation function. The output layer consisted of 3 units, which is then given to the regressor. 

The neural network was run for 100 epochs with the cross validation set as 3 splits. 

### Running the model:
Running this model is very easy as you just need to provide the path to the training and testing data to the pd.read_csv() function at the beginning of the file, and then you can simply run the entire code.

### Runtime of the model:
This code takes some time to train, and it can be completed in about 10 minutes.

### Dependencies:
There are multiple Python libraries that are necessary to run this model. They are:
1) Keras
2) Pandas
3) Numpy
4) Matplotlib
5) SciKit Learn
6) Seaborn
