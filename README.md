# Predicting the amount of precipitation using KNN and MLR

## Objective

Increase in global warming has given rise to climate change at much extent, where predicting rainfall has become a crucial part in many sectors, especially agricultre. Most of the environmental elements are co related to each other where they can be used to predict the change/value in one or more variables if being provided as input to right statistical method. Predicting the amount of rainfall based on other climatic observation, while revealing the hidden patterns between the dependent and independent variables will be beneficial for water resource management as well as agricultural planning.

Considering the above assumption, and following the motivation, in this study, we predict the amount of precipitation using Machine Learning Algorithm, based on various factors such as wind speed and direction, temperature range, latitude, longitude and many others, which we discussed in detail, below

## Methodology

For this research we will use K(Knowledge) D(Discovery) D(Database), which is KDD methodology with intention to fulfull our predefined goal and answer the stated research questions. As KDD method is structured in a way to understand the hidden patterns in the data, it is believed to be ideal for and not limited to 1. Find relationship between variables 2. Assign classes to input data, 3. Cluster data based on their features, which further supports regression, classification and clustering as few of many Data Mining applications[1]. KDD is formed of severals steps with Data Mining as one of its, with the aim to undertand the pattern and draw insights(model), the steps altogether with data mining make the process suitable where we intend to solve crucial problems using large data set. The steps are described as below:

1. Data Extraction - Here we extract the data and integrate it if needed, basically defining and confirming the dataset on which we perform knowledge discovery is identified.

2. Data Cleaning and Preprocessing - Here we deal with missing values, outliers and type of data.

3. Data Redundancy and Transformation - Here we evaluate the effectiveness of features based on correlation matrix(pearson coeeficient), lasso regression and other methods and remove the least effective ones, we check for covariance and deal with them according to the requirement. Further we transform the data using log, square root ot any other transformation idealogy to appropriate the weightage of each feature in order to prepare the data ready for the model.

4. Data Mining - Here we choose the appropriate model based on the data and direction of the discovery as well as apply the model to gain the results.

5. Interpretaion of the patterns - The Outputs are visualized and the patterns are further understood to draw useful isights

Evaluation - Here we evaluate/compare each model performace with other model and state the improtance of each metrics while gain an idea of which model perfroms better.

## Dataset

We downloaded the dataset from Kaggle, which was in a csv file
The dataset consisted of numerous columns as Country.Region	Province.State	time	summary	icon	sunriseTime	sunsetTime	moonPhase	precipIntensity	⋯	temperatureMinTime	temperatureMax	temperatureMaxTime	apparentTemperatureMin	apparentTemperatureMinTime	apparentTemperatureMax	apparentTemperatureMaxTime	Lat	Long	precipAccumulation, where precipAccumulation is the target column.
Here we drop off the columns which doesnt fit our motive and have least effect on calculating precipitation.
Thus we remove X, Country.Region, Province.State, time, summary, icon, precipType as they are characters with numerous values as well they have least affect on precipitation.

Further, we scale the data using cube root scaling to make it ready to fit on the models

## Machine Learning Models

##### Multiple Linear Regression
##### K- Nearest Neighbor

## Evaluation

We evaluate both models based on the following parameters

MLR results - 
R-squared:  0.9361423 MSE:  0.0004723808 MAE:  0.01584654  RMSE:  0.02173432

KNN results - 
R-squared: 0.4313803	MSE: 6.704781e-05	MAE: 0.008190637	RMSE: 0.003512344




