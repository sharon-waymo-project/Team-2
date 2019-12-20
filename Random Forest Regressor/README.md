# Random Forest Regressor

This directory contains the python code for running the Random Forest Regressor model

### Description:
After having some success with the NN-KerasRegressor model, we tried to experiment by using an ensemble method, called as Random Forest Regressor.

To find the best possible hyper parameters for training this model, we used a technique called as GridSearch.

While running GridSearch, we used the cross validation split as 3.

The different hyperparameters that we used for GridSearch were:

1) max_depth: The maximum depth of the tree
2) max_features: The number of features to consider when looking for the best split
3) min_samples_leaf: The minimum number of samples required to be at a leaf node.
4) min_samples_split: The minimum number of samples required to split an internal node
5) n_estimators: The number of trees in the forest

### Running the model:
Running this model is very easy as you just need to provide the path to the training and testing data to the pd.read_csv() function at the beginning of the file, and then you can simply run the entire code.

### Runtime of the model:
Since we are using GridSearch to find the best hyper parameters, this code takes a lot of time to execute. The running time of this code is about 20-30 minutes.

### Dependencies:
There are multiple Python libraries that are necessary to run this model. They are:
1) Pandas
2) Numpy
3) Matplotlib
4) SciKit Learn
5) Seaborn

NOTE: This code was run on Google Colab, so you can remove the cell where there is a google.colab import
