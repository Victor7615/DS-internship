# Week 1-2 Python Fundamentals - Exercises & Solutions

## Exercise Set 1: Variables and Data Types

### Problems

**1.1 Basic Variables**
```python
# Create variables for a person's profile
# TODO: Create the following variables:
# - name (string): "Alex"
# - age (integer): 25
# - gpa (float): 3.85
# - is_freshman (boolean): True

# Verify types using type()
```

**1.2 Type Conversion**
```python
# Given string "100", convert to different types
num_string = "100"

# TODO: 
# - Convert to integer and assign to num_int
# - Convert to float and assign to num_float
# - Convert to string (should stay same) and verify

# Print all three results
```

**1.3 Multiple Assignment**
```python
# TODO: Use multiple assignment to create:
# a = 1, b = 2, c = 3 in one line
# Then swap a and c in one line (without using temp variable)
# Print: a, b, c
```

---

## Exercise Set 2: String Operations

### Problems

**2.1 String Methods**
```python
text = "Data Science is Awesome"

# TODO: Using string methods, perform these operations:
# - Convert to lowercase
# - Convert to uppercase
# - Replace "Awesome" with "Amazing"
# - Count occurrences of 'a'
# - Check if "Science" is in the string

# Print each result
```

**2.2 String Indexing and Slicing**
```python
word = "Python"

# TODO: 
# - Get first character
# - Get last character
# - Get first 3 characters
# - Get last 3 characters
# - Reverse the word using slicing
# - Get every other character

# Print each result
```

**2.3 String Formatting**
```python
name = "Alice"
score = 95.5
subject = "Data Science"

# TODO: Using f-strings, create this output:
# "Alice scored 95.5 in Data Science"
# Also: "Alice scored 95% in Data Science" (round to integer)

# Print the formatted strings
```

---

## Exercise Set 3: Data Structures

### Problems

**3.1 List Operations**
```python
numbers = [10, 20, 30, 40, 50]

# TODO:
# - Access the first element
# - Access the last element
# - Get elements from index 1 to 3 (exclusive of 3)
# - Add 60 to the list
# - Remove 30 from the list
# - Get the length of list
# - Find the maximum value

# Print all results
```

**3.2 List Comprehension**
```python
# TODO: Using list comprehension, create:
# - squares: list of squares of numbers 1 to 10
# - evens: list of even numbers from 1 to 20
# - upper_letters: list of uppercase letters from ["a", "b", "c"]

# Print all lists
```

**3.3 Dictionary Operations**
```python
student = {"name": "John", "age": 20, "major": "CS"}

# TODO:
# - Access the value for "name"
# - Add a new key "gpa" with value 3.8
# - Update "age" to 21
# - Get all keys
# - Get all values
# - Check if "age" is a key

# Print all results
```

**3.4 Dictionary Comprehension**
```python
# TODO: Create a dictionary where:
# - Keys are numbers 1-5
# - Values are squares of those numbers
# (Result: {1: 1, 2: 4, 3: 9, 4: 16, 5: 25})

# Print the dictionary
```

---

## Exercise Set 4: Control Flow

### Problems

**4.1 If/Elif/Else**
```python
score = 85

# TODO: Create grade assignment logic:
# 90-100: A
# 80-89: B
# 70-79: C
# 60-69: D
# Below 60: F

# Print the grade for the given score
```

**4.2 For Loop with Range**
```python
# TODO: Print multiplication table for 5 (5x1 through 5x10)
# Using a for loop with range()

# Expected output:
# 5 x 1 = 5
# 5 x 2 = 10
# ... and so on
```

**4.3 For Loop with Lists**
```python
fruits = ["apple", "banana", "cherry", "date"]

# TODO:
# - Loop through and print each fruit
# - Loop through with index using enumerate()
# - Find and print the index of "cherry"
```

**4.4 While Loop**
```python
# TODO: Create a program that:
# - Starts with count = 1
# - Loops while count <= 10
# - Prints count * count (square)
# - Increments count

# Print squares of 1 to 10
```

**4.5 Nested Loops**
```python
# TODO: Create a 3x3 grid pattern using nested loops
# Expected output:
# * * *
# * * *
# * * *
```

---

## Exercise Set 5: Functions

### Problems

**5.1 Basic Function**
```python
# TODO: Create a function that:
# - Takes a name as parameter
# - Returns "Hello, [name]!"

# Call the function with "Alice"
```

**5.2 Function with Multiple Parameters**
```python
# TODO: Create a function that:
# - Takes two numbers as parameters
# - Returns their sum, difference, product
# - (Hint: return as tuple)

# Call with 10 and 5
# Unpack and print results
```

**5.3 Function with Default Arguments**
```python
# TODO: Create a function:
# - calculate_total(price, tax_rate=0.1)
# - Returns price + (price * tax_rate)

# Call with just price: 100
# Call with price and custom tax_rate: 100, 0.15
```

**5.4 List Comprehension with Function**
```python
# TODO: Using the previous sum function
# Create a list of sums of consecutive pairs:
# Given: [1, 2, 3, 4, 5]
# Result: [3, 5, 7, 9] (1+2, 2+3, 3+4, 4+5)

# Use list comprehension or loop
```

**5.5 Lambda Functions**
```python
# TODO: Create and use lambda functions for:
# - Double a number
# - Add two numbers
# - Check if number is even

# Test each with examples
```

**5.6 List Comprehension Review**
```python
# TODO: Create:
# - squared: [x**2 for x in range(1, 6)]
# - evens: [x for x in range(20) if x % 2 == 0]
# - pairs: [(x, x**2) for x in range(1, 6)]

# Print all
```

---

## Exercise Set 6: Object-Oriented Programming

### Problems

**6.1 Basic Class**
```python
# TODO: Create a Student class with:
# - __init__ method with name and age
# - greet() method that returns "Hello, I'm [name]"
# - birthday() method that increments age

# Create instance, test methods
```

**6.2 Class with Properties**
```python
# TODO: Create a BankAccount class with:
# - __init__ with account_holder (string) and balance (float)
# - deposit(amount) method
# - withdraw(amount) method (check balance)
# - get_balance() method

# Test with multiple operations
```

**6.3 Inheritance**
```python
# TODO: Create:
# - Animal class with name and sound attributes
# - Dog class that inherits from Animal
# - Cat class that inherits from Animal
# - Override speak() method in each

# Create instances and test
```

**6.4 String Representation**
```python
# TODO: Modify a Person class to:
# - Use __init__ with name and age
# - Implement __str__ to return "Person: name (age)"
# - Implement __repr__ for debugging

# Create and print instances
```

---

## Challenge Projects

### Project 1: Number Guessing Game

**Objective:** Create an interactive number guessing game

**Requirements:**
```python
# TODO: Create a game that:
# 1. Computer picks a random number 1-100
# 2. User has 7 attempts
# 3. After each guess:
#    - Tell if guess is too high/too low
#    - Show remaining attempts
# 4. Win: Print "Congratulations!"
# 5. Lose: Print the correct number
# 6. Ask to play again

# BONUS: Keep score across multiple rounds
```

### Project 2: Text Analysis Tool

**Objective:** Analyze text statistics

**Requirements:**
```python
# TODO: Create program that:
# 1. Takes user text input
# 2. Calculates:
#    - Total characters (with/without spaces)
#    - Total words
#    - Total sentences
#    - Average word length
# 3. Finds:
#    - Longest word
#    - Most common word
# 4. Estimates:
#    - Reading time (assuming 200 wpm)

# Use functions for each calculation
```

### Project 3: Simple Quiz Game

**Objective:** Create an interactive quiz

**Requirements:**
```python
# TODO: Create class-based quiz system:
# 1. Question class with question, options, correct_answer
# 2. Quiz class that:
#    - Stores multiple questions
#    - Presents questions to user
#    - Tracks correct answers
#    - Shows final score
# 3. Create 5 questions about Python
# 4. Run quiz and display results

# BONUS: Add difficulty levels
```

---

## Solution Hints

### Hint 1: Variables and Types
- Use `type()` function to check types
- `int()`, `float()`, `str()`, `bool()` for conversion
- Multiple assignment: `a, b, c = 1, 2, 3`

### Hint 2: Strings
- `.lower()`, `.upper()`, `.replace()`, `.count()`
- `text[start:end:step]` for slicing
- f-strings: `f"Hello {name}"`

### Hint 3: Data Structures
- Lists are mutable; tuples are immutable
- Dictionary access: `dict[key]`
- List methods: `.append()`, `.remove()`, `.extend()`

### Hint 4: Control Flow
- `if`, `elif`, `else` for conditions
- `for` loop for sequences
- `while` loop for conditions
- `break` and `continue` keywords

### Hint 5: Functions
- Define with `def` keyword
- `return` for output
- Parameters have default values
- Lambda: `lambda x: x * 2`

### Hint 6: OOP
- `self` refers to instance
- `__init__` is constructor
- Inheritance uses `class Child(Parent):`
- `super()` calls parent methods

---

## Review Checklist

- [ ] All exercises completed
- [ ] All solutions work correctly
- [ ] Understand each concept deeply
- [ ] Can explain to someone else
- [ ] Completed at least 2 challenge projects
- [ ] Code is well-commented
- [ ] Ready for Week 3

---

## Next Challenge

Once comfortable, try:
- Refactor code to be more efficient
- Add input validation
- Create comprehensive docstrings
- Write additional test cases
