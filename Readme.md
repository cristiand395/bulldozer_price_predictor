# Bulldozer Predictor - Regression Machine Learning Model
In this project I'm going to build a regression model to predict bulldozer price.


I use the following framework to build this model from scratch
![machine learning framework](./images/framework.png)

# 1. Problem Definition:
Can we predict the price of bulldozer base on the previous data about it?

# 2. Data:
The dataset used in this project was downloaded from the following source of Kaggle.
https://www.kaggle.com/c/bluebook-for-bulldozers/data

There are 3 datasets:

* Train.csv - Historical bulldozer sales examples up to 2011 (close to 400,000 examples with 50+ different attributes, including SalePrice which is the target variable).
* Valid.csv - Historical bulldozer sales examples from January 1 2012 to April 30 2012 (close to 12,000 examples with the same attributes as Train.csv).
* Test.csv - Historical bulldozer sales examples from May 1 2012 to November 2012 (close to 12,000 examples but missing the SalePrice attribute, as this is what we'll be trying to predict).

# 3. Evaluation:
Kaggle has set the evaluation metric to beign root mean squared log error (RMSLE). After we finish our model, we are going to compare it with other results from others on Kaggle.

# 4. Features:
Kaggle provide us a data dictionary which contains information about each attribute of the dataset. Its located in './data/Data Dictionary.xlsx'

# Modeling: 


# Experiment:

# Conlusion:

## Notes:


### Libraries:
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Scikit-learn

