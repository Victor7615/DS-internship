# Week 3-4 NumPy - Exercises & Solutions

## Exercise Set 1: Array Creation

### Problems

**1.1 Creating Arrays**
```python
import numpy as np

# TODO: Create the following arrays:
# - arr1: 1D array with values [1, 2, 3, 4, 5]
# - arr2: 2D array of zeros with shape (3, 4)
# - arr3: 2D array of ones with shape (2, 5)
# - arr4: Array with values 0 to 9 using arange()
# - arr5: Array with 5 evenly spaced values from 0 to 1

# Print shape and dtype for each
```

**1.2 Random Arrays**
```python
# TODO: Create:
# - rand_arr: Random 3x3 array with values 0-1
# - rand_int: Random 2x4 array with integers 1-10
# - rand_normal: 1D array of 100 values from normal distribution
# - rand_choice: Array of 10 random choices from [1, 2, 3, 4, 5]

# Print first few elements of each
```

**1.3 Array Properties**
```python
arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])

# TODO: Print:
# - Shape
# - Size (total elements)
# - Dtype
# - Number of dimensions
# - Memory size in bytes
```

---

## Exercise Set 2: Indexing and Slicing

### Problems

**2.1 1D Array Indexing**
```python
arr = np.array([10, 20, 30, 40, 50, 60, 70, 80, 90])

# TODO:
# - Get element at index 3
# - Get last element
# - Get element at index -2 (second from last)
# - Get elements from index 2 to 5 (exclusive of 5)
# - Get elements from index 0 to end, step 2
```

**2.2 2D Array Indexing**
```python
arr = np.array([[1, 2, 3], 
                [4, 5, 6], 
                [7, 8, 9]])

# TODO:
# - Get element at [1, 2]
# - Get entire first row
# - Get entire second column
# - Get 2x2 subarray from top-left
# - Get last row
# - Get last element
```

**2.3 Boolean Indexing**
```python
arr = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])

# TODO:
# - Get all elements greater than 5
# - Get all even elements
# - Get all elements divisible by 3
# - Get elements in range [3, 7]
# - Replace all elements > 5 with 0
```

**2.4 Fancy Indexing**
```python
arr = np.array([10, 20, 30, 40, 50, 60, 70])

# TODO:
# - Get elements at indices [0, 2, 4]
# - Get elements at indices [1, 3, 5]
# - Reorder: get elements at [6, 4, 2, 0]
# - Create boolean index for values > 30 and use it
```

---

## Exercise Set 3: Array Operations

### Problems

**3.1 Element-wise Operations**
```python
a = np.array([1, 2, 3, 4])
b = np.array([5, 6, 7, 8])

# TODO:
# - Add arrays
# - Subtract a from b
# - Multiply arrays (element-wise)
# - Divide b by a
# - Get remainder of b / a
# - Raise a to power 2

# Print all results
```

**3.2 Universal Functions**
```python
arr = np.array([1, 4, 9, 16, 25])

# TODO:
# - Square root
# - Exponential (e^x)
# - Natural logarithm
# - Sine values
# - Absolute value of [-1, -2, -3]

# Print all results
```

**3.3 Aggregation Functions**
```python
arr = np.array([10, 25, 15, 30, 20])

# TODO: Calculate:
# - Sum
# - Mean
# - Standard deviation
# - Variance
# - Min and max
# - Argmin and argmax (indices)

# Print all results
```

**3.4 Operations Along Axes**
```python
arr = np.array([[1, 2, 3],
                [4, 5, 6],
                [7, 8, 9]])

# TODO:
# - Sum along rows (axis=1)
# - Sum along columns (axis=0)
# - Mean along axis 0
# - Max along axis 1
# - Cumulative sum
```

---

## Exercise Set 4: Broadcasting

### Problems

**4.1 Basic Broadcasting**
```python
a = np.array([[1, 2, 3], 
              [4, 5, 6]])  # Shape: (2, 3)
b = np.array([10, 20, 30])  # Shape: (3,)

# TODO:
# - Add a + b (broadcasting b to each row)
# - Multiply a * 10
# - Divide a by [1, 2, 3]
# - Subtract [100] from a

# Explain why broadcasting works for each
```

**4.2 Broadcasting with Scalars**
```python
arr = np.array([[1, 2, 3],
                [4, 5, 6]])

# TODO:
# - Add 10 to all elements
# - Multiply all by 2
# - Compare to scalar (arr > 3)
# - Raise all to power 2
```

**4.3 Understanding Shapes**
```python
# For each pair, predict if broadcasting will work:
# (3, 1) and (3, 3) - YES/NO?
# (2, 3) and (3,) - YES/NO?
# (4, 1) and (1, 4) - YES/NO?
# (5,) and (1,) - YES/NO?

# TODO: Test your predictions with code
```

---

## Exercise Set 5: Reshaping and Transformation

### Problems

**5.1 Reshaping Arrays**
```python
arr = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])

# TODO:
# - Reshape to (3, 4)
# - Reshape to (4, 3)
# - Reshape to (2, 2, 3)
# - Flatten back to 1D
# - Transpose
```

**5.2 Stack Operations**
```python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])

# TODO:
# - Stack horizontally (hstack)
# - Stack vertically (vstack)
# - Use stack() along axis 0
# - Concatenate along axis 1
```

**5.3 Split Operations**
```python
arr = np.array([1, 2, 3, 4, 5, 6])

# TODO:
# - Split into 2 equal arrays
# - Split into 3 equal arrays
# - Split at specific positions [2, 4]
# - Verify by concatenating back
```

---

## Exercise Set 6: Linear Algebra

### Problems

**6.1 Matrix Operations**
```python
A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])

# TODO:
# - Matrix multiplication (A @ B)
# - Transpose of A
# - Determinant of A
# - Inverse of A
# - Trace of A (sum of diagonal)

# Verify A @ A^-1 ≈ Identity matrix
```

**6.2 Eigenvalues**
```python
A = np.array([[4, -2], [-1, 3]])

# TODO:
# - Calculate eigenvalues and eigenvectors
# - Print eigenvalues
# - Print eigenvectors
# - Verify: A @ v = λ @ v

# For a 2x2 matrix
```

**6.3 Linear System**
```python
# Solve: 2x + y = 5
#        x + 3y = 7

# TODO:
# - Set up as Ax = b
# - Use np.linalg.solve()
# - Verify solution

# Also solve another system of your choice
```

---

## Exercise Set 7: Random Numbers and Statistics

### Problems

**7.1 Probability Distributions**
```python
# TODO: Generate samples from:
# - Uniform distribution [0, 1): 1000 samples
# - Normal distribution (mean=0, std=1): 1000 samples
# - Exponential distribution (λ=1): 1000 samples

# For each, calculate mean and std
# Compare to theoretical values
```

**7.2 Statistical Analysis**
```python
data = np.random.randn(100)  # 100 random normal values

# TODO: Calculate:
# - Percentiles: 25th, 50th, 75th
# - Interquartile range
# - Coefficient of variation (std/mean)
# - Skewness and kurtosis (if available)
```

**7.3 Correlation and Covariance**
```python
x = np.array([1, 2, 3, 4, 5])
y = np.array([2, 4, 5, 4, 6])

# TODO:
# - Calculate covariance
# - Calculate correlation coefficient
# - Interpret the results
```

---

## Challenge Projects

### Project 1: Image Filtering

**Objective:** Create and filter a synthetic image

**Requirements:**
```python
# TODO:
# 1. Create a 100x100 random image array
# 2. Create filters:
#    - Blur filter (3x3 averaging kernel)
#    - Edge detection (Sobel-like)
# 3. Apply filters using convolution-like operations
# 4. Visualize original and filtered images
# 5. Calculate statistics before/after filtering

import matplotlib.pyplot as plt
```

### Project 2: Matrix Calculator

**Objective:** Create interactive matrix operations tool

**Requirements:**
```python
# TODO: Create functions for:
# 1. Matrix creation from user input
# 2. Basic operations (add, subtract, multiply)
# 3. Advanced operations (transpose, inverse)
# 4. Linear system solving
# 5. Eigenvalue decomposition
# 6. Menu-driven interface

# Test with various matrix sizes
```

### Project 3: Statistical Analysis

**Objective:** Analyze multiple distributions

**Requirements:**
```python
# TODO:
# 1. Generate samples from 5 different distributions
# 2. Calculate statistics for each:
#    - Mean, median, mode
#    - Std, variance, range
#    - Skewness, kurtosis
# 3. Create comparison table
# 4. Visualize all distributions
# 5. Analyze relationships between distributions
```

---

## Solution Hints

### Array Creation
- Use `np.zeros()`, `np.ones()`, `np.arange()`
- Use `np.random.rand()` for uniform, `np.random.randn()` for normal
- Check shape with `.shape`

### Indexing
- 1D: `arr[index]`
- 2D: `arr[row, col]`
- Slicing: `arr[start:end:step]`
- Boolean: `arr[arr > 5]`

### Operations
- Element-wise: `arr1 + arr2`
- Functions: `np.sqrt()`, `np.exp()`, `np.log()`
- Aggregation: `.sum()`, `.mean()`, `.std()`
- Specify axis: `arr.sum(axis=0)`

### Broadcasting
- Smaller arrays expand to match larger ones
- Missing dimensions are added on the left
- Size 1 can broadcast to any size

### Linear Algebra
- Matrix mult: `A @ B` or `np.dot(A, B)`
- Transpose: `A.T`
- Inverse: `np.linalg.inv(A)`
- Solve: `np.linalg.solve(A, b)`

---

## Review Checklist

- [ ] All exercises completed
- [ ] Understand broadcasting thoroughly
- [ ] Comfortable with indexing in multiple dimensions
- [ ] Can perform matrix operations
- [ ] Completed at least 2 challenge projects
- [ ] Ready for Week 5 (Pandas)

---

## Common NumPy Pitfalls

1. **View vs. Copy** - Slicing creates view, not copy
2. **2D vs. 1D** - Shape (3,) ≠ (3, 1)
3. **In-place vs. New** - `arr += 1` modifies, `arr + 1` doesn't
4. **Integer Division** - Use float for true division
5. **Empty Tuples** - `arr[()]` returns original array

Good luck with NumPy! You're building essential skills! 💪
