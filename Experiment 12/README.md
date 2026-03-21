# Experiment – 12  
# Title: Data Preprocessing and Handling Missing Values in Python  

## Aim  
To study data preprocessing techniques and handle missing values using different Python functions and operations.  

---------------------------------------------------------------------

# Theory  

Data preprocessing is an important step in data analysis. It involves cleaning and preparing raw data before performing analysis or building machine learning models.  

In real-world datasets, data often contains problems such as:  

• Missing values  
• Incorrect data formats  
• Duplicate records  
• Inconsistent or invalid values  

Handling these issues improves the overall quality of the data and helps produce more accurate analysis results.  

One of the most common preprocessing tasks is handling missing values.  

Missing values may appear in different forms such as:  

• NaN (Not a Number)  
• NULL values  
• Blank cells  
• Special symbols like ?, -, NA  

---------------------------------------------------------------------

### Data Preprocessing Functions / Operations  

#### 1. Display First Records  

This operation displays the first few rows of the dataset. It helps in quickly viewing the structure of the data.  

Function used:  
head()  

--------------------------------------------------

#### 2. Display Last Records  

This operation displays the last few rows of the dataset.  

Function used:  
tail()  

--------------------------------------------------

#### 3. Display Dataset Information  

This function provides information about the dataset such as the number of rows, columns, data types, and presence of missing values.  

Function used:  
info()  

--------------------------------------------------

#### 4. Check Data Types  

This function shows the data type of each column in the dataset.  

Function used:  
dtypes  

--------------------------------------------------

#### 5. Identify Missing Values  

This function detects missing values in the dataset and returns True wherever a missing value is present.  

Function used:  
isnull()  

--------------------------------------------------

#### 6. Count Missing Values  

This function counts the total number of missing values in each column.  

Function used:  
isnull().sum()  

--------------------------------------------------

#### 7. Detect Non-Missing Values  

This function identifies valid (non-missing) values in the dataset.  

Function used:  
notnull()  

--------------------------------------------------

#### 8. Replace Missing Symbols  

Sometimes missing values appear as special symbols such as ?. These symbols can be replaced with NaN values.  

Function used:  
replace()  

---------------------------------------------------------------------

### Methods to Handle Missing Values  

#### 1. Remove Rows with Missing Values  

This method removes rows that contain missing data.  

Function used:  
dropna()  

--------------------------------------------------

#### 2. Remove Columns with Missing Values  

This method removes columns that contain missing values.  

Function used:  
dropna(axis=1)  

--------------------------------------------------

#### 3. Fill Missing Values  

This method replaces missing values with a specified value.  

Function used:  
fillna()  

--------------------------------------------------

#### 4. Replace Missing Values with Mean  

This method replaces missing numerical values with the mean (average) of the column.  

Functions used:  
mean()  
fillna()  

--------------------------------------------------

#### 5. Replace Missing Values with Median  

This method replaces missing numerical values with the median value of the column. It is useful when the dataset contains outliers.  

Functions used:  
median()  
fillna()  

--------------------------------------------------

#### 6. Replace Missing Values with Mode  

This method replaces missing values using the most frequently occurring value in the column. It is mainly used for categorical data.  

Functions used:  
mode()  
fillna()  

--------------------------------------------------

#### 7. Forward Fill Method  

This method replaces missing values using the previous value in the column.  

Function used:  
fillna(method='ffill')  

--------------------------------------------------

#### 8. Backward Fill Method  

This method replaces missing values using the next available value in the column.  

Function used:  
fillna(method='bfill')  

---------------------------------------------------------------------

Other Preprocessing Operations  

Remove Duplicate Records  

This function removes duplicate rows from the dataset.  

Function used:  
drop_duplicates()  

--------------------------------------------------

Count Unique Values  

This function counts the number of unique values present in a column.  

Function used:  
nunique()  

--------------------------------------------------

Display Unique Values  

This function displays all distinct values present in a column.  

Function used:  
unique()  

---------------------------------------------------------------------

## Conclusion  

Thus, data preprocessing techniques and methods for handling missing values were studied using various Python functions. These operations help improve data quality and prepare the dataset for further analysis.
