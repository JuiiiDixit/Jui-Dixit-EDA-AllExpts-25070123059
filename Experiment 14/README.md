# Experiment – 14 
# Title: Data Normalization and Converting Categorical Variables into Quantitative Variables in Python  

## Aim  
To study data normalization techniques and convert categorical variables into numerical form using different Python functions and operations.  

---------------------------------------------------------------------

## Theory  

In data analysis and machine learning, raw datasets often contain numerical values with different ranges and categorical variables. Before performing analysis, the data must be preprocessed so that it becomes suitable for calculations and model building. Data preprocessing improves the quality of data and helps in obtaining more accurate and meaningful results.  

Two important preprocessing techniques used for this purpose are:  

• Data Normalization  
• Categorical Variable Encoding  

These techniques help improve data consistency, reduce errors, and increase the efficiency of data analysis.

---------------------------------------------------------------------

### 1. Data Normalization  

Definition  

Data normalization is a preprocessing technique used to scale numerical data into a common range so that all variables contribute equally during analysis. In many real-world datasets, numerical features may have very different ranges, which can affect the performance of data analysis and machine learning algorithms.

For example:

Feature Range  
Price 500 – 50000  
Rating 1 – 5  
Units Sold 10 – 1000  

In this example, the values of Price are much larger compared to Rating. Without normalization, features with larger values may dominate the smaller ones, leading to biased or incorrect results.

Normalization helps convert all numerical values into a similar scale without changing the relationship between the original data values. It improves the stability of calculations and makes the dataset easier to understand and analyze.

Normalization helps to:

• Standardize the scale of data  
• Improve the performance and accuracy of machine learning models  
• Reduce the effect of large value differences  
• Make comparison between variables easier  
• Improve visualization and interpretation of data  
• Reduce chances of calculation errors caused by large numbers  

Normalization is especially important when datasets contain multiple numerical columns measured in different units such as price, quantity, weight, or ratings.

---------------------------------------------------------------------

## Types of Normalization  

### 1. Min-Max Normalization  

This method scales values between 0 and 1 using the minimum and maximum values of the dataset. Each value is adjusted proportionally within the new range.

Functions / Operations used:  
min()  
max()  

These functions help find the smallest and largest values needed for scaling.

--------------------------------------------------

### 2. Z-score Normalization (Standardization)  

This method transforms data using the mean and standard deviation of the dataset. It measures how far each value is from the average value of the column.

Functions / Operations used:  
mean()  
std()  

--------------------------------------------------

### 3. Decimal Scaling  

In this method, values are scaled by shifting the decimal point so that all values fall within a smaller range.

Operation used:  
Division by powers of 10  

---------------------------------------------------------------------

## Useful Functions for Normalization  

Summary Statistics  

Function used:  
describe()  

This function displays important statistical values such as:

• Mean  
• Standard deviation  
• Minimum value  
• Maximum value  

--------------------------------------------------

## Identify Data Types  

Function used:  
dtypes  

This function helps identify numerical columns that require normalization.

--------------------------------------------------

## Select Columns  

Functions used:  
loc[]  
iloc[]  

These functions are used to select specific columns on which normalization is applied.

---------------------------------------------------------------------

### 2. Converting Categorical Variables into Quantitative Variables  

#### Definition  

Many datasets contain categorical variables that represent qualitative information instead of numbers. These variables describe labels or groups and cannot be directly used in mathematical calculations.

Examples:

Variable Values  
Gender Male, Female  
Payment Method UPI, Debit Card  
Product Category Electronics, Clothing  

Most data analysis methods require numerical input, so categorical data must be converted into numerical form. This process is known as categorical encoding.

---------------------------------------------------------------------

## Methods to Convert Categorical Data  

### 1. Label Encoding  

In this method, each category is assigned a unique numeric value.

Example:

Category Encoded Value  
Male 0  
Female 1  

Functions / Operations used:  
LabelEncoder()  
fit_transform()  

--------------------------------------------------

### 2. One-Hot Encoding  

This method creates separate binary columns for each category. Each column represents one category, and values are marked as 1 or 0.

Example:

Category Electronics Clothing Home  
Electronics 1 0 0  

Function used:  
get_dummies()  

--------------------------------------------------

### 3. Dummy Encoding  

This method is similar to One-Hot Encoding, but one column is removed to avoid duplication and redundancy between variables.

Function used:  
get_dummies(drop_first=True)  

---------------------------------------------------------------------

## Conclusion  

Thus, data normalization and methods for converting categorical variables into numerical values were studied using various Python functions and operations. These techniques improve data consistency and prepare the dataset for accurate analysis and further processing.
