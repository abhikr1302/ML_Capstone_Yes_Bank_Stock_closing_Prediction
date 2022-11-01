# ML_Capstone_Yes_Bank_Stock_closing_Prediction

# Introduction: - 

Fluctuations in stock prices are notoriously difficult to predict. For decades, economists have created complicated mathematical models that ultimately fail to describe share price movements. With the evolved technology we are now using Machine Learning algorithms to study the pattern and predict.

Yes Bank is an Indian bank headquartered in Mumbai, India and was founded by Rana Kapoor and Ashok Kapoor in 2004. In June 2005 it went public with the issue price of ₹35.  In September 2018, the then appointed CEO of Yes Bank, Rana Kapoor was alleged in a fraud case thus he was ordered by Kapoor to step down from his CEO position in January 2019. 
		   
We are here trying to study the stock price pattern and did it get affected by this fraud case using our knowledge about Python and ML algorithms.

# Problem Statement: -

We have been given a dataset of 185 entries with 5 features which gives a study about this stock Pattern over 15 years. We will then identify the independent and the dependent features to conduct our study. Then using EDA and ML we will study the below: -

1. Prediction of Yes bank Stock close Price
2. Effect of the Rana Kapoor fraud case on the stock price
3. Performing Regression Analysis using Multiple models to predict the Yes Bank Stock Close Price and compare the best fit model.

# DATASET:

The compact dataset given to us has monthly stock prices of the bank since its commenced and the features are closing, starting, highest and lowest prices of every month. The objective is to predict the dependent feature i.e stock’s closing price of the month.
Dataset contains following features--

1. Date: contains the month and year of investment. 
2. Open: the price at which a security first trades when an exchange opens for the day.
3. Close: the last price at which a stock trades during a regular trading session.
4. High: a data point on a stock chart that shows the highest value that a stock reached during a trading day
5. Low:  the lowest price at which a specific stock trades over the course of a trading day.

# Workflow: -

The solution code is divided into the following sections:

I. Data Study: First we will import multiple libraries required to perform the study and then load the CSV file. Later perform some operations to understand and analyze the data.

II. Data Manipulation: Since Dataset contains int64, float64, datetime64 type of data and no Null Values in the Dataset cleaning is not needed.

III. EDA and DATA Visualization 

Fluctuations in stock prices are notoriously difficult to predict. For decades, economists have created complicated mathematical models that ultimately fail to describe share price movements. With the evolved technology we are now using Machine Learning algorithms to study the pattern and predict.

Yes Bank is an Indian bank headquartered in Mumbai, India and was founded by Rana Kapoor and Ashok Kapoor in 2004. In June 2005 it went public with the issue price of ₹35.  In September 2018, the then appointed CEO of Yes Bank, Rana Kapoor was alleged in a fraud case thus he was ordered by Kapoor to step down from his CEO position in January 2019. 
		   
We are here trying to study the stock price pattern and did it get affected by this fraud case using our knowledge about Python and ML algorithms.

# Problem Statement: -

We have been given a dataset of 185 entries with 5 features which gives a study about this stock Pattern over 15 years. We will then identify the independent and the dependent features to conduct our study. Then using EDA and ML we will study the below: -

1. Prediction of Yes bank Stock close Price
2. Effect of the Rana Kapoor fraud case on the stock price
3. Performing Regression Analysis using Multiple models to predict the Yes Bank Stock Close Price and compare the best fit model.

# DATASET:

The compact dataset given to us has monthly stock prices of the bank since its commenced and the features are closing, starting, highest and lowest prices of every month. The objective is to predict the dependent feature i.e stock’s closing price of the month.
Dataset contains following features--

1. Date: contains the month and year of investment. 
2. Open: the price at which a security first trades when an exchange opens for the day.
3. Close: the last price at which a stock trades during a regular trading session.
4. High: a data point on a stock chart that shows the highest value that a stock reached during a trading day
5. Low:  the lowest price at which a specific stock trades over the course of a trading day.

# Workflow: -

The solution code is divided into the following sections:

I. Data Study: First we will import multiple libraries required to perform the study and then load the CSV file. Later perform some operations to understand and analyze the data.

II. Data Manipulation: Since Dataset contains int64, float64, datetime64 type of data and no Null Values in the Dataset cleaning is not needed.

III. EDA and DATA Visualization 

1. Year-Wise Study of Open and Close-
![download (1)](https://user-images.githubusercontent.com/110467640/198999293-21c580f3-e603-444d-b91b-c3265ec7a074.png)

This Data is between June 2005 to Nov 2020. Initially it opened around 20 till the peak value upto around 370. Then we can see after the fraud case in 2018 involving Rana Kapoor the Open value drastically drops with a small jump in 2019 and then further drops. Closing Value almost shadows the Open value.

2. Year-Wise Study of High and Low- 

![download (2)](https://user-images.githubusercontent.com/110467640/198999364-a174d868-fb33-42f2-b8f6-391bb8187bd1.png)

This study follows the similar trend as the above graph. There is growth till 2018 and then the fraud case affects the growth thus dropping in both High and low price.

IV. Data Distribution: A Study of all possible values for a variable and also the relative frequency. 

![download (3)](https://user-images.githubusercontent.com/110467640/198999441-d5aff457-a7ca-43c4-b342-b1b3b26cb32f.png)
![download (10)](https://user-images.githubusercontent.com/110467640/198999776-5657c355-fa74-47ce-b673-48cb0aa88bd0.png)
![download (11)](https://user-images.githubusercontent.com/110467640/198999809-82b08c23-231a-4c4f-a95c-1397ba682ad5.png)

It shows that the mean and median have significant differences indicating the data is not evenly distributed. 

![download (4)](https://user-images.githubusercontent.com/110467640/198999615-cfab9147-5941-4cf1-b96c-c89407614570.png)

                                          Data is negatively skewed.



V. Normalization: Normalization is the process of structuring a relational database in accordance with a series of normal forms in order to reduce data redundancy and improve data integrity. Log transformation is applied to normalize the data. 

![download (12)](https://user-images.githubusercontent.com/110467640/199000751-dd1b00f5-0b07-47b7-b234-2966444eedc8.png)
![download (13)](https://user-images.githubusercontent.com/110467640/199000759-7ea73ea2-e4e2-45e3-99ef-07b1c291f80b.png)
![download (14)](https://user-images.githubusercontent.com/110467640/199000765-afa416dc-3c95-4c71-b598-ae8b950a557d.png)

After applying the Log Transformation it is seen that the data is evenly distributed and also the difference between mean and median is minimal. After applying the log transformation normal distribution curve is achieved for the skewed data.
 
 ![download (5)](https://user-images.githubusercontent.com/110467640/199001051-380efe68-3eae-4bad-9440-8f15f7a07692.png)
 
VI. Heatmap: This shows the collective representation of correlation between all the features.

![download (9)](https://user-images.githubusercontent.com/110467640/199001124-165c9878-a7d9-49b1-9ca1-8a37b26c7d06.png)

VII. Correlation: Close is considered to be the dependent variable whereas the rest 3  High, Open, Low are the dependent variables. Here it's seen that the correlation is very high between each independent variable and the dependent variable.

![download (15)](https://user-images.githubusercontent.com/110467640/199001369-3881852c-9e28-40f6-ab62-6da2c248c615.png)
![download (16)](https://user-images.githubusercontent.com/110467640/199001387-0a55ae0a-b6ba-454b-a27f-d0ee8990bef2.png)
![download (17)](https://user-images.githubusercontent.com/110467640/199001399-869286e9-27e2-4c29-bfb1-75c2fe583f40.png)

VIII. Multicollinearity and VIF
| Variables | VIF |
|---|---|
| Open | 175.185704 |
| High | 167.057523 |
| Low | 71.574137 |

This table represents that there is high collinearity between independent variables.

IX. Train/Test Model: The library used to split the dataset: from sklearn.model_selection import train_test_split
 Train : Test ratio : 80:20
 
![Hold-out-method-for-model-evaluation](https://user-images.githubusercontent.com/110467640/199001450-abba9e3c-e7ae-4bf9-a6e7-5a6e4c5d60a3.png)

IX. Model Training with cross validation and hyper parameter tuning

1. Linear Regression: Linear Regression is the supervised Machine Learning model in which the model finds the best fit linear line between the independent and dependent variable. This calculator is built for simple linear regression, where only one predictor variable (X) and one response (Y) are used.

![download (18)](https://user-images.githubusercontent.com/110467640/199001814-093bb3e7-9ab6-46b9-8a14-0c8d6565a2db.png)

2. Ridge Regression: Ridge regression is a type of linear regression technique that is used in machine learning to reduce the overfitting of linear models. It is a model tuning method that is used to analyses any data that suffers from multicollinearity.

![download (19)](https://user-images.githubusercontent.com/110467640/199001877-54524e32-0c70-4eb8-8468-ba01adbaf309.png)

3. Lasso Regression: Lasso regression is a modification of linear regression, where the model is penalized for the sum of absolute values of the weights. It is used over regression methods for a more accurate prediction. This model uses shrinkage. Shrinkage is where data values are shrunk towards a central point as the mean. The lasso procedure encourages simple, sparse models.

![download (20)](https://user-images.githubusercontent.com/110467640/199001924-3880ff39-df97-4c4a-84c6-2b21ba9b45a5.png)

4. ElasticNet Regression: Elastic net linear regression uses the penalties from both the lasso and ridge techniques to regularize regression models. The technique combines both the lasso and ridge regression methods by learning from their shortcomings to improve the regularization of statistical models.

![download (21)](https://user-images.githubusercontent.com/110467640/199002057-c6b0d0fa-8513-4a75-a731-51dc550bc19c.png)

X. Matrix Comparison
| Model_Name | MSE | MAE | RMSE | R2 | Adjusted R2 |
|----|----|----|-----|----|----|
| Linear Regression | 0.031583 | 0.151285 | 0.177715 | 0.822570 | 0.806440 |
| Elastic Net Regression | 0.031589 | 0.152095 | 0.178764 | 0.820468 | 0.804147 |
| Lasso regression | 0.032040 | 0.152317 | 0.178996 | 0.820001 | 0.803638 |
| Ridge regression | 0.032679 | 0.153352 | 0.180773 | 0.816411 | 0.799721 |

# Conclusion: -

From the above study we can say that Linear regression has the best R2 and Adjusted R2 score hence Linear Regression is the best model.
