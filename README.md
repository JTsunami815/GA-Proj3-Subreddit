# Project-2: Ames-House-Price-Prediction

## Contents:
___
* [Summary](#Summary)
* [Problem Statement](#Problem-Statement)
* [Resources](#Resources)
* [Data Dictionary](#Data-Dictionary)
* [Recommedations & Conclusions](#Recommedations-&-Conclusions)
___

## Summary
___
The Ames Housing Data Set contains information from the Ames Assessor’s Office used in computing the value of individual residential properties sold in Ames, Iowa from 2006 to 2010, as well as the actual eventual sale prices for the properties.

The data set contains information for more than 2000 properties. The initial data dictionary outlines, which will not be illustrated, have more than 75 descriptive variables. Some are **nominal** (categorical), meaning they are non-numerical and lack clear-cut order (IE: Neighborhood, Type of roofing). Some are **ordinal**, meaning they are categorical but have a clear order (IE: External Quality (Excellent, Good, Average, Poor)). Some are **discrete**, meaning they are numerical but at set intervals (IE: Year Built, Garage Cars). The rest are **continuous**, meaning they are numerical and can theoretically take any value in a range (IE: 1st Floor Square Feet, 2nd Floor Square Feet, Basement Square Feet).

In this project, I have attempted to craft as accurate of a model as possible for predicting housing sale prices, using regression techniques, enhanced by feature engineering, feature selection, and regularization.The Ames data set was divided into a training set and a test set. I aim to accurately predict the withheld sale prices for the test set, based on the features and prices in the training set. 

[Return to Contents](#Contents:)

## Problem Statement
___
The main purpose of this project is to predict the home prices in Ames, Iowa by using regression models. After doing this data analysis, theoretical relationship can be found with what we have in mind. Throughout the progressive iterative modeling and feature selection processes in both manually and automatic, we can gain a deeper insight into variables which were directly correltes to property sales and understand better the mechanism behind various models.

[Return to Contents](#Contents:)

## Resources
___
To get a better understanding on what resides in Ames, Iowa, videos and online sites provided additional research materials. Sources from reputable YouTube content creators to websites in real estate, best places to live, and others were used to add values on top of the provide data.

**Data:**
* [Train CSV](train.csv)
* [Test CSV](test.csv)
* [Complete Dictionary](../datasets/data_description.txt)

**3rd Party**
- [The 2020 Top 100 Best Places to Live in America](https://livability.com/best-places/top-100-best-places-to-live/2020/ames-ia/)
- [Quickloan](https://www.quickenloans.com/learn/things-look-shopping-next-home)
- [Top House-Hunting Mistakes](https://www.investopedia.com/articles/mortgage-real-estate/09/buy-house-emotion-free.asp)
- [Iowa Home Buyer's Handbook](https://www.greatiowahomes.com/buyers/handbook.cfm)

[Return to Contents](#Contents:)

# Data Dictionary
___
The dictionary table below represents the only columns that are left from the total number of columns.
### Dictionary Key:
___

### Dictionary Key:
___

   |Feature|Type|Dataset|Description|
|- | -|- | -|
|**OverallQual**|integer|full_num_train_df|Rates the overall material and finish of the house|
|**YearBuilt**|integer|full_num_train_df|Original construction date|
|**YearRemod/Add**|integer|full_num_train_df|Remodel date|
|**MasVnrArea**|integer|full_num_train_df|Masonry veneer type|
|**ExterQual**|integer|full_num_train_df|Evaluates the quality of the material on the exterior|
|**BsmtQual**|integer|full_num_train_dfn|Evaluates the height of the basement|
|**TotalBsmtSF**|integer|full_num_train_df|Evaluates the total square footage of the basement| 
|**HeatingQC**|integer|full_num_train_df|Heating quality and condition|
|**1stFlrSF**|integer|full_num_train_df|First Floor square feet|
|**GrLivArea**|integer|full_num_train_df|Above grade (ground) living area square feet| 
|**FullBath**|integer|full_num_train_df|Full bathrooms above grade| 
|**KitchenQual**|integer|full_num_train_df|Kitchen quality|
|**TotRmsAbvGrd**|integer|full_num_train_df|Total rooms above grade (does not include bathrooms)|
|**Fireplaces**|integer|full_num_train_df|Number of fireplaces|
|**GarageFinish**|integer|full_num_train_df|Interior finish of the garage|
|**GarageCars**|integer|full_num_train_df|Size of garage in car capacity|
|**GarageArea**|integer|full_num_train_df|Size of garage in square feet|
|**SalePrice**|integer|full_num_train_dfn|The price of unit|
|**Foundation_PConc**|integer|full_num_train_df|Type of foundation|
|**HouseAge**|integer|full_num_train_df|The age of the house|
|**RemodelAge**|integer|full_num_train_df|The age of the house after remodelled|
|**TotalBthrm**|integer|full_num_train_df|The total number of bathrooms in the unit|
|**TotalSqFt**|integer|full_num_train_df|The total square feet of the unit|
|**GarageOverall**|integer|full_num_train_df|The overall square footage of the garage space|
___
[Return to Contents](#Contents:)

# Recommedations & Conclusions
____
The idea behind this study is to allow both home buyers and sellers to understand what are the top few features to takeaway before they dive into the market.  They can also utilize the model to assist them on predicting an approriate house value that does not over nor under sale to the market value.  

Built feature engineering on various features were expected to be significant determinants of house prices. The engineered data ran through three linear regression models: OLS, Ridge and Lasso. The assorted property size variables, namely living area, basement finished area, lot area and garage area, were all found to be positively correlated to the sale price. Build quality and condition were also found to be among the most important determinants of house prices.

This is believed to be a good starting point for consumers to use to get the fundamental idea of what to look out for or how to market their property.  Futher in-depth studies can be conducted in future where we can dive deeper into each feature and break it down even further to give the customers better results.  Some ideas would be public transportation, proximity to nearby parks, eateries, entertainment, etc, and many more.  
___

**Side Note:** 

If I want to improve the score for this, I would consider to change the way the columns were dropped.  Instead of dropping with a written function, I should of used lasso function to aggressively get ride of the noise and low correlation variances then followed up by the written function.  This may change my end result of this project.

[Return to Contents](#Contents:)
