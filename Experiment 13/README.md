# **Experiment-14**
# **Title:** Data Binning and Data Formatting in Python

## **Aim**
To understand and implement data binning and data formatting techniques using different Python functions and operations.

## **Theory**
Data preprocessing is a crucial step in data analysis. It involves converting raw and unorganized data into a structured and meaningful form.

Two key preprocessing techniques are:

### **1. Data Binning**
Data binning is a technique used to group continuous numerical values into specific ranges or intervals known as bins.

It helps in:

* Reducing noise in the data
* Making analysis easier
* Transforming continuous data into categorical data

**Example:**

| Age | Category |
| --- | -------- |
| 18  | Young    |
| 30  | Adult    |
| 60  | Senior   |

### **2. Data Formatting**
Data formatting involves organizing and converting data into a proper structure so it can be easily analyzed and processed.

**Examples include:**

* Converting strings into numeric values
* Changing date formats
* Modifying text case
* Removing unnecessary spaces

Proper formatting ensures consistency and improves the accuracy of data.

**Functions / Operations for Data Binning**

### **1. Creating Bins**
**Function:** `pd.cut()`
This function is used to divide numerical data into equal-sized intervals (bins).

### **2. Creating Quantile-Based Bins**
**Function:** `pd.qcut()`
This method divides data into bins containing an equal number of data points.

### **3. Counting Values in Each Bin**
**Function:** `value_counts()`
This function shows how many values fall into each bin.

### **4. Assigning Custom Labels**
**Parameter:** `labels`
Used along with binning functions to give meaningful names to bins such as:

* Low
* Medium
* High

## **Functions / Operations for Data Formatting**

### **1. Checking Data Types**
**Attribute:** `dtypes`
Displays the data type of each column in a dataset.

### **2. Converting Data Types**
**Function:** `astype()`
Used to change one data type into another.

## **Examples:**

* String to integer
* Float to integer

### **3. Converting String to Numeric**
**Function:** `pd.to_numeric()`
Used when numerical values are stored as text.

### **4. Converting to Date Format**
**Function:** `pd.to_datetime()`
Converts values into a proper date format.

### **5. Changing Text Case**
**Functions:**

* `str.lower()`
* `str.upper()`
* `str.title()`

These functions help standardize text data.

### **6. Removing Extra Spaces**
**Function:** `str.strip()`
Removes unnecessary spaces from the beginning and end of strings.

### **7. Replacing Values**
**Function:** `replace()`
Used to substitute incorrect or inconsistent values with correct ones.

## **Conclusion**
Data binning and data formatting techniques were successfully understood and applied using various Python functions and operations.
