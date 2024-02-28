# Yes-Bank-Stock-Closing-Price-Prediction---Regression-
The objective is to predict closing stock price of the month for Yes Bank Dataset.

Introduction
Provided with Yes Bank Stock Closing Price Prediction dataset, main objective is to do some analysis, model implementation and predict the stock’s closing price of the month.

Problem Statement
Yes Bank Stock Closing Price Prediction 
Yes Bank is a well-known bank in the Indian financial domain. Since 2018, it has been in the news because of the fraud case involving Rana Kapoor. Owing to this fact, it was interesting to see how that impacted the stock prices of the company and whether Time series models or any other predictive models can do justice to such situations. This dataset has monthly stock prices of the bank since its inception and includes closing, starting, highest, and lowest stock prices of every month. The main objective is to predict the stock’s closing price of the month. 

Dataset Information
The provided Dataset is of Yes Bank which consists detail of Stocks based on its High, Low and Opening prices. The provided dataset of Yes Bank have in total 185 rows and 5 columns. This rows and columns have Yes Banks details such as monthly stock prices of the bank since its inception and includes closing, starting, highest, and lowest stock prices of every month. The main objective is to predict the stock’s closing price of the month. Following are the details of all columns present:
Date- Date of record for stocks
Open – Opening price of stocks
High – Highest price in the day for stocks
Low – Lowest price in the day for stocks
Close – Closing price of stock
Data Preprocessing and Visualization
1.Handling Null & Duplicate Values
•	There were no null values present in dataset.
•	No duplicate values present in dataset.

2.Converting Datatypes
•	All columns datatype were correct except Date column.
•	Converted column Date to datetime data type

3.Creating New columns
•	Created new column ‘Year’,’Month’ with the help of Date column.
•	Created new column named as ‘independent_mean’ by taking mean of Open, High and Low columns.
While analyzing data, we obtain some important insights like in which year stock price was highest? From which year stock prices got effected and started declining. Data visualization, in general makes complex data easy to understand and get significant insights from that entire dataset, so we used visualization which gave lots of insights of dataset, many questions were answered using graphs and visual plots. The graphs and visual plots used in this project are as follows:
Distribution plot
Scatter plot
Box plot
Pair Plot
Line Chart
Coorelation Heatmap
For this visualization mainly seaborn & matplotlib library were used.

Model Implementation
The entire dataset needs to be divided into training and testing set, After Transformation and Scaling of Data model implementation takes place. Linear Regression Model, Lasso and Ridge Regularization models, Random Forest and Support Vector Regressor are the models that have been used. For better performance of model, hyperparameter tuning have been performed. Evaluated the performance of all models using metrics such as MAE, RMSE. Compared the models with each other to select a best model with better performance and low rate of error. 

Conclusion
The conclusion drawn after entire data cleaning, processing, analysing, visualizing and implementing different machine learning models are as follows:


**Conclusion drawn after Data Analysis and Visualization are as follows:**

1.The dataset consists of stock information in which no null and missing values are present.

2.Independent variable of dataset such as Open, High, Low have strong correlation with each other due to which multicollinearity exists.

3.Open, High and Low variable data are positively skewed data which needs to be transform so that data can be distributed close to normal.

4.Dependent Variable Close is also positively skewed data.

5.Variation in the stock price can be seen since 2008 till 2016 but after 2016 there has been rapid increase in pricing of stocks.

6.Stock price has been increased since 2016 to 2018 but after 2018 stock prices have been decreased continously.

7.Highest price of stock was recorded as 404.0 in month 2018.

8.Lowest price of stock was recorded as 5.55 in month 2020.

9.Independent Variable such as Open, High and Low have strong linear relationship with dependent variable Close.

10.There are some outliers present in the dataset but as the dataset is very small dropping those outliers can lead of data loss.

**Conclusion drawn after Model Implementation:**

For Machine Learning model implementation, Linear Regression, Lasso and Ridge regularization models, Random Forest and Support Vector Regressor have been used.

At first basic implementation started with linear regression model which gave decent training and test score

Then used Lasso and Ridge Regression model and got impressive training and testing score with low MAE and RMSE score compare to the base model.

Implemented Random Forest model which gave better training and testing score compare to any other model

Then finally implemented Support Vector Regressor model which seems to be performing bad as compare to other models with training score and testing score
