[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15470632&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

     Python is a popular programming language known for being easy to read and use. Its key features include:

1. **Simple Syntax**: It's straightforward to write and understand.
2. **Versatile**: It can be used for many tasks like web development, data analysis, and automation.
3. **Large Community**: There are many libraries and tools available.
4. **Cross-Platform**: Works on different operating systems like Windows, Mac, and Linux.

**Examples of use cases**:
- **Web Development**: Building websites with frameworks like Django and Flask.
- **Data Analysis**: Analyzing data with libraries like pandas and NumPy.
- **Automation**: Writing scripts to automate repetitive tasks.
- **Machine Learning**: Developing AI models using TensorFlow and scikit-learn.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
     Go to python.org and download python to my local machine. Then install the extensions for vs code for using python.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
     print("Hello, World!"); . What ever is in the print statement gets written on the console in this case the console will display Hello, World! .

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
     Data Types are as follows in python:
     Integer (int): Whole numbers (e.g., 5, -3).
Float (float): Numbers with decimal points (e.g., 3.14, -0.5).
String (str): Text enclosed in quotes (e.g., "hello", 'world').
Boolean (bool): Represents True or False.
     

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
  
     ### Conditional Statements

**Use**: Conditional statements in Python let you execute certain code only if specific conditions are met. They help make decisions in your programs.

**Example**: `if-else` statement

```python
# Example of an if-else statement
temperature = 30

if temperature > 25:
    print("It's hot outside.")
else:
    print("It's not too hot outside.")
```

In this example, the program checks if the temperature is greater than 25. If it is, it prints "It's hot outside." Otherwise, it prints "It's not too hot outside."

### Loops

**Use**: Loops let you repeat code multiple times. This is useful for tasks like iterating over a list of items or executing code a set number of times.

**Example**: `for` loop

```python
# Example of a for loop
for i in range(5):
    print("Iteration", i)
```

In this example, the `for` loop runs 5 times (from 0 to 4) and prints the iteration number each time. The `range(5)` function generates a sequence of numbers from 0 to 4.

### Summary

- **`if-else` statement**: Makes decisions based on conditions.
- **`for` loop**: Repeats code a specific number of times.

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
  
     ### Functions in Python

**What are Functions?**
Functions are blocks of reusable code that perform a specific task. They help organize your code into smaller, manageable parts, making it easier to read, maintain, and debug.

**Why are They Useful?**
- **Reusability**: Write code once and use it multiple times.
- **Modularity**: Breaks down complex problems into simpler, manageable pieces.
- **Clarity**: Makes code more readable by giving meaningful names to code blocks.

### Example Function

Here’s a Python function that takes two arguments and returns their sum:

```python
def add_numbers(a, b):
    return a + b

# Example of calling the function
result = add_numbers(3, 5)
print("The sum is:", result)
```

**Explanation:**
- `def add_numbers(a, b)`: Defines a function named `add_numbers` with two parameters, `a` and `b`.
- `return a + b`: Adds the two arguments and returns the result.
- `result = add_numbers(3, 5)`: Calls the function with arguments `3` and `5`, storing the result in the variable `result`.
- `print("The sum is:", result)`: Prints the result.

This function makes it easy to add two numbers and can be reused with different values.

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
  
### Lists vs. Dictionaries

- **Lists**:
  - **Order**: Maintains order.
  - **Access**: By index (e.g., `list[0]`).

- **Dictionaries**:
  - **Order**: Maintains insertion order (Python 3.7+).
  - **Access**: By key (e.g., `dict["key"]`).

### Example Script

```python
# List of numbers
numbers = [1, 2, 3, 4, 5]
numbers.append(6)  # Add 6
print("List:", numbers)
print("First element:", numbers[0])

# Dictionary
person = {"name": "Alice", "age": 30}
person["city"] = "New York"  # Add city
print("\nDictionary:", person)
print("Name:", person["name"])
del person["age"]  # Remove age
print("After removing age:", person)
```

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
  
### Exception Handling in Python

**What is Exception Handling?**
Exception handling in Python is a way to manage errors that occur during the execution of a program. It helps prevent the program from crashing and allows you to handle errors gracefully.

**Basic Blocks**:
- **`try`**: Contains the code that might cause an error.
- **`except`**: Contains code that runs if an error occurs.
- **`finally`**: Contains code that runs no matter what, whether an error occurred or not.

### Example Script

```python
try:
    # Code that might cause an error
    result = 10 / 0
except ZeroDivisionError:
    # Code that runs if an error occurs
    print("Cannot divide by zero.")
finally:
    # Code that always runs
    print("Execution completed.")
```

**Explanation**:
- **`try`**: Attempts to divide 10 by 0, which raises a `ZeroDivisionError`.
- **`except ZeroDivisionError`**: Catches the division by zero error and prints a message.
- **`finally`**: Prints "Execution completed." regardless of whether an error occurred.

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

     ### Modules and Packages in Python

**Modules**:
- **Concept**: A module is a single file containing Python code, which can define functions, classes, and variables. It helps organize and reuse code.
- **Use**: Import a module into your script to use its functions and variables.

**Packages**:
- **Concept**: A package is a collection of related modules stored in a directory. It allows for a hierarchical organization of modules.
- **Use**: Import modules from packages using dot notation.

### Importing and Using a Module

**Example with `math` Module**:
The `math` module provides mathematical functions.

```python
import math

# Use a function from the math module
square_root = math.sqrt(16)
print("Square root of 16:", square_root)

# Use another function from the math module
pi_value = math.pi
print("Value of pi:", pi_value)
```

**Explanation**:
- **`import math`**: Imports the `math` module.
- **`math.sqrt(16)`**: Calls the `sqrt` function from the `math` module to compute the square root of 16.
- **`math.pi`**: Accesses the constant `pi` from the `math` module.

11. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
   
      ### Reading from and Writing to Files in Python

**Reading from a File**:
- **Open** the file in read mode (`'r'`).
- **Read** the content.
- **Close** the file.

**Writing to a File**:
- **Open** the file in write mode (`'w'`).
- **Write** the content.
- **Close** the file.

### Script to Read from a File

```python
# Read from a file and print its content
with open('example.txt', 'r') as file:
    content = file.read()
    print("File content:")
    print(content)
```

**Explanation**:
- **`with open('example.txt', 'r')`**: Opens the file `example.txt` in read mode.
- **`file.read()`**: Reads the entire content of the file.
- **`print(content)`**: Prints the file's content.

### Script to Write to a File

```python
# List of strings to write to a file
lines = ["First line", "Second line", "Third line"]

# Write the list of strings to a file
with open('output.txt', 'w') as file:
    for line in lines:
        file.write(line + '\n')
```

**Explanation**:
- **`with open('output.txt', 'w')`**: Opens the file `output.txt` in write mode.
- **`file.write(line + '\n')`**: Writes each string from the list to the file, adding a newline character after each string.

Using the `with` statement ensures that files are properly closed after their block of code is executed.

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


