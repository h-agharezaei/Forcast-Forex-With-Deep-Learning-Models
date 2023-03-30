# Forcast-Forex-With-Deep-Learning-Models

This code retrieves financial data from Tiingo API and trains a SimpleRNN neural network model on the EURJPY currency pair's historical data to make predictions.

The following libraries are used in this code:

* pandas
* numpy
* matplotlib
* seaborn
* requests
* datetime
* scipy
* pylab
* statsmodels
* sklearn
* keras
* tensorflow


After importing the required libraries, the code sets the necessary variables such as the API key, start and end dates for the data retrieval, the financial asset's ticker symbol, and the interval for resampling. The retrieved data is saved in an Excel file using the pandas library.

The data is then preprocessed, which includes converting the 'date' column to a datetime format, dropping the 'ticker' column, setting the 'date' column as the index, and plotting the probability distribution and ACF plots of the 'high' column.

The data is then split into training and testing sets, and MinMax scaling is applied to both input and output data. The RNN model is then defined, compiled, and trained using the training set. Finally, the model's performance is evaluated using the testing set, and the training history is saved for further analysis.


******

Do you want to predict the EURJPY exchange rate? Check out my latest project on GitHub!

I have built a machine-learning model to forecast the EURJPY exchange rate using historical data from the past two years. By analyzing the data, I identified patterns and trends in the market that helped me create a model that accurately predicts future rates.
To develop this model, I had to overcome several challenges, including:
🔹 Data Collection: Collecting data from a reliable source was challenging. I used the Tiingo API to retrieve data for the last two years, which required an API key.
🔹 Data Preprocessing: The data collected was in JSON format, and it was necessary to clean and transform it into a pandas data frame to be usable in machine learning models.
🔹 Feature Engineering: I experimented with different time intervals and lag periods to determine the best features for the model. I used statistical techniques such as probability plots, ADF tests, and histograms to analyze the data and select the best features.
🔹 Scaling Data: The scale of the data was an important consideration when using machine learning models. I used the MinMaxScaler from the scikit-learn library to scale the data to a range of 0 to 1.
Using a combination of different machine learning models, including LSTM, GRU, SimpleRNN, and Dense layers, I built a forecasting model that predicts the EURJPY exchange rate with high accuracy. The model is trained on a dataset of 17,520 data points and tested on 4,380 data points.
