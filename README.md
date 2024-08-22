## Prediction of time-series data using Artificial Neural Networks (ANN) using sliding window technique

*Modelling of ANN for Time series data using sliding window technique*

This code defines a class `sys` that performs data preprocessing, training, and evaluation of an Artificial Neural Network (ANN) model using the Keras library. Here's a breakdown of its functionality:

1. __Initialization__ (`__init__` method):

    - Loads data from an Excel file based on a specified cluster.
    - Normalizes the data using `MinMaxScaler`.
    - Sets various parameters for training, such as train size, sequence size, number of layers, nodes in each layer, and activation function.

2. __Data Splitting__ (`train_split` method):

    - Splits the data into training and testing sets based on the specified train size.

3. __Sequence Conversion__ (`to_sequences` method):

    - Converts the data into sequences suitable for training the ANN.
    - Using sliding window technique.

4. __ANN Model Training__ (`ANN` method):

    - Prepares the training and testing data sequences.
    - Defines and compiles an ANN model with specified layers and nodes.
    - Trains the model on the training data and evaluates it on the testing data.
    - Calculates performance metrics such as R2 score and Mean Squared Error (MSE) for both training and testing data.
    - Inverses the scaling of predictions and actual values for better interpretability.

5. __Printing Results__ (`printing` method):

    - Prints the Root Mean Squared Error (RMSE) for the testing data.
6. __Plotting Results__ (`plotting` method):

    - Plots the predicted and actual values for both training and testing data to visualize the model's performance.
7. __Execution__ (`do_it` method):

    - Calls the methods to split the data, train the ANN, print results, and plot the results.

_This class is designed to automate the process of training an ANN on time-series data, evaluating its performance, and visualizing the results._

### Results

1. Effect of Sample size for training
2. Effect of Window size
3. Effect of Hidden Layers
4. Effect of Activation Functions
5. Effect of Hidden nodes