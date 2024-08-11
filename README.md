# Stock-Prediction-using-LSTM
I tried to use an LSTM model to train and test on Nifty-50 fifteen years (minute-wise) data.

LSTMs are excellent for time-series analysis, especially when the next prediction can be made by using a fixed window size.
Furthermore, there might be more than one logical analysis of the prices to predict the next price, hence the multiple heads of an LSTM.
The data used here give the stock prices per minute. But an LSTM is unbelievably accurate even for such a volatile and unpredictable situation.

Since the stock prices are volatile and do not heavily depend on prices of the far past, I used a window size of 14.
That is, based on the last 14 prices, the 15th price is predicted.
