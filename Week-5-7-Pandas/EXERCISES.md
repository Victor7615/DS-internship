# Week 5-7 Pandas - Exercises & Solutions

## Exercise Set 1: Series Basics

### Problems

**1.1 Creating Series**
```python
import pandas as pd
import numpy as np

# TODO: Create Series:
# - s1: From list [10, 20, 30, 40]
# - s2: From dictionary {'a': 10, 'b': 20, 'c': 30}
# - s3: With custom index from range(5)
# - s4: Using range with index

# Print each series
```

**1.2 Series Operations**
```python
s = pd.Series([1, 2, 3, 4, 5], index=['a', 'b', 'c', 'd', 'e'])

# TODO:
# - Access element 'c'
# - Get multiple elements ['a', 'c', 'e']
# - Get elements with s > 3
# - Add 10 to all elements
# - Multiply by 2
# - Apply sqrt function

# Print results
```

---

## Exercise Set 2: DataFrame Creation and Inspection

### Problems

**2.1 Creating DataFrames**
```python
# TODO: Create DataFrames:
# - df1: From dictionary of lists
#   {'Name': ['Alice', 'Bob', 'Charlie'],
#    'Age': [25, 30, 35],
#    'Score': [85, 90, 95]}
# - df2: From nested list with columns
# - df3: Using pd.DataFrame() with index

# Print each
```

**2.2 DataFrame Inspection**
```python
df = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Charlie', 'David'],
    'Age': [25, 30, 35, 28],
    'Score': [85, 90, 88, 92]
})

# TODO: Print:
# - First 2 rows
# - Last 2 rows
# - Random 2 rows
# - Shape
# - Info (dtypes, null counts)
# - Describe (statistics)
# - Column names
# - Data types
```

---

## Exercise Set 3: Indexing and Selection

### Problems

**3.1 Column Selection**
```python
df = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Age': [25, 30, 35],
    'Score': [85, 90, 88],
    'Grade': ['A', 'A', 'B']
})

# TODO:
# - Select 'Name' column (single)
# - Select ['Name', 'Score'] (multiple)
# - Check type of each selection
# - Get unique values from 'Grade'
# - Count values in 'Grade'
```

**3.2 Row Selection**
```python
# TODO:
# - Get first row (iloc[0])
# - Get last row
# - Get rows 1-3 (iloc[1:3])
# - Get row with label 'Charlie' (loc)
# - Get rows where Age > 26
# - Get rows where Grade == 'A'
```

**3.3 Element Selection**
```python
# TODO:
# - Get element at [0, 'Name'] (loc)
# - Get element at [1, 1] (iloc)
# - Set specific element value
# - Get multiple elements with boolean index
```

---

## Exercise Set 4: Data Cleaning

### Problems

**4.1 Missing Data**
```python
df = pd.DataFrame({
    'A': [1, 2, np.nan, 4],
    'B': [5, np.nan, np.nan, 8],
    'C': [9, 10, 11, 12]
})

# TODO:
# - Check for missing values
# - Count missing values per column
# - Drop rows with any missing values
# - Drop rows where specific column is null
# - Fill missing with 0
# - Fill missing with mean
# - Forward fill method
# - Backward fill method
```

**4.2 Duplicates**
```python
df = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Alice', 'Charlie'],
    'Age': [25, 30, 25, 35],
    'Score': [85, 90, 85, 88]
})

# TODO:
# - Check for duplicates
# - Drop duplicates
# - Drop duplicates in specific columns
# - Find duplicate rows
```

**4.3 Data Type Conversion**
```python
df = pd.DataFrame({
    'Name': ['Alice', 'Bob'],
    'Age': ['25', '30'],  # String!
    'Score': [85.5, 90.2]
})

# TODO:
# - Convert Age to integer
# - Convert Score to integer
# - Convert column to datetime
# - Convert to categorical
# - Check new dtypes
```

---

## Exercise Set 5: GroupBy Operations

### Problems

**5.1 Basic GroupBy**
```python
sales = pd.DataFrame({
    'Product': ['A', 'B', 'A', 'B', 'A', 'B'],
    'Region': ['North', 'North', 'South', 'South', 'North', 'South'],
    'Amount': [100, 150, 200, 120, 180, 160]
})

# TODO:
# - Group by Product and sum Amount
# - Group by Region and mean Amount
# - Group by Product and count
# - Group by Region and get max Amount
```

**5.2 Multiple Aggregations**
```python
# TODO:
# - Group by Product:
#   - Sum of Amount
#   - Mean of Amount
#   - Count
# - Using agg() with multiple functions
# - Using agg() with dictionary mapping
```

**5.3 Multiple GroupBy**
```python
# TODO:
# - Group by both Product and Region
# - Aggregate Amount (sum)
# - View as pivot table
# - Get group sizes
```

---

## Exercise Set 6: Merging and Joining

### Problems

**6.1 Merge Operations**
```python
df1 = pd.DataFrame({
    'ID': [1, 2, 3],
    'Name': ['Alice', 'Bob', 'Charlie']
})

df2 = pd.DataFrame({
    'ID': [1, 2, 3],
    'Score': [85, 90, 88]
})

# TODO:
# - Inner join on ID
# - Left join on ID
# - Right join on ID
# - Outer join on ID
# - Merge on both ID columns
```

**6.2 Concat Operations**
```python
df1 = pd.DataFrame({'A': [1, 2], 'B': [3, 4]})
df2 = pd.DataFrame({'A': [5, 6], 'B': [7, 8]})
df3 = pd.DataFrame({'C': [9, 10]})

# TODO:
# - Concatenate df1 and df2 (vertically)
# - Concatenate df1 and df3 (horizontally)
# - Ignore index
# - Use different axis
```

**6.3 Join Operations**
```python
df1 = pd.DataFrame({'A': [1, 2]}, index=['a', 'b'])
df2 = pd.DataFrame({'B': [3, 4]}, index=['a', 'b'])

# TODO:
# - Join df1 and df2
# - Join with how='outer'
# - Join with different indices
```

---

## Exercise Set 7: Advanced Operations

### Problems

**7.1 Pivot Tables**
```python
sales = pd.DataFrame({
    'Product': ['A', 'A', 'B', 'B'],
    'Region': ['North', 'South', 'North', 'South'],
    'Amount': [100, 200, 150, 250]
})

# TODO:
# - Pivot: Product rows, Region columns, Amount values
# - Pivot with aggregation function
# - Pivot with margins=True
# - Stack and unstack operations
```

**7.2 Melt Operations**
```python
df = pd.DataFrame({
    'Name': ['Alice', 'Bob'],
    'Math': [85, 90],
    'Science': [88, 92]
})

# TODO:
# - Melt into long format
# - Specify id_vars and value_vars
# - Rename variables
# - Pivot back to original
```

**7.3 String Operations**
```python
df = pd.DataFrame({
    'Name': ['  Alice  ', 'bob smith', 'CHARLIE']
})

# TODO:
# - Strip whitespace
# - Convert to lowercase
# - Convert to uppercase
# - Check if contains 'a'
# - Replace 'a' with 'A'
# - Split name into first and last
```

---

## Exercise Set 8: Real Data Projects

### Project 1: SF Salaries (Provided Dataset)

```python
# Load: 04-Pandas-Exercises/Salaries.csv

# TODO:
# 1. Load data and explore
# 2. Check shape and info
# 3. Handle missing values
# 4. Identify data types
# 5. Group by JobTitle and calculate:
#    - Mean salary
#    - Median salary
#    - Salary range
# 6. Find highest and lowest paying jobs
# 7. Analyze by Agency
# 8. Create summary statistics
# 9. Visualize findings
```

### Project 2: E-commerce Purchases (Provided Dataset)

```python
# Load: 04-Pandas-Exercises/Ecommerce Purchases

# TODO:
# 1. Load data and explore
# 2. Data quality assessment
# 3. Customer analysis:
#    - Total customers
#    - Purchase frequency
#    - Average purchase value
# 4. Product analysis:
#    - Popular products
#    - Product categories
# 5. Revenue analysis:
#    - Total revenue
#    - Revenue by category
#    - Time-based trends
# 6. Create summary report
```

### Project 3: Custom Data Integration

```python
# TODO:
# 1. Find or create 2-3 datasets
# 2. Load into DataFrames
# 3. Explore each dataset
# 4. Identify join keys
# 5. Clean each dataset
# 6. Merge/join datasets
# 7. Perform integrated analysis
# 8. Create visualizations
# 9. Generate insights report
```

---

## Challenge Exercises

**8.1 Data Cleaning Challenge**
```python
# Create messy dataset with:
# - Missing values
# - Inconsistent formats
# - Duplicate rows
# - Outliers

# TODO: Clean it!
# - Handle missing values appropriately
# - Standardize formats
# - Remove/identify duplicates
# - Flag/remove outliers
# - Document all changes
```

**8.2 GroupBy Challenge**
```python
# Multi-level groupby:
# Group by multiple columns
# Use multiple aggregation functions
# Transform data
# Filter groups
# Create pivot tables

# Real-world scenario:
# Analyze sales by Product, Region, Month
```

**8.3 Merging Challenge**
```python
# Scenario: Customer database with:
# - Customers table
# - Orders table
# - Products table

# TODO:
# - Merge all tables appropriately
# - Handle missing customers
# - Calculate customer metrics
# - Find best customers
# - Create customer report
```

---

## Solutions Hints

### Series
- Index with: `s['label']` or `s[0]`
- Filter with: `s[s > 5]`
- Operations: `.sum()`, `.mean()`, etc.

### DataFrame
- Columns: `df['col']` or `df.col`
- Rows: `df.iloc[0]` or `df.loc['label']`
- Info: `.head()`, `.info()`, `.describe()`

### Cleaning
- Missing: `.isnull()`, `.dropna()`, `.fillna()`
- Duplicates: `.duplicated()`, `.drop_duplicates()`
- Types: `.astype()`

### GroupBy
- Basic: `df.groupby('col').sum()`
- Multiple: `df.groupby(['col1', 'col2'])`
- Custom: `.agg(func)`

### Merge/Join
- `pd.merge(df1, df2, on='key')`
- `pd.concat([df1, df2])`
- `df1.join(df2)`

---

## Review Checklist

- [ ] Completed all exercises
- [ ] Reviewed both project solutions
- [ ] Comfortable with GroupBy
- [ ] Understand merging strategies
- [ ] Can clean real data
- [ ] Completed custom project
- [ ] Ready for Week 8 (Visualization)

Excellent work with Pandas! You're ready to visualize data! 📊
