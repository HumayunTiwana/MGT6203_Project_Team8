# MGT6203_Project_Team8

PERFORMANCE ANALYSIS AND PRICE PREDICTION FOR ASX 200
Introduction:
The aim of the project is to:

	Forecast the performance of ASX 200 Stock over i time period.
	Understanding factors contributing to the performance of ASX 200 stock in comparison with other US Market indices (S&P 500, Nasdaq etc.) 

The institutions and individuals are interested in understanding the performance of the stock market and predicting the future stock prices, be it a long-term holder or a day-trader. The investors and institutions need to decide where to invest and the best time to sell, buy or hold a share in the stock market based on the available information. This Project would enable investors to invest into stocks with more confidence level and high return probability.
Our team compromises of people with diverse experience which include a stock trading SME and a Finance & Investments SME, this would fuel up the project with real life/industry expert input.
ASX 200 daily stock for a period of 10 years (01/07/2010 to 30/06/2020) was used in this research. Due to the time zone differences between Australia and most of the world, Australians have an advantage of knowing what happens in markets elsewhere in the world before the Australian market (ASX) is open in the morning (Sydney time). This prior knowledge provides a perfect opportunity for arbitrage. In the hands of a savvy day-trader, or a shrewd long-term investor, this information gives you the advantage of predicting the ASX and achieve potentially significant financial gains.
Data Sets and Potential Data Sources:
This dataset is collected from various reliable public-domain sources and compiled by the author (YasAli) on Kaggle. Similar datasets can be obtained from various sources i.e., Yahoo Finance, OFX, federal banks etc. 
As per exploratory data analysis performed on this dataset, the author has worked on the factors affecting ASX200, below were some interesting insights.
-	ASX200 Correlated well with the US indices, but it correlated better with European Indices
-	French CAC40 seems to be the best predictor for the Aussie market.
-	No correlation to Asian Market found.





Description of Datasets and Key Variables:
This dataset contains daily closing prices for 41 global markets from 01/07/2010 to 30/06/2020. These 41 market indicators are considered as significant measures of various external factors that may affect the performance of the Australian Stock Market, as represented by the ASX200.
Those indicators are presented in the table below:
Variables	Category	Reasons/Comments
ASX200 Closing Price	Dependent Variable (Y)	Performance metrics for ASX200
Date, Month of Date	Independent variables (X)	Date dimension
FTSE100, S&P500, NASDAQ, DAX, CAC40, Nikkei 225, Shanghai, Hangseng, Dow Jones	Independent variables (X)	Nine major stock market indices from the USA, Europe, and Asia.
Fed-rate, RBA-rate	Independent variables (X)	Official interest rates by the RBA and the US Feds, as indicators of affinity of foreign funds to Australia
GBP; SGD; USD; EUR; 10 AED 10 CNY; 10,000 IDR; 100 INR 100 JPY; 1000 KRW	Independent variables (X)	The exchange rate of the $AU against 10 world currencies that are most relevant to Australia's international trade.
Germany 1yr, Singapore 1yr, Korea 1yr, US 1yr, Swiss 1yr, Japan 1yr, AU 1yr, China 1yr, UK 1yr, Hong Kong 1yr	Independent variables (X)	Yield rates for governments-issued short-term bonds by 10 countries from Western and Asian economies, as measures of relative availability of credit and cross-border investment
Germany 30yr, Singapore 30yr, Korea 20yr, US 30yr, Swiss 30yr, Japan 30yr, Au 10yr, China 30yr, UK 30yr, Hong Kong 10yr	Independent variables (X)	Yield rates for governments-issued long-term bonds by 10 countries from Western and Asian economies, as measures of relative availability of credit and cross-border investment
Screenshot of Dataset / Link:
Screenshot of dataset and link of the source location is given below:
https://www.kaggle.com/yasali/predict-the-asx200?select=ASX200.csv
 






List of Models to Be Used:

We are approaching to target this challenge as a time series problem, since our hypothesis is ‘The future value of the stock is correlated with the past and the current values’. One of our group members is a SME in Stock Markets, his input also makes us believe the same.

We would also be incorporating other exogenous variables in the models that would help to identify any added signals necessary for the model to forecast accurately. The Models which we would experiment are as following.


ARIMA	Autoregressive Integrated Moving Average (ARIMA) will try to forecast time series as it’s based on the idea that the information in the past values of the time series can alone be used to predict the future values

SARIMA	SARIMA stands for Seasonal Autoregressive Integrated Moving Average. It extends the ARIMA model by adding a linear combination of seasonal past values and forecast errors.

VAR	The Vector Autoregression (VAR) method models the next step in each time series using an AR model. The VAR model is useful when you are interested in predicting multiple time series variables using a single model

Recurrent Neural Network
	RNN can model sequence of data so that each sample can be assumed to be dependent on previous ones

Long Short-Term Memory (LSTM)	(LSTM) networks are a modified version of recurrent neural networks, which makes it easier to remember past data in memory. LSTM is well-suited to classify, process and predict time series given time lags of unknown duration.
 
Since we would trying different models with different configurations and will choose the best model based on our 'Metric of Interest’ which could be:
 
-        Mean Absolute Error
-        Root Mean Squared Error
-        Mean Absolute Percentage Error (MAPE)
 
We intend to consume R Language, Tableau (for EDA), Microsoft Word, and Excel where required for the deliverables.

Conclusion:
We want to explore the dataset to validate the correlation between ASX200 and other market indices. We anticipate the ASX200 to follow other market trends in Asia, Europe and USA. Also, it would be interesting to see the relationship of currencies and bonds on market behavior which we are anticipating as highly correlated. We would like to slice and dice on the dataset to explore more dimensions and insights.





Brief Bio of Team # 8:

My name is Muhammad Aamer Zaman, currently residing in Saudi Arabia. I graduated from NUST in 2001 with majors in Telecommunication Engineering. I’ve been working across the Middle East in the field of Network Optimization and since the last 9 years I've been working in the domain of Customer Experience and analytics. I expect to learn analyzing business data and bringing actionable insights which can deliver value to the business and the customers.

My name is Humayun Akram Tiwana, currently residing in Australia. I graduated from U.E.T Lahore in 2007 with majors in Electrical Engineering. I’ve been working across the Middle East and Asia Pacific in the field of data analytics. I expect to harness my data analytical skills to add value to business through informed decision making.

I am Joudat Hashmi, currently residing in Saudi Arabia. I graduated from Comsats University Islamabad in 2008 with majors in system programming. I have been working across multiple industries since 14 years which include Analytics Consultancy, Telecom IT and Cx, City Development, Smart city across multiple organizations in PAK, KSA and UAE. I have a knack for seeing solutions in sprawling data sets by concentrating on portfolios of “data use cases” that address opportunities which businesses face.

My name is Ali Riaz, currently residing in Abu Dhabi, U.A.E. I graduated as a Mechanical Engineer in 2013 from Khalifa University, Abu Dhabi - U.A.E. For the past 8 years, I have been working in the Oil & Gas and Petrochemical Industries as a Mechanical Engineer and have always been fascinated by the vast amount of data we deal with. I expect to learn and develop skills in different methods of statistical analysis as well as necessary programming knowledge for better decision making.

I am Imran Khan; residing in Abu Dhabi, UAE, having undergraduate in commerce and graduated with majors in economics from University of Karachi in 2010; besides I am a certified chartered accountant (ACCA, UK). I have been working for more than 12 years in the audit and finance field and have dealt with financial data since then. I hope to acquire and foster abilities in various techniques of data analytics to assist the organization to meet its strategic objectives.

References:

[1] Ariyo, A. A., Adewumi, A. O., & Ayo, C. K. (2014). Stock price prediction using the Arima model. 2014 UKSim-AMSS 16th International Conference on Computer Modelling and Simulation. https://doi.org/10.1109/uksim.2014.67.
[2] C. Angadi, M., & P. Kulkarni, A. (2015). Time Series Data Analysis for Stock Market Prediction using Data Mining Techniques with R. International Journal of Advanced Research in Computer Science, 6(6), 104–108.
[3] Islam, M. R., & Nguyen, N. (2020). Comparison of financial models for stock price prediction. Journal of Risk and Financial Management, 13(8), 181. https://doi.org/10.3390/jrfm13080181.







