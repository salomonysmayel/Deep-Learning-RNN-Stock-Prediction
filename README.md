# Deep_Learning_Homework

## Which model has a lower loss?

The model for predicting price using closing prices had the lower loss mean squared error of 0.0363 compared to 0.2016 from the sentiment based model

## Which model tracks the actual values better over time?

The model for predicting price using closing prices tracks better the values over time, as can be seen in the graphs

### closing prices model graph, Predicted vs Real

![table](https://github.com/salomonysmayel/Deep_Learning_Homework/blob/master/Image1.png "Image1")

### Greed and fear model graph, Predicted vs Real

![table](https://github.com/salomonysmayel/Deep_Learning_Homework/blob/master/image2.png "image2")

## Which window size works best for the model?

For both models a window of 1 results in lower values for loss function, hence works best for the models


loss = 0.2016 / window = 1

loss = 0.2095 / window = 2

loss = 0.2709 / window = 10


loss = 0.0363 / window = 1

loss = 0.0389 / window = 2

loss = 0.1026 / window = 10
