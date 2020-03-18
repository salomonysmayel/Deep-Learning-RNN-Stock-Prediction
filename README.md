# Deep Learning Homework

## Background

Due to the volatility of cryptocurrency speculation, investors will often try to incorporate sentiment from social media and news articles to help guide their trading strategies. One such indicator is the Crypto Fear and Greed Index (FNG) which attempts to use a variety of data sources to produce a daily FNG value for cryptocurrency. You have been asked to help build and evaluate deep learning models using both the FNG values and simple closing prices to determine if the FNG indicator provides a better signal for cryptocurrencies than the normal closing price data.
In this assignment, you will use deep learning recurrent neural networks to model bitcoin closing prices. One model will use the FNG indicators to predict the closing price while the second model will use a window of closing prices to predict the nth closing price.

You will need to:

Prepare the data for training and testing
Build and train custom LSTM RNNs
Evaluate the performance of each model

## Instructions

Prepare the data for training and testing

Use the starter code as a guide to create a Jupyter Notebook for each RNN. The starter code contains a function to help window the data for each dataset.

For the Fear and Greed model, you will use the FNG values to try and predict the closing price. A function is provided in the notebook to help with this.

For the closing price model, you will use previous closing prices to try and predict the next closing price. A function is provided in the notebook to help with this.

Each model will need to use 70% of the data for training and 30% of the data for testing.

Apply a MinMaxScaler to the X and y values to scale the data for the model.

Finally, reshape the X_train and X_test values to fit the model's requirement of (samples, time steps, features).

Build and train custom LSTM RNNs

In each Jupyter Notebook, create the same custom LSTM RNN architecture. In one notebook, you will fit the data using the FNG values. In the second notebook, you will fit the data using only closing prices.
Use the same parameters and training steps for each model. This is necessary to compare each model accurately.

Evaluate the performance of each model

Finally, use the testing data to evaluate each model and compare the performance.

**Use the above to answer the following:**

Which model has a lower loss?

Which model tracks the actual values better over time?

Which window size works best for the model?

## Results

**Which model has a lower loss?**

The model for predicting price using closing prices had the lower loss mean squared error of 0.0363 compared to 0.2016 from the sentiment based model

**Which model tracks the actual values better over time?**

The model for predicting price using closing prices tracks better the values over time, as can be seen in the graphs

**closing prices model graph, Predicted vs Real**

![table](https://github.com/salomonysmayel/Deep_Learning_Homework/blob/master/Image1.png "Image1")

**Greed and fear model graph, Predicted vs Real**

![table](https://github.com/salomonysmayel/Deep_Learning_Homework/blob/master/image2.png "image2")

**Which window size works best for the model?**

For both models a window of 1 results in lower values for loss function, hence works best for the models

**Greed and fear model loss vs window**

loss = 0.2016 / window = 1

loss = 0.2095 / window = 2

loss = 0.2709 / window = 10

**closing prices model loss vs window**

loss = 0.0363 / window = 1

loss = 0.0389 / window = 2

loss = 0.1026 / window = 10
