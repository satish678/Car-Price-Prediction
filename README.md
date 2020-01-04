# Car-Price-Prediction
Predicting the car price based on certain independent features using Supervised Regression methods


This Repo helps in answering below questions.

1) Load the file “imports-85.data” into a dataframe from https://archive.ics.uci.edu/ml/machine-learning-databases/autos/imports-85.data and column names of this data set can be found here --https://archive.ics.uci.edu/ml/machine-learning-databases/autos/imports-85.names

2) Explain the problem statement. What are you predicting and what attributes you have to predict?

3) Browse a sample record from the dataframe. Are there any missing values?

4) How many records are available in the data set and how many attributes. Do you think the depth (number of records) is sufficient given the breadth? In other words, is the sample likely to be a good representative of the universe?

5) Analyse the data distribution for the various attributes and share your observations. 

6) Are there any independent attributes which have |R| close to 1?

7) Which attributes seem to have a stronger relationship with the dependent variable (Price of the car)?

8) Given the above analysis, which algorithm will be more suitable? Why?


4 IPYNB files are present for 4 different scenario:

Case 1: Applying get_dummies() on categorial variables and considering all the features. 
 
Conclusion: model performance good on train set (overfitting) but fails on test set (curse of dimensionality) 
 
Case 2: Applying LabelEncoder() on categorial variables and considering all the features 
 
Conclusion: model performance good on train set compared to test set 
 
Case 3: Applying LabelEncoder() on categorial variables and considering strong features whose R value close to 1 
 
Conclusion: model performance good on both train as well as test set 
 
Case 4: Using Stats model 
 
Conclusion: Helps in finding Actual predictors which have p<0.5 and model parameters with R square and Adjusted R square. 
