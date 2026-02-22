Experiment: Study of Pandas Library in Python
Aim

To study the Pandas library in Python and perform fundamental operations on Series and DataFrame objects.

Objectives

To understand the key features of the Pandas library

To create and manipulate Series and DataFrame

To perform data selection and filtering

To handle missing values

To read and write data using Pandas

Software Requirements

Python 3.x

Pandas Library

Jupyter Notebook / Google Colab / Python IDE

Theory

Pandas is an open-source Python library designed for data manipulation and analysis. It provides powerful and flexible data structures that make working with structured data easier and more efficient.

The two primary data structures in Pandas are:

1. Series

A one-dimensional labeled array capable of storing data of any type such as integers, strings, or floating-point numbers.

2. DataFrame

A two-dimensional labeled data structure organized in rows and columns, similar to a table or spreadsheet.

Pandas is widely used in:

Data cleaning

Data transformation

Statistical analysis

Exploratory Data Analysis (EDA)

It is built on the NumPy library and offers fast and efficient data handling capabilities.

Important Functions in Pandas
Function	Description
head()	Displays the first five rows of the dataset
tail()	Displays the last five rows of the dataset
info()	Provides information about dataset structure
describe()	Generates statistical summary of numerical data
loc	Label-based data selection
iloc	Position-based data selection
isnull()	Detects missing values
dropna()	Removes missing values
fillna()	Replaces missing values
Program
import pandas as pd

# Creating Series
s = pd.Series([10, 20, 30, 40])
print("Series:\n", s)

# Creating DataFrame
data = {
    "Name": ["A", "B", "C"],
    "Marks": [85, 90, 78]
}
df = pd.DataFrame(data)
print("\nDataFrame:\n", df)

# Display first rows
print("\nFirst 5 rows:\n", df.head())

# Statistical summary
print("\nDescription:\n", df.describe())

# Selecting column
print("\nMarks Column:\n", df["Marks"])
Output

Series object is created and displayed successfully

DataFrame is generated and printed

First five rows of the dataset are shown

Statistical summary of numerical data is displayed

Column selection operation is performed

Conclusion

Thus, the basic operations of the Pandas library, including the creation of Series and DataFrame, data viewing, statistical analysis, and data selection, were successfully studied and implemented.

