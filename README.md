The objective of this project is to analyze historical gold prices from January 1950 to July 2020 
and develop forecasting models to predict future prices. Gold has been a valuable asset and 
understanding its price trends can provide insights for investors and economists. 


Data Preparation
1. Data Loading: 
o The dataset, named gold_monthly_csv.csv, is loaded into a Pandas DataFrame. 
o The dataset contains two columns: Date and Price, representing the monthly 
gold prices. 
2. Data Inspection: 
o The first few rows of the dataset are examined using df.head(). 
o The dataset consists of 847 rows and 2 columns. 
o The date range of the dataset spans from January 1950 to July 2020. 
3. Data Cleaning: 
o A new column, month, is created using a date range from January 1950 to July 
2020. 
o The original Date column is dropped, and the month column is set as the index 
of the DataFrame. 
Data Exploration 
1. Descriptive Statistics: 
o A summary of the gold prices is generated using df.describe(), providing insights 
into the mean, standard deviation, and range of prices. 
2. Data Visualization: 
o A line plot visualizes the trend of gold prices over time. 
o A box plot is created to visualize the distribution of gold prices across diƯerent 
years and months. 
3. Time Series Analysis: 
o The data is resampled to calculate yearly, quarterly, and decade averages, 
allowing for trend analysis over diƯerent time frames.
Modeling and Forecasting 
1. Splitting Data: 
o The dataset is divided into training (up to 2015) and testing (2016 and beyond) 
sets to evaluate model performance. 
2. Linear Regression Model: 
o A linear regression model is fitted using time as the independent variable to 
predict gold prices. 
o The Mean Absolute Percentage Error (MAPE) is calculated to evaluate the 
model's accuracy, resulting in a MAPE of 29.76%. 
3. Naive Forecast Model: 
o A naive forecasting model is applied, predicting that future prices will remain 
constant at the last observed price. 
o The MAPE for this model is significantly lower, at 19.38%. 
4. Exponential Smoothing Model: 
o The Exponential Smoothing model (additive trend and seasonal components) is 
fitted to the training data. 
o This model provides a MAPE of 17.24%, indicating improved accuracy over the 
previous models. 
5. Forecasting Future Prices: 
o The Exponential Smoothing model is used to forecast future gold prices for the 
test set. 
o Confidence intervals for the predictions are calculated and visualized. 
Results 
 Linear Regression: MAPE of 29.76%
 Naive Forecast: MAPE of 19.38%
 Exponential Smoothing: MAPE of 17.24%
The Exponential Smoothing model shows the best predictive performance among the models 
evaluated, suggesting that it eƯectively captures the trends and seasonality in gold price data.
Visualizations 
 The following visualizations were created during the analysis: 
o Line plots showing monthly gold prices over time. 
o Box plots for price distributions across years and months. 
o Predictions from the Exponential Smoothing model with confidence intervals. 
Conclusion 
This project successfully analyzed historical gold prices and developed forecasting models. The 
Exponential Smoothing model outperformed other models in terms of accuracy, indicating its 
suitability for time series forecasting in this context. The insights derived from this analysis can 
be beneficial for investors and stakeholders interested in gold market trends.
