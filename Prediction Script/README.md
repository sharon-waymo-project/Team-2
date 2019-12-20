# Prediction Script

This directory contains the python code for generating the predictions on the unseen data.

This file is mainly used to generate predictions using the VotingRegressor model that we trained in the VotingRegressor_GridSearch.ipynb file

## Input
For running the code in this file, we need 4 inputs:

1) The CSV file of the data for which predictions are needed
2) Saved weights of the VotingRegressor for ax
3) Saved weights of the VotingRegressor for ay
4) Saved weights of the VotingRegressor for az

### Running the model:
Running this model is very easy as you just need to provide the path to the testing data to the pd.read_csv() function at the beginning of the file, and you need to provide the path where the weights of the VotingRegressor model are saved.

### Runtime of the model:
Since we are just generating predictions for a test file, this script does not take a lot of time to process. The runtime execution of the script is about 2-5 minutes.

### Dependencies:
There are multiple Python libraries that are necessary to run this model. They are:
1) Pandas
2) Numpy
3) SciKit Learn
4) Pickle

NOTE: This code was run on Google Colab, so you can remove the cell where there is a google.colab import

### Outputs:
After running the code, 2 files are generated:
1) y_pred.csv: This file contains the predictions of the ax, ay and az
2) y_truth.csv: This file contains the testing data provided.

Both of these files can then be used for Visualization (refer to the Visualization directory)
