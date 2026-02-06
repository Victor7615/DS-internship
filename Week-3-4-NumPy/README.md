# Week 3-4: NumPy for Numerical Computing

## Overview
NumPy is the foundation of numerical computing in Python. These two weeks focus on creating and manipulating arrays, performing mathematical operations, and understanding broadcasting—essential for data science work.

## Learning Objectives
By the end of these weeks, you should be able to:
- [ ] Create and manipulate NumPy arrays
- [ ] Use indexing and slicing effectively
- [ ] Perform element-wise and matrix operations
- [ ] Understand broadcasting
- [ ] Use mathematical functions
- [ ] Work with multi-dimensional arrays
- [ ] Solve linear algebra problems

## Weekly Schedule

### Week 3: NumPy Arrays & Operations

**Monday - Introduction & Array Creation**
- Review NumPy fundamentals
- Study: Creating arrays (array(), zeros(), ones(), arange())
- Study: Array attributes (shape, dtype, size)
- Complete: Creation exercises
- Time: 3 hours

**Tuesday - Indexing & Selection**
- Study: 1D array indexing and slicing
- Study: 2D array indexing
- Study: Boolean indexing and fancy indexing
- Practice: Multiple indexing exercises
- Time: 3 hours

**Wednesday - Array Operations**
- Study: Element-wise operations
- Study: Universal functions (ufuncs)
- Study: Aggregation functions (sum, mean, std, etc.)
- Complete: Operation exercises
- Time: 3 hours

**Thursday - Broadcasting & Shape Manipulation**
- Study: Broadcasting rules
- Study: Reshaping arrays
- Study: Transposing and flattening
- Practice: Broadcasting exercises
- Time: 3 hours

**Friday - Review & Challenge Project**
- Review Week 3 concepts
- Complete challenge exercises
- Start Week 4 preparation
- Time: 2 hours

### Week 4: Advanced NumPy & Linear Algebra

**Monday - Multi-dimensional Arrays**
- Study: 3D and higher dimensional arrays
- Study: Iterating over arrays
- Practice: Working with complex shapes
- Time: 2.5 hours

**Tuesday - Linear Algebra**
- Study: Matrix operations
- Study: Dot product, matrix multiplication
- Study: Solving linear systems
- Practice: Linear algebra problems
- Time: 3 hours

**Wednesday - Random Numbers & Statistics**
- Study: Random number generation
- Study: Statistical functions
- Study: Probability distributions
- Complete: Statistics exercises
- Time: 3 hours

**Thursday - Advanced Functions & Optimization**
- Study: Sorting and searching
- Study: Set operations
- Study: File I/O with NumPy
- Practice exercises
- Time: 3 hours

**Friday - Integration Project & Reflection**
- Complete Week 4 challenges
- Create a data analysis mini-project
- Review all NumPy concepts
- Prepare for Week 5
- Time: 2 hours

## Key Concepts to Master

### Array Creation
```python
import numpy as np

# Different ways to create arrays
arr = np.array([1, 2, 3, 4])
zeros = np.zeros((3, 3))
ones = np.ones((2, 4))
arange = np.arange(0, 10, 2)
linspace = np.linspace(0, 1, 5)
random = np.random.rand(3, 3)
```

### Indexing & Slicing
```python
arr = np.array([10, 20, 30, 40, 50])

# Basic indexing
arr[0]      # 10
arr[-1]     # 50

# Slicing
arr[1:4]    # [20, 30, 40]
arr[::2]    # [10, 30, 50]

# 2D indexing
arr2d = np.array([[1, 2, 3], [4, 5, 6]])
arr2d[0, 1]  # 2
arr2d[1, :]  # [4, 5, 6]
```

### Operations
```python
# Element-wise operations
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])

a + b  # [5, 7, 9]
a * b  # [4, 10, 18]

# Broadcasting
a + 10  # [11, 12, 13]

# Aggregation
np.sum(a)
np.mean(a)
np.std(a)
```

### Broadcasting
```python
# Different shapes can combine
a = np.array([[1, 2, 3], [4, 5, 6]])  # Shape: (2, 3)
b = np.array([10, 20, 30])              # Shape: (3,)

# Broadcasting adds dimension to b
result = a + b  # Shape: (2, 3)
```

## Study Materials

### Primary Resources
1. `02-Python-for-Data-Analysis-NumPy/01-NumPy Arrays.ipynb`
2. `02-Python-for-Data-Analysis-NumPy/02-Numpy Indexing and Selection.ipynb`
3. `02-Python-for-Data-Analysis-NumPy/03-Numpy Operations.ipynb`
4. `02-Python-for-Data-Analysis-NumPy/04-Numpy Exercises.ipynb`
5. `02-Python-for-Data-Analysis-NumPy/05-Numpy Exercises - Solutions.ipynb`

### Learning Path
1. **Lecture Study** (1.5 hours) - Watch and understand concepts
2. **Code Along** (1 hour) - Type every example
3. **Exercises** (1.5 hours) - Complete all exercises
4. **Solutions Review** (30 min) - Learn best practices
5. **Challenge Problems** (1 hour) - Apply knowledge

## Daily Practice Routine

```
Morning (1.5 hours):
- Review previous day's notes
- Recall key formulas and operations

Active Study (2-3 hours):
- Read new concept
- Type code examples
- Complete exercises

Afternoon (1.5 hours):
- Solve challenge problems
- Experiment with edge cases
- Create your own examples

Evening (30 min):
- Summarize learning
- Prepare question list
- Preview next day
```

## Exercises to Complete

### Exercise 1: Array Creation & Properties
- [ ] Create arrays using different methods
- [ ] Understand array shapes and dtypes
- [ ] Convert between array types
- [ ] Understand memory efficiency

### Exercise 2: Indexing & Slicing
- [ ] Index 1D and 2D arrays
- [ ] Use negative indexing
- [ ] Slice with steps
- [ ] Use boolean indexing
- [ ] Practice fancy indexing

### Exercise 3: Array Operations
- [ ] Perform arithmetic operations
- [ ] Use aggregation functions
- [ ] Apply universal functions
- [ ] Compare arrays

### Exercise 4: Broadcasting
- [ ] Understand broadcasting rules
- [ ] Operate on different shapes
- [ ] Reshape for operations
- [ ] Avoid broadcasting errors

### Exercise 5: Linear Algebra
- [ ] Matrix multiplication
- [ ] Transpose operations
- [ ] Determinants and inverses
- [ ] Eigenvalues and eigenvectors

### Exercise 6: Advanced Topics
- [ ] Generate random numbers
- [ ] Calculate statistics
- [ ] Sort and search
- [ ] File I/O operations

## Challenge Projects

### Project 1: Image Filtering
Create image processing:
- Create synthetic image (2D array)
- Apply filters (blur, edge detection)
- Use convolution-like operations
- Visualize results

### Project 2: Matrix Operations Calculator
Build a calculator that:
- Performs matrix operations
- Solves linear systems
- Calculates eigenvalues
- Handles edge cases

### Project 3: Statistical Analysis
Analyze synthetic data:
- Generate random samples
- Calculate statistics
- Create correlation matrices
- Perform basic hypothesis testing

## Common Mistakes to Avoid

1. **View vs. Copy** - Understand when slicing creates views vs. copies
2. **Broadcasting Errors** - Check shape compatibility
3. **Dtype Confusion** - Know your data types
4. **In-place Operations** - Understand += vs. +
5. **Axis Confusion** - Remember axis=0 is rows, axis=1 is columns
6. **Memory Issues** - Large arrays consume significant memory

## Mathematical Concepts Reference

### Matrix Operations
```
A @ B    # Matrix multiplication
A.T      # Transpose
np.linalg.inv(A)     # Inverse
np.linalg.det(A)     # Determinant
np.linalg.eig(A)     # Eigenvalues
```

### Statistics
```
np.mean(arr)         # Average
np.std(arr)          # Standard deviation
np.var(arr)          # Variance
np.percentile(arr, 50)  # Median
np.cov(a, b)         # Covariance
np.corrcoef(a, b)    # Correlation
```

## Visualization Tip
Use Matplotlib to visualize arrays:
```python
import matplotlib.pyplot as plt

arr = np.random.rand(100, 100)
plt.imshow(arr)
plt.colorbar()
plt.show()
```

## Resources

### Documentation
- NumPy Official: https://numpy.org/doc/stable/
- NumPy Tutorial: https://numpy.org/doc/stable/user/basics.html
- Real Python: https://realpython.com/numpy-array-programming/

### Interactive Practice
- Kaggle Notebooks: https://www.kaggle.com/learn/numpy
- DataCamp: https://www.datacamp.com/courses/intro-to-python-for-data-science

## Checklist Before Moving to Week 5

- [ ] Completed all NumPy exercises
- [ ] Reviewed solution notebooks
- [ ] Completed 3 challenge projects
- [ ] Comfortable with indexing and slicing
- [ ] Understand broadcasting
- [ ] Can perform matrix operations
- [ ] Familiar with statistical functions

## Tips for Success

1. **Visualize Arrays** - Draw shapes on paper
2. **Test Shapes** - Use `.shape` attribute frequently
3. **Experiment** - Try different operations
4. **Use Documentation** - NumPy docs are excellent
5. **Build Intuition** - Understand why, not just how
6. **Practice Indexing** - It's crucial for data science
7. **Save Code Snippets** - Create your reference library

## Common Performance Tips

```python
# Vectorize instead of loops
# SLOW: for i in range(len(a)): b[i] = a[i] * 2
# FAST:
b = a * 2

# Use appropriate dtypes
arr = np.array([1, 2, 3], dtype=np.int32)  # Saves memory

# Preallocate arrays
result = np.empty((1000, 1000))
```

## Next Steps

After completing NumPy, you're ready for:
- **Week 5-7**: Pandas for data manipulation
- You'll use NumPy arrays within DataFrames

Excellent progress! You're building a strong foundation! 🎯
