Experiment 10
Creating and Uploading Dataset using Pandas
Aim
To create a dataset using a dictionary in Python, convert it into a Pandas DataFrame, save it as a CSV file, and perform basic data inspection operations such as shape, size, info(), describe(), head(), and tail().
Theory
A dataset is a structured collection of related data arranged in rows and columns. In Python, datasets are handled using the Pandas library. Pandas provides a data structure called a DataFrame, which is used to store and manipulate tabular data efficiently.
A DataFrame is a two-dimensional labeled data structure with rows and columns. Each column can store different types of data such as integers, strings, or floating-point values.
Datasets in Pandas can be created manually using Python data structures like dictionaries, or they can be imported from external files such as CSV, Excel, JSON, or SQL databases.
Basic data inspection functions are used to understand the structure and summary of the dataset. These functions help identify the number of rows and columns, data types of columns, presence of missing values, and statistical details of numerical data.
The commonly used inspection functions are:
df.shape: Returns the number of rows and columns in the dataset.
df.size: Returns the total number of elements in the dataset.
df.info(): Provides information about column names, data types, and non-null values.
df.describe(): Generates statistical summary of numerical columns.
df.head(): Displays the first five rows of the dataset.
df.tail(): Displays the last five rows of the dataset.
df.columns: Displays the column names of the dataset.
Saving a dataset as a CSV file is done using the to_csv() function. A dataset can be reloaded using the read_csv() function.
Conclusion
Thus, the dataset was successfully created using a dictionary and converted into a Pandas DataFrame. Basic inspection operations such as shape, size, info(), describe(), head(), and tail() were performed to analyze the dataset structure and statistical details. The dataset was also saved as a CSV file and successfully uploaded again. This experiment helped in understanding basic data creation, storage, and analysis using the Pandas library.
