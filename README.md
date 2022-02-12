# 100 DAYS OF MACHINE LEARNING
# DAY 1 

- **Step 1 :  Importing the required libraries.**
     ![enter image description here](https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/120px-NumPy_logo_2020.svg.png?20200723114325)
![enter image description here](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/120px-Pandas_logo.svg.png?20200209204934)

- **Step 2 :  Importing the Data Set** 
We use the read_csv method of the Pandas library to read a local CVS file as a dataframe.

- **Step 3 : Handling the Missing Data**
There are no missing values in the data

- **Step 4: Encoding Categorial Data**
Categorical data are variables that contain label values rather than numeric values. We import LabelEncoder class from sklearn.preprocessing library.

- **Step 5 : Splitting the dataset into test set and traning set**
We make two partitions of dataset one for tranining the model called training the model called training set and other for testing the performance of the trained model called test set. We import train_test_split() method of sklearn.crossvalidation library.

- **Step 6 : Feature Scaling**
After testing, we performed feature standardization or Z-score normalization. The StandardScaler of Sklearn.preprocessing is imported.

