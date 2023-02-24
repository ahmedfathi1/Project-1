# Sales Repository prediction insights
## We are looking at the Item sales of different goods and how well different store types perform in selling goods in hopes to predict future sales of goods. 

**Author**: Ahmed Fathi

### Business problem: We want to know how well the item sales are in order to predict.


### Data: https://docs.google.com/spreadsheets/d/e/2PACX-1vT7T4OEvxCrrx8SNk2CNc9yyApd4S8_rhhT2p2zqCeptIaPmGiSlh-bKDDYQ6beipefWAOvzlb_glAe/pub?output=csv
For this dataset, there were 8523 rows and 12 columns


## Methods: The data was cleaned and the following processes were performed


## Explanatory Data Analysis


![Bar viz](https://user-images.githubusercontent.com/115515293/202751002-4d31031a-2272-4c5d-ae7c-b6c4ceead2b4.png)


> Using a histogram to look at the number of products based on their Item group. We can see that a large majority of goods are grouped in fruits and vegetables and snack foods.

![Hist viz](https://user-images.githubusercontent.com/115515293/202751167-e79fc263-3ae5-4581-b02c-772b8be18b70.png)


> Box plot used to look at the statistics of item sales based on the type of store. From this graph we can see that supermarket Type3 have the most amount of sales.


## Model

There were two models used for evaluation (Linear Regression and Regression Tree). The final model used was a Regression Tree Model which was tuned to a max_depth of 5.

Results for training data: 
 MSE 1171332.784431318,
 RMSE: 1082.281287111312,
 R^2: 0.6042066848171654 
 
Results for Test data: 
 MSE 1114615.8633462703,
 RMSE: 1055.7536944506849,
 R^2: 0.5960039728227073

The training set had about 60% variance in y and the testing had about 59% variance in y.


## Recommendations: I would recommend implementing the Regression Tree Model as it fits both the training and testing sets pretty well in comparrison to the linear regression model used in the code.



# Focussing on Importances and Coefficients and seeing how they differ between LinearRegression and RandomForest

## LinearRegression Model
(https://github.com/ahmedfathi1/Sales-Repository/blob/main/LinearRegression_Plot.png)
The top 3 Coefficients that the LinearRegression model shows to be impactful are Outlet_Type_Supermarket_type_3, Outlet_Establishment_year_1999, and Outlet_Type_Supermarket_type_1 based on the fact that they are the 3 that have the highest impact on Item_Outlet_Sales based on the graphic.

## RandomForest Model
(https://github.com/ahmedfathi1/Sales-Repository/blob/main/RandomForest_Plot.png)
Based on our RandomForest model, the top 5 features are:
- Item_MRP
- Outlet_Type_Grocery Store
- Item_Visibilty
- Item_Weight
- Outlet_Type_supermarket Type 3

### For further information


For any additional questions, please contact **a.fathi111@gmail.com**
