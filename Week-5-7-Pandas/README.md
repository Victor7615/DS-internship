# Week 5-7: Pandas for Data Manipulation & Cleaning

## Overview
Pandas is the primary tool for data manipulation in data science. These three weeks cover everything from basic DataFrames to advanced data cleaning techniques that you'll use in virtually every data science project.

## Learning Objectives
By the end of these weeks, you should be able to:
- [ ] Create and manipulate Series and DataFrames
- [ ] Load data from various file formats
- [ ] Handle missing data effectively
- [ ] Perform groupby operations
- [ ] Merge and join datasets
- [ ] Transform and reshape data
- [ ] Clean real-world messy data
- [ ] Export processed data

## Weekly Schedule

### Week 5: Pandas Fundamentals

**Monday - Introduction to Pandas**
- Study: Pandas overview and installation
- Study: Series basics
- Study: DataFrames and creation methods
- Practice: Creating data structures
- Time: 3 hours

**Tuesday - Indexing & Selection**
- Study: Accessing columns and rows
- Study: Label-based and position-based indexing
- Study: Conditional selection
- Practice: Complex selection operations
- Time: 3 hours

**Wednesday - Data Input/Output**
- Study: Reading CSV files
- Study: Excel, JSON, SQL data
- Study: Writing to different formats
- Practice: Load and save operations
- Time: 2.5 hours

**Thursday - Basic DataFrame Operations**
- Study: Descriptive statistics
- Study: Data types and conversion
- Study: Sorting and ranking
- Practice: Operations exercises
- Time: 3 hours

**Friday - Review & Integration**
- Review Week 5 concepts
- Complete integration exercises
- Prepare for Week 6
- Time: 2 hours

### Week 6: Data Cleaning & Transformation

**Monday - Missing Data**
- Study: Identifying missing values
- Study: Handling strategies (drop, fill, interpolate)
- Study: Forward fill and backward fill
- Practice: Missing data exercises
- Time: 3 hours

**Tuesday - Data Transformation**
- Study: Apply and map functions
- Study: String operations on columns
- Study: Category and datetime handling
- Practice: Transformation exercises
- Time: 3 hours

**Wednesday - Groupby Operations**
- Study: GroupBy fundamentals
- Study: Aggregation functions
- Study: Multiple grouping levels
- Study: Custom aggregation
- Practice: GroupBy exercises
- Time: 3 hours

**Thursday - Merging & Joining**
- Study: Merge operations
- Study: Concat and append
- Study: Join types (inner, outer, left, right)
- Practice: Complex joins
- Time: 3 hours

**Friday - Data Quality Project**
- Complete data cleaning mini-project
- Work with real messy dataset
- Document cleaning steps
- Time: 2 hours

### Week 7: Advanced Pandas & Capstone

**Monday - Reshaping Data**
- Study: Pivot tables
- Study: Stack and unstack operations
- Study: Melt operations
- Practice: Reshaping exercises
- Time: 3 hours

**Tuesday - Time Series**
- Study: DateTime indexing
- Study: Resampling and rolling operations
- Study: Time-based selection
- Practice: Time series exercises
- Time: 3 hours

**Wednesday - Duplicate & Outlier Handling**
- Study: Finding and removing duplicates
- Study: Detecting outliers
- Study: Data validation techniques
- Practice: Data quality exercises
- Time: 3 hours

**Thursday - Advanced Operations**
- Study: Window functions
- Study: Ranking and percentiles
- Study: Cross-tabulation
- Practice: Advanced exercises
- Time: 3 hours

**Friday - Comprehensive Project & Review**
- Complete comprehensive data analysis project
- Demonstrate all learned skills
- Review and consolidate learning
- Prepare for Week 8
- Time: 2 hours

## Key Concepts to Master

### Series Basics
```python
import pandas as pd

# Create a Series
s = pd.Series([10, 20, 30], index=['a', 'b', 'c'])

# Access elements
s['a']  # 10
s[0]    # 10
s[s > 15]  # [20, 30]
```

### DataFrame Creation
```python
# From dictionary
df = pd.DataFrame({'Name': ['Alice', 'Bob'],
                  'Age': [25, 30]})

# From lists
df = pd.DataFrame([[1, 2], [3, 4]], 
                  columns=['A', 'B'])

# From CSV
df = pd.read_csv('data.csv')
```

### Indexing & Selection
```python
df.head()  # First 5 rows
df['Name']  # Single column
df[['Name', 'Age']]  # Multiple columns
df.loc[0]  # Row by label
df.iloc[0]  # Row by position
df.loc[df['Age'] > 25]  # Conditional selection
```

### Data Cleaning
```python
# Handle missing values
df.isnull()  # Check for nulls
df.dropna()  # Remove nulls
df.fillna(0)  # Fill with value
df.interpolate()  # Interpolate

# Duplicates
df.drop_duplicates()
```

### Groupby Operations
```python
# Group and aggregate
df.groupby('Category').sum()
df.groupby('Category')['Price'].mean()

# Multiple grouping
df.groupby(['Category', 'Year']).sum()

# Custom aggregation
df.groupby('Category').agg({'Price': 'sum',
                            'Quantity': 'mean'})
```

### Merging Data
```python
# Merge (SQL-like join)
merged = pd.merge(df1, df2, on='key')

# Concatenate
combined = pd.concat([df1, df2])

# Join
result = df1.join(df2)
```

## Study Materials

### Primary Resources
1. `03-Python-for-Data-Analysis-Pandas/01-Introduction to Pandas.ipynb`
2. `03-Python-for-Data-Analysis-Pandas/02-Series.ipynb`
3. `03-Python-for-Data-Analysis-Pandas/03-DataFrames.ipynb`
4. `03-Python-for-Data-Analysis-Pandas/04-Missing Data.ipynb`
5. `03-Python-for-Data-Analysis-Pandas/05-Groupby.ipynb`
6. `03-Python-for-Data-Analysis-Pandas/06-Merging, Joining, and Concatenating.ipynb`
7. `03-Python-for-Data-Analysis-Pandas/07-Operations.ipynb`
8. `03-Python-for-Data-Analysis-Pandas/08-Data Input and Output.ipynb`

### Practice Exercises
- `04-Pandas-Exercises/01-SF Salaries Exercise.ipynb`
- `04-Pandas-Exercises/02-SF Salaries Exercise - Solutions.ipynb`
- `04-Pandas-Exercises/03-Ecommerce Purchases Exercise.ipynb`
- `04-Pandas-Exercises/04-Ecommerce Purchases Exercise - Solutions.ipynb`

## Daily Practice Routine

```
Morning (1.5 hours):
- Review yesterday's concepts
- Skim solution notebooks

Active Study (2.5 hours):
- Read new material
- Type all examples
- Complete exercises

Afternoon (1.5-2 hours):
- Solve additional problems
- Work on projects
- Experiment with variations

Evening (30 min):
- Summarize key concepts
- Create reference sheet
- Plan next day
```

## Exercises to Complete

### Exercise 1: Series Operations
- [ ] Create Series from lists and dictionaries
- [ ] Perform arithmetic on Series
- [ ] Use conditional indexing
- [ ] Apply functions to Series

### Exercise 2: DataFrame Creation & Inspection
- [ ] Create DataFrames from various sources
- [ ] Inspect shape, dtypes, info
- [ ] Display head, tail, sample
- [ ] Get basic statistics

### Exercise 3: Indexing & Selection
- [ ] Select columns (single and multiple)
- [ ] Select rows by position and label
- [ ] Use boolean indexing
- [ ] Use .loc and .iloc effectively

### Exercise 4: Data Cleaning
- [ ] Identify and handle missing values
- [ ] Remove and handle duplicates
- [ ] Convert data types
- [ ] Validate data quality

### Exercise 5: GroupBy & Aggregation
- [ ] Group by single columns
- [ ] Group by multiple columns
- [ ] Apply multiple aggregation functions
- [ ] Create pivot tables

### Exercise 6: Merging & Reshaping
- [ ] Perform different types of joins
- [ ] Concatenate datasets
- [ ] Stack and unstack data
- [ ] Pivot and melt operations

## Challenge Projects

### Project 1: SF Salaries Analysis (Provided)
Use included SF Salaries dataset:
- [ ] Load and explore data
- [ ] Clean data (handle missing, outliers)
- [ ] Calculate salary statistics
- [ ] GroupBy department analysis
- [ ] Identify trends and patterns

### Project 2: E-commerce Purchases Analysis (Provided)
Use included Ecommerce Purchases dataset:
- [ ] Load and inspect data
- [ ] Clean customer information
- [ ] Analyze purchase patterns
- [ ] Calculate customer metrics
- [ ] Segment customers

### Project 3: Personal Data Integration Project
Create your own analysis:
- [ ] Find or create multiple datasets
- [ ] Merge datasets on key
- [ ] Perform comprehensive cleaning
- [ ] Create derived features
- [ ] Generate summary reports

## Common Mistakes to Avoid

1. **Chained Indexing** - Use .loc[] instead of chained brackets
2. **Copy vs. View** - Use .copy() to avoid warnings
3. **Inplace Confusion** - Understand inplace=True behavior
4. **Axis Confusion** - axis=0 is rows, axis=1 is columns
5. **Dtype Issues** - Check dtypes, convert when needed
6. **Missing Value Handling** - Different strategies for different scenarios
7. **Index Alignment** - Be careful with alignment in operations

## Best Practices for Data Cleaning

```python
# GOOD: Systematic cleaning
df = pd.read_csv('data.csv')
print(f"Initial shape: {df.shape}")
print(df.isnull().sum())
df = df.dropna(subset=['essential_column'])
df = df.drop_duplicates()
print(f"Final shape: {df.shape}")
```

## Resources

### Documentation
- Pandas Official: https://pandas.pydata.org/docs/
- Pandas User Guide: https://pandas.pydata.org/docs/user_guide/index.html
- Real Python Pandas: https://realpython.com/learning-paths/pandas-data-science/

### Datasets
- Kaggle Datasets: https://www.kaggle.com/datasets
- UCI ML Repository: https://archive.ics.uci.edu/ml/
- Google Dataset Search: https://datasetsearch.research.google.com/

### Interactive Learning
- DataCamp Pandas: https://www.datacamp.com/courses/data-manipulation-with-pandas
- Mode Analytics SQL: https://mode.com/sql-tutorial/

## Checklist Before Moving to Week 8

- [ ] Completed all Pandas exercises
- [ ] Reviewed solution notebooks thoroughly
- [ ] Completed both provided real-world projects
- [ ] Comfortable with DataFrame operations
- [ ] Confident in data cleaning techniques
- [ ] Understand merging and joining
- [ ] Can handle missing data appropriately
- [ ] Experienced with GroupBy operations

## Tips for Success

1. **Understand Data First** - Always use .head(), .info(), .describe()
2. **Check Assumptions** - Verify your data matches your assumptions
3. **Document Changes** - Keep track of cleaning steps
4. **Validate Results** - Check outputs make sense
5. **Use Chaining** - Chain operations for readability
6. **Read Carefully** - Pay attention to axis parameter
7. **Ask Questions** - When confused, check documentation

## Data Cleaning Checklist

Before moving data to analysis, ensure:
- [ ] No unreasonable null values
- [ ] Appropriate data types
- [ ] No obvious duplicates
- [ ] Outliers handled or documented
- [ ] Column names clear and consistent
- [ ] Index makes sense
- [ ] Data validated against source

## Next Steps

After Pandas, you're ready for:
- **Week 8-9**: Data Visualization (Matplotlib, Seaborn, Plotly)
- You'll use Pandas DataFrames to create visualizations

Congratulations on progressing through data manipulation! You're now equipped for real data work! 🎉
