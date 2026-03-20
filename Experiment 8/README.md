## Experiment8: Introduction to NumPy
### Aim
To study the NumPy library and perform basic operations on NumPy arrays.

### Objectives
To create NumPy arrays
To perform mathematical operations on arrays
To understand array attributes and indexing
To use built-in NumPy functions

Software Requirements
Python
NumPy library
Jupyter Notebook / Google Colab / Python IDE

### Theory
NumPy (Numerical Python) is a library used for numerical computations.
It provides a powerful N-dimensional array object and functions for performing mathematical operations efficiently.
Advantages of NumPy:
Faster than Python lists
Requires less memory
Supports vectorized operations
Provides mathematical and statistical functions

### Procedure
## 1. Import NumPy
import numpy as np

## 2. Create NumPy Array
a = np.array([10, 20, 30, 40])
print(a)

## 3. Create Array with Zeros, Ones and Range
print(np.zeros(4))
print(np.ones(4))
print(np.arange(1, 10, 2))

## 4. Check Array Attributes
a = np.array([[1, 2, 3], [4, 5, 6]])

print(a.ndim)    # number of dimensions
print(a.shape)   # size of array
print(a.size)    # total number of elements
print(a.dtype)   # data type

## 5. Reshape the Array
a = np.array([1, 2, 3, 4, 5, 6])
print(a.reshape(2, 3))

## 6. Mathematical Operations
a = np.array([10, 20, 30])
b = np.array([1, 2, 3])

print(a + b)
print(a - b)
print(a * b)
print(a / b)

## 7. Statistical Operations
a = np.array([10, 20, 30, 40])

print(np.mean(a))
print(np.sum(a))
print(np.max(a))
print(np.min(a))
print(np.std(a))

## 8. Indexing and Slicing
a = np.array([10, 20, 30, 40, 50])

print(a[1])
print(a[1:4])

### Output
NumPy arrays were created
Mathematical operations performed successfully
Statistical values calculated
Array attributes displayed

### Conclusion
Basic operations on NumPy arrays were successfully performed.

