#Experiment – 11  
#Title: Categorical Data Analysis using Python

##Aim  
To perform categorical data analysis using Python by identifying categories, calculating frequency distributions, performing cross-tabulation, and visualizing categorical variables.

---------------------------------------------------------------------

##Theory

###1. Categorical Data

Categorical data refers to data that represents groups, labels, or categories instead of numerical values. It describes qualities or characteristics and cannot be measured numerically.

Examples:
• Gender (Male, Female)  
• Product Category (Electronics, Clothing, Grocery)  
• Payment Method (Cash, Card, UPI)  
• Customer Type (New, Returning)

Categorical data is widely used in business analytics, marketing analysis, social sciences, and survey data analysis.

---------------------------------------------------------------------

###2. Types of Categorical Data

Nominal Data

Nominal data represents categories that do not have any natural order or ranking. These values are only used as labels.

Examples:
• Department (IT, CSE, Mechanical)  
• City (Pune, Mumbai, Delhi)  
• Blood Group (A, B, AB, O)

In this type of data, the categories cannot be arranged in any meaningful sequence.

Ordinal Data

Ordinal data represents categories that have a meaningful order or ranking. However, the difference between categories cannot be measured numerically.

Examples:
• Satisfaction Level (Poor, Average, Good, Excellent)  
• Education Level (Diploma, Graduate, Postgraduate)

Although these categories follow an order, the difference between them is not defined.

---------------------------------------------------------------------

###3. Importance of Categorical Data Analysis

Categorical data analysis helps in:

• Understanding the distribution of categories  
• Identifying relationships between variables  
• Summarizing data for better decision making  
• Detecting patterns and trends in data

For example:

• Which product category is sold the most?  
• Which payment method is preferred by customers?  
• How customer types vary across different cities?

---------------------------------------------------------------------

###4. Common Operations in Categorical Data Analysis

1. Frequency Count

Frequency count determines how many times each category appears in the dataset.

Example:

Electronics → 3  
Clothing → 3  
Grocery → 2  

In Python, this is done using the function:
value_counts()

--------------------------------------------------

2. Unique Category Identification

This operation helps identify the distinct categories present in a dataset.

Example:
UPI, Card, Cash

In Python, this is done using:
unique()

--------------------------------------------------

###3. Cross-Tabulation

Cross-tabulation is used to analyze the relationship between two categorical variables.

Example:

Product Category     UPI     Card     Cash  
Electronics           2       0        1  
Clothing              0       2        1  

This helps identify patterns between variables.

In Python, this is done using:
pd.crosstab()

--------------------------------------------------

###4. Grouping of Data

Grouping helps summarize data based on categories.

Example:
Number of orders by product category.

In Python, this is done using:
groupby()

---------------------------------------------------------------------

###5. Role of Python in Categorical Data Analysis

Python provides powerful libraries for analyzing categorical data.

Library        Purpose  
Pandas         Data manipulation and analysis  
Matplotlib     Data visualization  
Seaborn        Advanced statistical visualization  

These libraries help in organizing, analyzing, and visualizing categorical datasets efficiently.

---------------------------------------------------------------------

#Conclusion

Categorical data analysis helps in understanding patterns, relationships, and distributions within qualitative data. Python libraries such as Pandas, Matplotlib, and Seaborn provide efficient tools to analyze and visualize categorical datasets.
