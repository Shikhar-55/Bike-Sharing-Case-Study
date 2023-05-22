# Bike-Sharing-Case-Study


This repository contains the code and documentation for building a demand prediction model for a bike-sharing system. The model aims to understand the factors that affect the demand for shared bikes in the American market and provide insights for business planning and strategy.

### Problem Statement
BoomBikes, a bike-sharing provider in the US, has experienced a decline in revenue due to the ongoing Corona pandemic. To prepare for the post-lockdown period and accelerate their revenue growth, BoomBikes wants to understand the demand for shared bikes among the people once the situation improves. By identifying the significant variables that affect bike demand and analyzing their impact, BoomBikes aims to develop a strategy to cater to the increased demand and differentiate themselves from competitors.

The consulting company contracted by BoomBikes has gathered a large dataset on daily bike demands across the American market, considering various meteorological surveys and people's styles. The goal is to model the demand for shared bikes using the available independent variables and gain insights into the demand dynamics of the market.

### Business Goal
The business goal of this project is to develop a demand prediction model that accurately captures the relationship between various features and the demand for shared bikes. The model will help the management understand how demand varies with different factors and guide them in formulating the business strategy to meet customer expectations and optimize operations. Additionally, the model will provide valuable insights into the demand dynamics of a new market.

### Data Preparation
The dataset provided contains several variables, such as 'weathersit' and 'season,' with numeric values (1, 2, 3, 4) that have associated labels (as described in the data dictionary). However, these numeric values do not represent an ordered relationship between the labels. It is recommended to convert such feature values into categorical string values before proceeding with model building. Please refer to the data dictionary for a better understanding of all the independent variables.

Another important consideration is the 'yr' column, which has values 0 and 1 representing the years 2018 and 2019, respectively. Although it may seem reasonable to drop this column due to having only two values, it actually provides valuable information about the increasing demand for bike-sharing systems over time. Carefully consider whether to include or drop this column based on its potential predictive power.

### Model Building
In the provided dataset, three columns named 'casual,' 'registered,' and 'cnt' are present. 'casual' represents the number of rentals made by casual users, 'registered' represents the total number of rentals made by registered users, and 'cnt' represents the total number of bike rentals, including both casual and registered users. The model should be built using 'cnt' as the target variable for demand prediction.

### Model Evaluation
After building the model, conducting residual analysis, and making predictions on the test set, it is essential to evaluate the model's performance.

### Dependencies
The following dependencies are required to run the code in this repository:

Python 3.7+

NumPy

pandas

scikit-learn

Matplotlib

Jupyter Notebook

Ensure that these dependencies are properly installed
