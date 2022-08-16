# Data-Science-Project : STOCK FORECASTING

Objective: Data science approach to stock prices forecasting & prediction of TATA MOTORS Ltd. stock using Long Short-Term Memory (LSTM) model.

Introduction :

Stock market prediction is the act of trying to determine the future value of company stock or other financial instruments traded on an exchange.The successful prediction of a stock’s future price could yield a significant profit. In this application, we used the LSTM network to predict the next single day as well as next 10 days closing stock price using the past 10 years stock prices. We have imported few libraries for stock market forecasting and they are namely as : pandas,numpy,matplotlib,plotly,datetime to get stock information & data visualization purpose.


---> What is Time-Series?
Time Series comprises of observations that are captured at regular intervals. Time Series datasets have a strong temporal dependence. It can be used to forecast future observations based on previous ones.

Import Dataset from yfinance

---> Discription of Attributes
Date: — Trading date of the stock.

Open: — This price of stock’s opening price which means the very beginning price of particular trading day, but which is not be the same price of precious’s day ending price.

High: — This is the highest price of the stock on a particular trading day.

Low: — This is the lowest stock price during trade day.

Close: — This is the closing price of the stock during trade-in particular day.

Volume: — This is the number of stocks traded on a particular day.

Adj Close: — This is the ending or closing price of the stock which was changed to contain any corporations’ actions and distribution that is occurred during trade time of the day.

---> Show [Close] column plot by using plotly 

---> Implementation of model : LSTM
---> Seggregate the data into Train & Test

---> Model Buiding
Building the LSTM
 
In order to build the LSTM, we need to import a couple of modules from Keras:

1. Sequential for initializing the neural network
2. Dense for adding a densely connected neural network layer
3. LSTM for adding the Long Short-Term Memory layer
4. Dropout for adding dropout layers that prevent overfitting

When defining the Dropout layers, we specify 0.2, meaning that 20% of the layers will be dropped. 
Thereafter, we add the Dense layer that specifies the output of 1 unit.

Now, it’s time to build the model. We will build the LSTM with different sets of neurons and 3 hidden layers. Finally, we will assign 1 neuron in the output layer for predicting the normalized stock price. We will use the MSE loss function and the Adam stochastic gradient descent optimizer.

---> Data visualization of Train & Test data on [Close] column

---> Prediction for single day & next 10 days 

---> Deployment on Streamlit

