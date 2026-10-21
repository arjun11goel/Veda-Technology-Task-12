# NumPy Array Operations - Task-12

## Description
This project demonstrates fundamental vectorized numerical operations using the NumPy library in Python. It involves creating two one-dimensional arrays and performing element-wise addition, subtraction, multiplication, and division to highlight the efficiency and concise syntax of NumPy compared to standard Python lists.

## Objective
To understand and implement vectorized numerical operations using NumPy arrays.

## Prerequisites
To run this project, you need the following installed:
* Python 3.x
* Jupyter Notebook (or any Python IDE)
* NumPy library

You can install the required NumPy library using pip:
```bash
pip install numpy
```

## Usage
1. Open a Jupyter Notebook or a standard Python script file.
2. Copy and paste the core Python code into a cell/file.
3. Execute the code to see the vectorized operations in action.

## Code Overview
The code initializes two arrays using `np.array()` and performs arithmetic directly on the array variables:
```python
import numpy as np

array1 = np.array([10, 20, 30, 40, 50])
array2 = np.array([2, 4, 5, 8, 10])

# Vectorized operations
addition = array1 + array2
subtraction = array1 - array2
multiplication = array1 * array2
division = array1 / array2
```

## Expected Output
When you run the code, it will print the original arrays, their shapes, and the results of the operations:

```text
Array 1: [10 20 30 40 50]
Array 2: [ 2  4  5  8 10]
Shape of Array 1: (5,)
Shape of Array 2: (5,)
------------------------------
Addition (Array 1 + Array 2): [12 24 35 48 60]
Subtraction (Array 1 - Array 2): [ 8 16 25 32 40]
Multiplication (Array 1 * Array 2): [ 20  80 150 320 500]
Division (Array 1 / Array 2): [5. 5. 6. 5. 5.]
```

## Concepts Covered
* **Array Creation:** Using `np.array()` to initialize numerical data structures.
* **Shape Inspection:** Using the `.shape` attribute to verify array dimensions before operating on them.
* **Vectorization:** Executing batch operations on entire arrays at once without writing explicit `for` loops. This leverages NumPy's optimized, pre-compiled C backend for significantly faster element-wise arithmetic.

## Interview Q&A Reference
* **What is vectorization?** Processing entire arrays simultaneously rather than elements sequentially using loops.
* **What happens when two NumPy arrays are added?** NumPy performs element-wise addition (matching indices are added together).
* **Why is NumPy faster?** It uses contiguous memory blocks, pre-compiled C code, and avoids Python loop overhead through vectorization.
