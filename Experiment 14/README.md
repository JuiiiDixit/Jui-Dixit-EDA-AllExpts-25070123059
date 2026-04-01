# Experiment – 13  
# Title: Data Normalization and Converting Categorical Variables into Quantitative Variables using Scikit-learn in Python  

## Aim  
To study data normalization techniques and convert categorical variables into numerical form using Scikit-learn and various Python functions and operations.  

---------------------------------------------------------------------

## Theory  

In data analysis and machine learning, raw datasets often contain numerical values with different ranges and categorical variables. Before performing analysis, the data must be preprocessed so that it becomes suitable for calculations and model building. Data preprocessing improves the quality of data and ensures better accuracy in results.

Two important preprocessing techniques used for this purpose are:

• Data Normalization  
• Categorical Variable Encoding  

These techniques help improve data consistency, reduce errors, and increase the efficiency of data analysis.

Scikit-learn is a powerful Python library used for machine learning and data preprocessing. It provides built-in functions for normalization, scaling, and encoding categorical data, making preprocessing faster and more efficient.

---------------------------------------------------------------------

### 1. Data Normalization  

## Definition  

Data normalization is a preprocessing technique used to scale numerical data into a common range so that all variables contribute equally during analysis. In many real-world datasets, numerical features often have very different ranges, which can affect the performance of data analysis and machine learning algorithms.

For example:

Feature Range  
Price 500 – 50000  
Rating 1 – 5  
Units Sold 10 – 1000  

In this example, the values of Price are much larger compared to Rating. Without normalization, features with larger values may dominate smaller ones, leading to incorrect analysis results.

Normalization converts numerical values into a similar scale without changing the relationship between original data values.

Normalization helps to:

• Standardize the scale of data  
• Improve performance and accuracy of models  
• Reduce the effect of large value differences  
• Make comparison between variables easier  
• Improve visualization and interpretation of data  

---------------------------------------------------------------------

## Types of Normalization  

### 1. Min-Max Normalization  

This method scales values between 0 and 1 using minimum and maximum values.

Functions used:  
min()  
max()  
MinMaxScaler()  

--------------------------------------------------

### 2. Z-score Normalization (Standardization)  

This method standardizes data using mean and standard deviation.

Functions used:  
mean()  
std()  
StandardScaler()  

--------------------------------------------------

### 3. Decimal Scaling  

In this method, values are scaled by shifting the decimal point so that all values fall within a smaller range.

Operation used:  
Division by powers of 10  

---------------------------------------------------------------------

#### Useful Functions for Normalization  

describe()  
Displays summary statistics such as mean, minimum, maximum, and standard deviation.

dtypes  
Displays the data types of columns.

loc[]  
Used to select specific rows or columns using labels.

iloc[]  
Used to select specific rows or columns using index positions.

---------------------------------------------------------------------

### 2. Converting Categorical Variables into Quantitative Variables  

### Definition  

Categorical variables represent qualitative data such as names, labels, or groups. Since most machine learning algorithms require numerical input, categorical data must be converted into numerical form. This process is known as categorical encoding.

Examples:

Variable Values  
Gender Male, Female  
Payment Method UPI, Debit Card  
Product Category Electronics, Clothing  

---------------------------------------------------------------------

## Types of Encoding Methods  

### 1. Label Encoding  

In Label Encoding, each category is assigned a unique numeric value.

Example:

Category Encoded Value  
Male 0  
Female 1  

Functions used:  
LabelEncoder()  
fit()  
transform()  
fit_transform()  

--------------------------------------------------

### 2. One-Hot Encoding  

In One-Hot Encoding, separate binary columns are created for each category.

Example:

Category Electronics Clothing Home  
Electronics 1 0 0  

Functions used:  
get_dummies()  
OneHotEncoder()  
fit_transform()  

--------------------------------------------------

### 3. Dummy Encoding  

Dummy Encoding is similar to One-Hot Encoding, but one column is removed to avoid redundancy between variables.

Function used:  
get_dummies(drop_first=True)  

---------------------------------------------------------------------

## Scikit-learn Library  

Scikit-learn is a widely used Python library designed for machine learning and data preprocessing tasks. It provides tools for scaling numerical data, encoding categorical variables, and building machine learning models. The library simplifies preprocessing by providing ready-to-use classes such as scalers and encoders.

Common Modules Used:

sklearn.preprocessing  

This module contains functions used for scaling and encoding data.

---------------------------------------------------------------------

## Theory of Functions Used  

min()  
Returns the smallest value in a dataset or column.

max()  
Returns the largest value in a dataset or column.

mean()  
Calculates the average value of numerical data.

std()  
Calculates the standard deviation, showing how values vary from the mean.

describe()  
Generates summary statistics including count, mean, minimum, maximum, and standard deviation.

dtypes  
Displays data types of dataset columns.

loc[]  
Selects data using row or column labels.

iloc[]  
Selects data using index numbers.

MinMaxScaler()  
Used to scale numerical data between 0 and 1 using minimum and maximum values.

StandardScaler()  
Used to standardize numerical data by removing the mean and scaling to unit variance.

LabelEncoder()  
Converts categorical labels into numerical form.

fit()  
Learns parameters from the data.

transform()  
Applies transformation to the data.

fit_transform()  
Performs both fitting and transformation in a single step.

OneHotEncoder()  
Converts categorical variables into binary numeric columns.

get_dummies()  
Converts categorical variables into dummy or binary variables.

get_dummies(drop_first=True)  
Performs dummy encoding by removing one column to prevent redundancy.

---------------------------------------------------------------------

## Conclusion  

Thus, data normalization and categorical encoding techniques were studied using Scikit-learn and various Python functions. These techniques help standardize numerical values and convert categorical data into numerical form, making datasets suitable for machine learning and data analysis.
