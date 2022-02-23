﻿# 100 DAYS OF MACHINE LEARNING
# DAY 1 

- **Step 1 :  Importing the required libraries.**
     
     ![enter image description here](https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/120px-NumPy_logo_2020.svg.png?20200723114325)
	![enter image description here](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/120px-Pandas_logo.svg.png?20200209204934)

- **Step 2 :  Importing the Data Set** 

	 We use the read_csv method of the Pandas library to                                 read a local CVS file as a dataframe.

- **Step 3 : Handling the Missing Data**
	There are no missing values in the data

- **Step 4: Encoding Categorial Data**

	Categorical data are variables that contain label values rather than numeric values. We import LabelEncoder class from sklearn.preprocessing library.

- **Step 5 : Splitting the dataset into test set and traning set**

	We make two partitions of dataset one for tranining the model called training the model called training set and other for testing the performance of the trained model called test set. We import train_test_split() method of sklearn.crossvalidation library.

- **Step 6 : Feature Scaling**

	After testing, we performed feature standardization or Z-score normalization. The StandardScaler of Sklearn.preprocessing is imported.

# DAY 2 
## SIMPLE LINEAR REGRESSION 
Simple linear regression is a method to predict dependent variable(Y) based on values of independent variables(X). It is assumed that the two variables are lenearly related. Hence, we try to find a linear function that predicts the response value(Y) as accurately as possible as a function of the feature or independent variable(X).
![enter image description here](https://miro.medium.com/max/960/1*jt-pyQQ7bgL2lyganse0nQ.png)
To establish notation for future use, we’ll use x(i) to denote the “input” variables (living area in this example), also called input features, and y(i) to denote the “output” or target variable that we are trying to predict (price). A pair (x(i), y(i)) is called a training example, and the dataset that we’ll be using to learn—a list of m training examples (x(i),y(i)); i=1,...,m—is called a training set. Note that the superscript “(i)” in the notation is simply an index into the training set, and has nothing to do with exponentiation. We will also use X to denote the space of input values, and Y to denote the space of output values. In this example, X = Y = ℝ. 

To describe the supervised learning problem slightly more formally, our goal is, given a training set, to learn a function h : X → Y so that h(x) is a “good” predictor for the corresponding value of y. For historical reasons, this function h is called a hypothesis. 



# DAY 3
## MULTIPLE LINEAR REGRESSION

Multiple linear regression attempts to model the relationship between two or more features and response by fitting a linear equation to observed data. The steps to perform multiple linear regresion are  almost similar to that of simple linear regression. The difference lies in the evaluation. You can use it to find out which factor has the highest impact on the predicted output and how factor has highest impact on the predicted output and how different variables relate to each other.

![enter image description here](data:image/png;base64,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)
