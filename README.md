# Forecasting_S&P500_Stock_Prices_with_LSTM

The S&P 500 is a stock market index featuring the top 500 publicly traded companies in the United States. It is often used to get a general understanding of how the U.S. economy is performing. The aim of this project is to create a LSTM model that forecasts S&P 500 closing stock prices. The S&P 500 Index closing prices will provide a general overview of closing prices and behavior of most large U.S. stocks.

The source data is from Yahoo! Finance consisting of S&P 500 five-year historical data from February 28th, 2017 to February 28th, 2022. Because COVID-19 impacted the stock market during the last two years, the probable new cases per day from the Centers for Disease Control and Prevention is also used in a few model experiments. The input and output data are preprocessed into time step lags that to be inputted into the model. Each model and its performance will be analyzed to recommend the best S&P 500 forecaster model among the models experimented. Please refer to the report for the model experiments. 

The LSTM models were able to successfully capture temporal correlations that provided context for the predicted closing price for the next day. From these experiments, the best model was Experiment A.1, the single layer LSTM with an input of closing price and time step of 30. The test MAE score was 0.03. The  addition of the COVID-19 probable new cases data did not result in a big difference in performance. Experiment A.1 seemed to best predict the dips and spikes and able follow upward and downward trends.
