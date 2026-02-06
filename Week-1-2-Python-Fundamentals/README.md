# Week 1-2: Python Fundamentals & Environment Setup

## Overview
These first two weeks establish your foundation in Python programming and set up your development environment. You'll learn essential programming concepts that will support all future data science work.

## Learning Objectives
By the end of these weeks, you should be able to:
- [ ] Set up Python and Jupyter notebooks
- [ ] Understand variables, data types, and operators
- [ ] Write and use functions effectively
- [ ] Use control flow (if statements, loops)
- [ ] Work with data structures (lists, dictionaries, tuples)
- [ ] Understand object-oriented programming basics
- [ ] Write clean, documented code

## Weekly Schedule

### Week 1: Python Basics & Setup

**Monday - Setup & Introduction**
- Install Python 3.8+ and Anaconda
- Install VS Code or PyCharm
- Launch first Jupyter notebook
- Read: `01-Python-Crash-Course/01-Python Crash Course.ipynb`
- Time: 2-3 hours

**Tuesday - Variables & Data Types**
- Study: Variables, integers, floats, strings, booleans
- Complete exercises in provided notebook
- Practice: Create variables of different types
- Time: 3 hours

**Wednesday - Operators & String Operations**
- Study: Arithmetic, comparison, logical operators
- Study: String methods and formatting
- Complete: All exercises in notebook
- Practice challenge: String manipulation problems
- Time: 3 hours

**Thursday - Lists & Data Structures**
- Study: Lists, tuples, dictionaries, sets
- Practice: Indexing and slicing
- Complete exercises and practice problems
- Time: 3 hours

**Friday - Review & Reflection**
- Review all Week 1 content
- Complete the Week 1 challenge exercises
- Create a summary document
- Time: 2 hours

### Week 2: Control Flow, Functions & OOP

**Monday - Conditionals & Loops**
- Study: if/elif/else statements
- Study: for and while loops
- Practice loop exercises and nested loops
- Time: 3 hours

**Tuesday - Functions**
- Study: Defining functions, parameters, return values
- Study: Default arguments, *args, **kwargs
- Complete function exercises
- Practice: Create reusable functions
- Time: 3 hours

**Wednesday - Advanced Functions**
- Study: Lambda functions, map, filter
- Study: List comprehensions and generators
- Complete exercises
- Time: 3 hours

**Thursday - Object-Oriented Programming**
- Study: Classes, objects, methods, attributes
- Study: Inheritance and polymorphism
- Complete OOP exercises
- Practice: Create simple classes
- Time: 3 hours

**Friday - Integration Project & Review**
- Complete the integrated exercises
- Review solutions
- Prepare for Week 3
- Time: 2-3 hours

## Key Concepts to Master

### Variables & Data Types
```python
# Variables store data
name = "Data Scientist"  # String
age = 25                 # Integer
gpa = 3.8               # Float
is_student = True       # Boolean

# Check types
type(name)  # <class 'str'>
```

### Control Flow
```python
# If statements
if age > 18:
    print("Adult")
elif age > 13:
    print("Teen")
else:
    print("Child")

# Loops
for i in range(5):
    print(i)

while age < 30:
    age += 1
```

### Functions
```python
def greet(name, greeting="Hello"):
    return f"{greeting}, {name}!"

result = greet("Alice")
```

### Data Structures
```python
# List (ordered, mutable)
numbers = [1, 2, 3, 4, 5]

# Dictionary (key-value pairs)
person = {"name": "John", "age": 30}

# Tuple (ordered, immutable)
coordinates = (10, 20)

# Set (unique values)
unique_numbers = {1, 2, 3}
```

## Study Materials

### Primary Resources
1. `01-Python-Crash-Course/01-Python Crash Course.ipynb` - Main lecture
2. `01-Python-Crash-Course/02-Python Crash Course Exercises.ipynb` - Exercises
3. `01-Python-Crash-Course/03-Python Crash Course Exercises - Solutions.ipynb` - Solutions

### Learning Approach
1. **Read & Understand** (30 min) - Go through notebook cells
2. **Code Along** (1 hour) - Type every code example
3. **Solve Exercises** (1.5 hours) - Complete all exercises
4. **Review Solutions** (30 min) - Compare with solution notebook
5. **Extra Practice** (1 hour) - Solve challenge problems

## Daily Practice Routine

```
Morning (1 hour):
- Review yesterday's notes
- Re-read one difficult concept

Active Study (2-3 hours):
- Read new material
- Type code examples
- Complete exercises

Afternoon (1-2 hours):
- Solve challenge problems
- Experiment with variations
- Write your own examples

Evening (30 min):
- Review and summarize learning
- Note down questions
- Plan next day
```

## Exercises to Complete

### Exercise 1: Variables & Types
- [ ] Create variables of each data type
- [ ] Convert between types
- [ ] Understand type errors

### Exercise 2: String Operations
- [ ] Slice strings
- [ ] Use string methods (upper, lower, replace)
- [ ] Format strings using f-strings
- [ ] Work with string operations

### Exercise 3: Data Structures
- [ ] Create and manipulate lists
- [ ] Access dictionary values
- [ ] Understand list vs. tuple differences
- [ ] Use set operations

### Exercise 4: Control Flow
- [ ] Write if/elif/else logic
- [ ] Use for loops with range()
- [ ] Create nested loops
- [ ] Use while loops safely

### Exercise 5: Functions
- [ ] Define and call functions
- [ ] Use parameters and return values
- [ ] Use default arguments
- [ ] Create list comprehensions

### Exercise 6: OOP Basics
- [ ] Create a simple class
- [ ] Add methods and attributes
- [ ] Use inheritance
- [ ] Understand self parameter

## Challenge Projects

### Project 1: Number Guessing Game
Create a game where:
- Computer picks random number
- User tries to guess
- Give hints (too high/low)
- Count attempts
- Play multiple rounds

### Project 2: Personal Data Management
Create a program that:
- Stores person information in a dictionary
- Has functions to add, update, delete info
- Displays formatted information
- Uses object-oriented design

### Project 3: Text Analysis Tool
Create a tool that:
- Takes a text input
- Counts words and characters
- Finds most common words
- Calculates reading time
- Uses functions and data structures

## Common Mistakes to Avoid

1. **Off-by-one errors** - Remember indexing starts at 0
2. **Mutable default arguments** - Don't use `[]` as default
3. **Infinite loops** - Always ensure loop termination
4. **Variable scope** - Understand local vs. global variables
5. **Type errors** - Remember types matter in Python
6. **Indentation** - Python cares deeply about indentation

## Resources

### Documentation
- Python Official: https://docs.python.org/3/tutorial/
- Real Python Tutorials: https://realpython.com/
- W3Schools Python: https://www.w3schools.com/python/

### Interactive Practice
- LeetCode: https://leetcode.com/
- CodeWars: https://www.codewars.com/
- HackerRank: https://www.hackerrank.com/

## Checklist Before Moving to Week 3

- [ ] Completed all exercises in both weeks
- [ ] Reviewed all solution notebooks
- [ ] Completed all 3 challenge projects
- [ ] Feel comfortable with Python basics
- [ ] Can write functions confidently
- [ ] Understand when to use different data structures
- [ ] Can create simple classes

## Tips for Success

1. **Type Everything** - Don't copy-paste; type code
2. **Experiment** - Modify examples to understand them
3. **Break Code** - Intentionally create errors to learn
4. **Read Error Messages** - They tell you what's wrong
5. **Write Comments** - Explain your code to yourself
6. **Ask Questions** - Use notebooks to test ideas
7. **Sleep** - Neural connections form during rest

## Next Steps

Once you complete this week, you're ready for:
- **Week 3-4**: NumPy for numerical computing
- You'll build on these Python fundamentals to analyze data

## Questions? Getting Stuck?

**For debugging:**
1. Read error messages carefully
2. Check variable values with `print()`
3. Use interactive Python to test code
4. Consult documentation
5. Search error message + "Python"

Good luck! Python mastery is within reach! 🚀
