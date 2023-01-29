# Project Title : Seoul Bike Sharing Demand Prediction
![image](https://user-images.githubusercontent.com/102457644/196049024-eb6e2099-b768-467c-88ad-8b6af3a28bb0.png)
## Problem Description
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.
## Data Description
The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.
## Attribute Information:
* Date : year-month-day
* Rented Bike count - Count of bikes rented at each hour
* Hour - Hour of he day
* Temperature-Temperature in Celsius
* Humidity - %
* Windspeed - m/s
* Visibility - 10m
* Dew point temperature - Celsius
* Solar radiation - MJ/m2
* Rainfall - mm
* Snowfall - cm
* Seasons - Winter, Spring, Summer, Autumn
* Holiday - Holiday/No holiday
* Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)

## Business Use Case:
* A bike rental company can use a machine learning regression model to predict the demand for bikes in certain areas at specific times. This information can be used to optimize the distribution of bikes, ensuring that there are enough bikes in high-demand areas and reducing the number of bikes in low-demand areas. This can help the company to save on transportation costs and increase efficiency in bike distribution.
* This model can also be used in similar business problems where we need to predict the deamand of certain item.

## Data Pre-Processing
* Got the descriptive information of the data.
* checked for null values if any
* Checked for Outliers

## Exploratory Data Analysis Feature Engineering
* Used Libraries such as matplotlib.pyplot and seaborn to visualize the data
* Found the distribution of target variable positively skewed hence applied Square root transformation to it.
* separated numerical and catagorical features and checked for their distribution using histplot
* checked corelation with heatmap and found high corelation between Temperature and dew point temperature.  
* applied one hot encoding to categorical features.

## Model training
* defined funvtions to train linear and non-linear models and get their performance metrics
* Performance metrics used were MSE,RMSE,R@ score, adjusted r2 score
* defined a fuction for feature importance
* splitted data into training and testing
* Scaled training and testing sets of independent variables using StandardScaler 
* trained models such as linear regression, L! and L2 regression, KNN, Decision trees, Random forest,Gradient Boost, CatBoost.
* Found CatBoost as the best model with Adjusted r2 score of 90%.
