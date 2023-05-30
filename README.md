# CryptoPricePrediction
For this course project, I decided to predict the price trend of Binance, using both LSTM and ARIMA model. After comparing the results of the prediction, I foud LSTM provides a better accuracy than traditional statistical ARIMA model, while ARIMA model did a good job in the short term. 

This is a very simple project to practice and review the concepts of LSTM.

#### Steps:
I’m going to call API to extract the price of Binance as an example (one of the most popular cryptocurrencies in the market). My objective is to investigate and analyze the overall trend of change in Binance close price from 2018-12-25 to 2023-02-02 and predict the Binance price after 2023-02-02 (the latest 60 days). I would like to learn and try neural network we learned in class and see how it improves the traditional statistical model in predicting stock/cryptocurrencies price. 

As we have a time-series dataset, which is continuous, I’ll use the traditional ARIMA model as the reference model and test how LSTM performs with different loss functions and optimizers that can improve the price prediction. Here I choose MSE and RMSE as our evaluation metrics. 

After building several models, we found ML does a better job than ARIMA model and for LSTM - loss function MSE will perform better than MAE and based on the models we build, LSTM(100) with MSE and ADAM optimizer shows the best performance with lowest MSE and RMSE. 

Note: Binance is restricted in Ontario, so no matter how prediction goes, it’s just a project for the purpose of practice
