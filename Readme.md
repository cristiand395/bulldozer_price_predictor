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
For this project we chosse classification models, all that scikit-learn can give us.
Models that we tried:
- Logistic Regression
- RandomForestClassifier
- Linear SVC
- KNeighborsClassifier
![models no tunning compare](./images/models_no_tunning_compare.png)

# Experiment:
Trying all the models for classification and after tunning we choose `Logistic Regression` with somes specific hyperparameters because give us the best the best performance.

# Conlusion:
* Because this dataset its limited (about 300 samples), we could not reach our goal to obtain at least 90% accuracy, but we absolutly find out some interesting things about this reserach and trained a model to predict with 86% of accuracy if a patient has or no Heart Disease.
* The plots that we created could be use as a reference in future researches about this topic, maybe try a different model to improve the accuracy.

## Notes:
* Chest pain its the most importance variable to predict if a patient has heart disease or not, at least with this dataset and in the same environtment.
* The best estimiator is Logistic Regression tunned with the parameters defined with the GridSearchCV.
- All the plots created in this notebook are located in './images'

![features importance](./images/features_importance.png)


### Libraries:
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Scikit-learn

