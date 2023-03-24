# RR Diner Coffee

![image](https://user-images.githubusercontent.com/86930309/227387324-7433daa7-cff3-4520-9279-4c154c380ac5.png)

In this case study, you’ll become the lead data scientist for an up-and-coming specialty coffee company seeking to use customer data to justify critically important
business decisions. You will use scikitlearn to build four different decision tree models — two using entropy and two using gini impurity — to ascertain whether a 
potentially business-transforming deal with a mysterious coffee farm in China will take your business to the next level. 

The case study will involve your use of the full data science pipeline, from importing, loading and cleaning the data right through to modeling and concluding. In the
case study, your decision trees will properly implement the supervised learning method of classification, and you will enforce the best practices of:

- Making an appropriate train/test split
- One-hot encoding
- Model evaluation
- Restricting the maximum depth of the tree
- Using random forest to increase predictive accuracy and control overfitting

## 1. Sourcing and loading

Import packages
Load data
Explore the data

## 2. Cleaning, transforming and visualizing

- Cleaning the data
- Train/test split

To execute the train/test split properly, we need to do five things:

a. Drop all rows with a null value in the Decision column, and save the result as NOPrediction: a dataset that will contain all known values for the decision

b. Visualize the data using scatter and boxplots of several variables in the y-axis and the decision on the x-axis

c. Get the subset of coffeeData with null values in the Decision column, and save that subset as Prediction

d. Divide the NOPrediction subset into X and y, and then further divide those subsets into train and test subsets for X and y respectively

e. Create dummy variables to deal with categorical inputs

- Visualize the data

![image](https://user-images.githubusercontent.com/86930309/227389110-e3312092-4a90-4e66-9930-8273332e0fca.png)

There is a wide range of customers that spent money last week on the coffee and that said yes they would buy the hidden farm coffee. The median was 40 dollars. A majority of the customers that said no they would not buy the hidden farm coffee was from 0-30 dollars with a median of 25 dollars.

## 3. Modelling

- Model 1: Entropy model - no max_depth
- Model 2: Gini impurity model - no max_depth
- Model 3: Entropy model - max depth 3
- Model 4: Gini impurity model - max depth 3

## 4. Evaluating and concluding

- How many customers will buy Hidden Farm coffee?

Only 69.23 % would potentially buy the Hiddden Farm coffee by our gini model with a max depth of 3.

- Decision

## 5. Random Forest

- Import necessary modules
- Model

The RF model predicts a higher rate of potenital customers that will buy the hidden coffee of 82.89%.

- Revise conclusion

The random forest is the best model. Its accuracy score is relevent compared to the others and predicts that more customers would potiental purchase the Hidden Farm coffee. Given that the other model predicted that 69.23% would purchase the coffee and the random forest model predicted 82.89%, I would recommend that they go ahead and create a contract with Hidden Farms to produce the coffee.
