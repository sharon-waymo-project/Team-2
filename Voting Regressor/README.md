# Voting Regressor

This directory contains the python code for running the Voting Regressor model

After seeing good results with the Random Forest Regressor model, we decided to use an ensemble of regressors, called as Voting Regressor.

This directory contains 2 files, and the description of both the files is given below:

## VotingRegressor_GridSearch.ipynb
This file contains the code where we trained the models like RandomForestRegressor, AdaBoostRegressor, ExtraTreesRegressor and GradientBoostingRegressor with GridSearch.

While running GridSearch, we used the cross validation split as 5.

The different hyperparameters that we used for RandomForestRegressor were:
1) max_depth: The maximum depth of the tree
2) max_features: The number of features to consider when looking for the best split
3) n_estimators: The number of trees in the forest.

The different hyper parameters that we used for AdaBoostRegressor were:
1) n_estimators: Maximum
number of trees when boosting is stopped
2) learning_rate: Shrinks the
contribution of each regressor by the value of the learning_rate
3) loss: Loss function used to update the weights after
each boosting iteration

The different hyper parameters that we used for ExtraTreesRegressor were:
1) n_estimators: The number of trees used in the forest
2) max_features: Number of
features to consider to get the best split

The different hyper parameters that we used for GradientBoostingRegressor were:
1) n_estimators: Number of boosting stages to perform
2) learning_rate: Shrinks the contribution of each tree by the value of the learning_rate
3) max_depth: Max depth value of each regressors
4) max_features: Amount of features to consider for the split

### Running the model:
Running this model is very easy as you just need to provide the path to the training and testing data to the pd.read_csv() function at the beginning of the file, and then you can simply run the entire code.

### Runtime of the model:
Since we are using GridSearch to find the best hyper parameters, this code takes a lot of time to execute. The running time of this code is about 30-45 minutes.

### Dependencies:
There are multiple Python libraries that are necessary to run this model. They are:
1) Pandas
2) Numpy
3) Matplotlib
4) SciKit Learn
5) Pickle
6) Xgboost

NOTE: This code was run on Google Colab, so you can remove the cell where there is a google.colab import

### Outputs:
This code trains for the labels of ax, ay and az individually. Thus, after training for each label, a model of the Voting Regressor is saved, which can be later used for prediction of unseen data. We decided to do this as retraining the model every time would be very time consuming.

## VotingRegressor.ipynb
This file uses the same regressors that we used in the previous file, but instead of running GridSearch again, we simply used the best hyper parameters found from the previous file, and train the VotingRegressor.

The main purpose of this file was to get the average MAE, and check how much time it takes for the training of the VotingRegressor without the hyper parameter tuning.

### Running the model:
Running this model is very easy as you just need to provide the path to the training and testing data to the pd.read_csv() function at the beginning of the file, and then you can simply run the entire code.

### Runtime of the model:
This model is not that complicated, so the running time of this code is about 10-15 minutes.

### Dependencies:
There are multiple Python libraries that are necessary to run this model. They are:
1) Pandas
2) Numpy
3) Matplotlib
4) SciKit Learn
5) Pickle
6) Xgboost

NOTE: This code was run on Google Colab, so you can remove the cell where there is a google.colab import
