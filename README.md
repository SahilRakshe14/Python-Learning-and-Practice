# Python Learning and Practice

A complete collection of Python programming notes, concepts, practical examples, and outputs based on the MCA Python Programming syllabus.

This repository covers Python fundamentals, functions, data structures, regular expressions, modules, and object-oriented programming.

The main goal of this repository is to understand Python concepts through simple explanations and practical examples.

---

# Table of Contents

- [Unit 1: Fundamentals of Python Programming](#unit-1-fundamentals-of-python-programming)
- [Unit 2: Functions and Data Structures](#unit-2-functions-and-data-structures)
- [Unit 3: Regular Expressions and Modules](#unit-3-regular-expressions-and-modules)
- [Unit 4: Object-Oriented Programming](#unit-4-object-oriented-programming)

---

# Unit 1: Fundamentals of Python Programming

## 1. Introduction to Python

Python is a high-level, interpreted, general-purpose programming language.

It was created by Guido van Rossum and first released in 1991.

Python has simple syntax and is easy to learn and understand.

### Features of Python

1. Easy to Learn: Python has simple and readable syntax.
2. Interpreted Language: Python code is executed by an interpreter.
3. High-Level Language: Programmers do not need to manage low-level system details.
4. Open Source: Python is freely available.
5. Platform Independent: Python works on Windows, Linux, and macOS.
6. Object-Oriented: Python supports object-oriented programming.
7. Large Standard Library: Python provides many built-in modules.

### Applications of Python

- Web Development
- Artificial Intelligence
- Machine Learning
- Data Science
- Automation
- Game Development
- Software Development

### Python Installation

Python can be downloaded from the official website:

https://www.python.org/

To check the installed Python version:

```bash
python3 --version
```

Output:

```text
Python 3.x.x
```

## 2. Python Data Types

A data type defines the type of value stored in a variable.

Python provides different built-in data types.

| Data Type | Description | Example |
|---|---|---|
| int | Integer numbers | 10 |
| float | Decimal numbers | 10.5 |
| complex | Complex numbers | 2+3j |
| str | Text values | "Python" |
| bool | True or False | True |
| list | Ordered, mutable collection | [10, 20] |
| tuple | Ordered, immutable collection | (10, 20) |
| set | Unique elements | {10, 20} |
| dict | Key-value pairs | {"name": "Sahil"} |

Example:

```python
a = 10
b = 10.5
name = "Python"
is_valid = True

print(type(a))
print(type(b))
print(type(name))
print(type(is_valid))
```

Output:

```text
<class 'int'>
<class 'float'>
<class 'str'>
<class 'bool'>
```

## 3. Variables

A variable is a name used to store data in a program.

Python does not require us to declare the variable type separately.

Example:

```python
name = "Sahil"
age = 22
marks = 85.5

print(name)
print(age)
print(marks)
```

Output:

```text
Sahil
22
85.5
```

### Rules for Naming Variables

- A variable name must start with a letter or underscore.
- It cannot start with a number.
- It can contain letters, numbers, and underscores.
- Variable names are case-sensitive.
- Python keywords cannot be used as variable names.

Valid names:

```python
name = "Sahil"
student_age = 22
_marks = 90
```

Invalid names:

```python
# 2name = "Sahil"
# student-age = 22
# class = "MCA"
```

## 4. Identifiers

Identifiers are names given to variables, functions, classes, and other objects in Python.

Example:

```python
student_name = "Sahil"

def display():
    print(student_name)

display()
```

Output:

```text
Sahil
```

Here, `student_name` and `display` are identifiers.

## 5. Keywords

Keywords are reserved words that have special meanings in Python.

They cannot be used as variable names.

Examples of Python keywords:

```text
if, else, elif, for, while, break, continue,
pass, def, return, class, try, except,
finally, import, from, as, True, False,
None, and, or, not, in, is, lambda
```

To display Python keywords:

```python
import keyword

print(keyword.kwlist)
```

Output:

```text
['False', 'None', 'True', 'and', 'as', ...]
```

The complete list depends on the Python version.

## 6. Literals

Literals are fixed values written directly in a Python program.

Types of literals:

1. Numeric Literals
2. String Literals
3. Boolean Literals
4. Special Literal
5. Collection Literals

Example:

```python
age = 22
price = 99.50
name = "Sahil"
is_student = True
value = None

print(age)
print(price)
print(name)
print(is_student)
print(value)
```

Output:

```text
22
99.5
Sahil
True
None
```

## 7. Strings

A string is a sequence of characters enclosed in single, double, or triple quotation marks.

Example:

```python
name = "Python"
message = 'Welcome'

print(name)
print(message)
print(name[0])
print(name[1])
```

Output:

```text
Python
Welcome
P
y
```

### String Slicing

Slicing is used to access a part of a string.

Syntax:

```python
string[start:end:step]
```

Example:

```python
text = "Python Programming"

print(text[0:6])
print(text[7:18])
print(text[::-1])
```

Output:

```text
Python
Programming
gnimmargorP nohtyP
```

### Common String Methods

```python
text = "python programming"

print(text.upper())
print(text.capitalize())
print(text.title())
print(text.replace("python", "Java"))
print(len(text))
```

Output:

```text
PYTHON PROGRAMMING
Python programming
Python Programming
Java programming
18
```

### String Concatenation

Concatenation means joining two or more strings.

```python
first = "Hello"
second = "Python"

result = first + " " + second

print(result)
```

Output:

```text
Hello Python
```

### String Repetition

```python
print("Python " * 3)
```

Output:

```text
Python Python Python
```

## 8. Operators in Python

Operators are symbols or keywords used to perform operations on values and variables.

### A. Arithmetic Operators

Arithmetic operators perform mathematical operations.

| Operator | Meaning | Example |
|---|---|---|
| + | Addition | 10 + 5 |
| - | Subtraction | 10 - 5 |
| * | Multiplication | 10 * 5 |
| / | Division | 10 / 5 |
| // | Floor Division | 10 // 3 |
| % | Modulus | 10 % 3 |
| ** | Exponentiation | 2 ** 3 |

Example:

```python
a = 10
b = 3

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a // b)
print(a % b)
print(a ** b)
```

Output:

```text
13
7
30
3.3333333333333335
3
1
1000
```

### B. Relational Operators

Relational operators compare two values and return True or False.

| Operator | Meaning |
|---|---|
| == | Equal to |
| != | Not equal to |
| > | Greater than |
| < | Less than |
| >= | Greater than or equal to |
| <= | Less than or equal to |

Example:

```python
a = 10
b = 20

print(a == b)
print(a != b)
print(a > b)
print(a < b)
print(a >= b)
print(a <= b)
```

Output:

```text
False
True
False
True
False
True
```

### C. Logical Operators

Logical operators combine conditional expressions.

- `and`: True if both conditions are True.
- `or`: True if at least one condition is True.
- `not`: Reverses the result.

Example:

```python
a = 10
b = 20

print(a < 15 and b > 15)
print(a > 15 or b > 15)
print(not(a > 15))
```

Output:

```text
True
True
True
```

### D. Boolean Operators and Boolean Values

Boolean values are `True` and `False`.

Example:

```python
is_active = True
is_admin = False

print(is_active)
print(is_admin)
print(is_active and is_admin)
```

Output:

```text
True
False
False
```

### E. Assignment Operators

Assignment operators assign or update variable values.

| Operator | Example | Meaning |
|---|---|---|
| = | a = 10 | Assign |
| += | a += 5 | Add and assign |
| -= | a -= 5 | Subtract and assign |
| *= | a *= 2 | Multiply and assign |
| /= | a /= 2 | Divide and assign |
| //= | a //= 2 | Floor divide and assign |
| %= | a %= 3 | Modulus and assign |
| **= | a **= 2 | Power and assign |

Example:

```python
a = 10

a += 5
print(a)

a -= 3
print(a)

a *= 2
print(a)
```

Output:

```text
15
12
24
```

### F. Membership Operators

Membership operators check whether a value exists in a sequence.

- `in`: Returns True if the value exists.
- `not in`: Returns True if the value does not exist.

Example:

```python
name = "Python"

print("P" in name)
print("z" in name)
print("z" not in name)
```

Output:

```text
True
False
True
```

### G. Identity Operators

Identity operators check whether two variables refer to the same object.

- `is`
- `is not`

Example:

```python
a = [10, 20]
b = a
c = [10, 20]

print(a is b)
print(a is c)
print(a is not c)
```

Output:

```text
True
False
True
```

Note: `==` compares values, while `is` compares object identity.

### H. Bitwise Operators

Bitwise operators perform operations on the binary representation of integers.

| Operator | Meaning |
|---|---|
| & | Bitwise AND |
| \| | Bitwise OR |
| ^ | Bitwise XOR |
| ~ | Bitwise NOT |
| << | Left Shift |
| >> | Right Shift |

Example:

```python
a = 5
b = 3

print(a & b)
print(a | b)
print(a ^ b)
print(~a)
print(a << 1)
print(a >> 1)
```

Output:

```text
1
7
6
-6
10
2
```

### I. Increment and Decrement

Python does not support `++` and `--` as increment and decrement operators like C or Java.

We use `+=` and `-=` instead.

Example:

```python
a = 10

a += 1
print(a)

a -= 1
print(a)
```

Output:

```text
11
10
```

## 9. Comments in Python

Comments are used to explain code. They are ignored during program execution.

### Single-Line Comment

A single-line comment starts with `#`.

```python
# This is a single-line comment

print("Hello Python")
```

Output:

```text
Hello Python
```

### Multi-Line Comments

Python does not have a separate multi-line comment symbol. Multiple `#` lines are commonly used.

```python
# This program displays
# a welcome message
# using Python.

print("Welcome to Python")
```

Output:

```text
Welcome to Python
```

Triple-quoted strings are also used for documentation and docstrings.

## 10. Input and Output Statements

### Output Using print()

The `print()` function displays information on the screen.

Example:

```python
print("Hello World")
print(10 + 20)
```

Output:

```text
Hello World
30
```

### Input Using input()

The `input()` function accepts data from the user.

By default, it returns a string.

Example:

```python
name = input("Enter your name: ")
print("Welcome", name)
```

Output:

```text
Enter your name: Sahil
Welcome Sahil
```

### Type Conversion of Input

```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

print("Sum =", a + b)
```

Output:

```text
Enter first number: 10
Enter second number: 20
Sum = 30
```

## 11. Type Conversion and Type Casting

Type conversion means changing one data type into another.

### Implicit Type Conversion

Python automatically converts one data type into another when appropriate.

Example:

```python
a = 10
b = 2.5

result = a + b

print(result)
print(type(result))
```

Output:

```text
12.5
<class 'float'>
```

### Explicit Type Casting

Explicit conversion is performed manually using functions such as `int()`, `float()`, and `str()`.

Example:

```python
a = "100"
b = int(a)

print(b)
print(type(b))
```

Output:

```text
100
<class 'int'>
```

## 12. Conditional Statements

Conditional statements execute code depending on a condition.

### A. if Statement

The `if` statement executes a block when the condition is True.

Syntax:

```python
if condition:
    statement
```

Example:

```python
age = 20

if age >= 18:
    print("Eligible to vote")
```

Output:

```text
Eligible to vote
```

### B. if-else Statement

The `else` block executes when the if condition is False.

Example:

```python
age = 16

if age >= 18:
    print("Eligible to vote")
else:
    print("Not eligible to vote")
```

Output:

```text
Not eligible to vote
```

### C. if-elif-else Statement

The `elif` statement checks additional conditions.

Example:

```python
marks = 75

if marks >= 90:
    print("Grade A")
elif marks >= 70:
    print("Grade B")
elif marks >= 50:
    print("Grade C")
else:
    print("Fail")
```

Output:

```text
Grade B
```

### D. Nested if Statement

An if statement inside another if statement is called a nested if statement.

Example:

```python
age = 22
has_id = True

if age >= 18:
    if has_id:
        print("Entry allowed")
    else:
        print("ID required")
else:
    print("Entry not allowed")
```

Output:

```text
Entry allowed
```

## 13. Indentation in Python

Indentation means spaces at the beginning of a line.

Python uses indentation to define blocks of code.

Example:

```python
age = 20

if age >= 18:
    print("Adult")
    print("Eligible")
```

Output:

```text
Adult
Eligible
```

Incorrect indentation can cause an `IndentationError`.

Python commonly uses four spaces for each indentation level.

## 14. Iteration and Loops

Loops are used to execute a block of code repeatedly.

Python provides two main loops:

1. for loop
2. while loop

### A. for Loop

The `for` loop is used to iterate over a sequence.

Syntax:

```python
for variable in sequence:
    statement
```

Example:

```python
for i in range(1, 6):
    print(i)
```

Output:

```text
1
2
3
4
5
```

### B. while Loop

The `while` loop executes as long as its condition is True.

Example:

```python
i = 1

while i <= 5:
    print(i)
    i += 1
```

Output:

```text
1
2
3
4
5
```

### C. Nested Loops

A loop inside another loop is called a nested loop.

Example:

```python
for i in range(1, 3):
    for j in range(1, 3):
        print(i, j)
```

Output:

```text
1 1
1 2
2 1
2 2
```

## 15. Loop Control Statements

Loop control statements change the normal execution of loops.

### A. break

The `break` statement terminates the loop immediately.

Example:

```python
for i in range(1, 6):
    if i == 3:
        break
    print(i)
```

Output:

```text
1
2
```

### B. continue

The `continue` statement skips the current iteration and moves to the next iteration.

Example:

```python
for i in range(1, 6):
    if i == 3:
        continue
    print(i)
```

Output:

```text
1
2
4
5
```

### C. pass

The `pass` statement does nothing. It is used as a placeholder.

Example:

```python
for i in range(1, 4):
    if i == 2:
        pass
    print(i)
```

Output:

```text
1
2
3
```

### Difference Between break, continue and pass

| Statement | Meaning |
|---|---|
| break | Terminates the loop |
| continue | Skips the current iteration |
| pass | Does nothing |

## 16. Exit Functions

Exit functions are used to terminate program execution.

### exit()

The `exit()` function is commonly used in interactive Python environments.

### sys.exit()

The `sys.exit()` function raises the `SystemExit` exception and terminates the program.

Example:

```python
import sys

print("Program started")

sys.exit()

print("Program ended")
```

Output:

```text
Program started
```

The last print statement is not executed.

---

# Unit 2: Functions and Data Structures

## 17. Functions in Python

A function is a reusable block of code that performs a specific task.

Functions help reduce code repetition and improve program organization.

### Types of Functions

1. Built-in Functions
2. User-Defined Functions

### A. Built-in Functions

Built-in functions are already provided by Python.

Examples:

```python
numbers = [10, 20, 30, 40]

print(len(numbers))
print(max(numbers))
print(min(numbers))
print(sum(numbers))
print(type(numbers))
```

Output:

```text
4
40
10
100
<class 'list'>
```

### B. Math Module

The math module provides mathematical functions.

Example:

```python
import math

print(math.sqrt(25))
print(math.factorial(5))
print(math.ceil(4.2))
print(math.floor(4.8))
```

Output:

```text
5.0
120
5
4
```

### C. Statistics Module

The statistics module provides functions for statistical calculations.

Example:

```python
import statistics

numbers = [10, 20, 30, 40, 50]

print(statistics.mean(numbers))
print(statistics.median(numbers))
```

Output:

```text
30
30
```

## 18. User-Defined Functions

A user-defined function is created by the programmer using the `def` keyword.

Syntax:

```python
def function_name():
    statements
```

Example:

```python
def greet():
    print("Welcome to Python")

greet()
```

Output:

```text
Welcome to Python
```

## 19. Function Arguments

Arguments are values passed to a function when it is called.

Python supports different types of arguments.

### A. Positional Arguments

Values are passed according to their position.

Example:

```python
def student(name, age):
    print(name, age)

student("Sahil", 22)
```

Output:

```text
Sahil 22
```

### B. Default Arguments

Default arguments have predefined values.

Example:

```python
def greet(name="Student"):
    print("Hello", name)

greet()
greet("Sahil")
```

Output:

```text
Hello Student
Hello Sahil
```

### C. Keyword Arguments

Arguments are passed using parameter names.

Example:

```python
def student(name, age):
    print("Name:", name)
    print("Age:", age)

student(age=22, name="Sahil")
```

Output:

```text
Name: Sahil
Age: 22
```

### D. Variable-Length Arguments (*args)

Variable-length arguments allow a function to accept multiple positional arguments.

Example:

```python
def add(*numbers):
    print(sum(numbers))

add(10, 20, 30)
```

Output:

```text
60
```

### E. Variable-Length Keyword Arguments (**kwargs)

`**kwargs` allows a function to accept multiple keyword arguments.

Example:

```python
def student(**details):
    print(details)

student(name="Sahil", age=22, city="Pune")
```

Output:

```text
{'name': 'Sahil', 'age': 22, 'city': 'Pune'}
```

## 20. Scope of Variables

Scope defines where a variable can be accessed in a program.

### A. Local Variable

A local variable is created inside a function.

Example:

```python
def display():
    message = "Hello Python"
    print(message)

display()
```

Output:

```text
Hello Python
```

### B. Global Variable

A global variable is declared outside a function and can be accessed throughout the module.

Example:

```python
message = "Welcome"

def display():
    print(message)

display()
print(message)
```

Output:

```text
Welcome
Welcome
```

### global Keyword

The `global` keyword allows a function to modify a global variable.

Example:

```python
count = 10

def update():
    global count
    count = 20

update()
print(count)
```

Output:

```text
20
```

## 21. return Statement

The `return` statement sends a result from a function back to the caller.

Example:

```python
def add(a, b):
    return a + b

result = add(10, 20)

print(result)
```

Output:

```text
30
```

## 22. Recursion

Recursion is a process in which a function calls itself.

A recursive function must have a base condition to stop repeated calls.

Example: Factorial of a number.

```python
def factorial(n):
    if n == 0 or n == 1:
        return 1
    return n * factorial(n - 1)

print(factorial(5))
```

Output:

```text
120
```

## 23. Importing Modules

A module is a Python file containing reusable functions, classes, and variables.

The `import` keyword is used to include a module in a program.

Example:

```python
import math

print(math.sqrt(64))
print(math.pi)
```

Output:

```text
8.0
3.141592653589793
```

### Importing Specific Functions

```python
from math import sqrt

print(sqrt(49))
```

Output:

```text
7.0
```

### Module Aliasing

An alias is an alternative name given to a module.

Example:

```python
import math as m

print(m.sqrt(81))
```

Output:

```text
9.0
```

## 24. Lists

A list is an ordered and mutable collection of elements.

Lists allow duplicate values and can store different data types.

Example:

```python
numbers = [10, 20, 30, 40]

print(numbers)
print(numbers[0])
print(numbers[-1])
```

Output:

```text
[10, 20, 30, 40]
10
40
```

### A. Adding Items to a List

The `append()` method adds an element at the end.

The `insert()` method adds an element at a specified position.

The `extend()` method adds multiple elements.

Example:

```python
numbers = [10, 20, 30]

numbers.append(40)
numbers.insert(1, 15)
numbers.extend([50, 60])

print(numbers)
```

Output:

```text
[10, 15, 20, 30, 40, 50, 60]
```

### B. Finding Items in a List

The `index()` method returns the position of an element.

The `in` operator checks whether an element exists.

Example:

```python
numbers = [10, 20, 30, 40]

print(numbers.index(30))
print(20 in numbers)
```

Output:

```text
2
True
```

### C. Updating List Items

List elements can be updated using their index.

Example:

```python
numbers = [10, 20, 30]

numbers[1] = 25

print(numbers)
```

Output:

```text
[10, 25, 30]
```

### D. Nested Lists

A list containing another list is called a nested list.

Example:

```python
matrix = [
    [1, 2],
    [3, 4]
]

print(matrix)
print(matrix[0][1])
```

Output:

```text
[[1, 2], [3, 4]]
2
```

### E. Cloning Lists

Cloning means creating a separate copy of a list.

Example:

```python
original = [10, 20, 30]

copy_list = original.copy()

copy_list.append(40)

print(original)
print(copy_list)
```

Output:

```text
[10, 20, 30]
[10, 20, 30, 40]
```

### F. Looping Through a List

A for loop can access each element of a list.

Example:

```python
fruits = ["Apple", "Mango", "Banana"]

for fruit in fruits:
    print(fruit)
```

Output:

```text
Apple
Mango
Banana
```

### G. Sorting a List

The `sort()` method sorts a list.

Example:

```python
numbers = [40, 10, 30, 20]

numbers.sort()

print(numbers)

numbers.sort(reverse=True)

print(numbers)
```

Output:

```text
[10, 20, 30, 40]
[40, 30, 20, 10]
```

### H. List Concatenation

The `+` operator joins two lists.

Example:

```python
a = [10, 20]
b = [30, 40]

result = a + b

print(result)
```

Output:

```text
[10, 20, 30, 40]
```

### I. List Slicing

Slicing accesses a portion of a list.

Example:

```python
numbers = [10, 20, 30, 40, 50]

print(numbers[1:4])
print(numbers[:3])
print(numbers[2:])
print(numbers[::-1])
```

Output:

```text
[20, 30, 40]
[10, 20, 30]
[30, 40, 50]
[50, 40, 30, 20, 10]
```

### J. Common List Methods

| Method | Description |
|---|---|
| append() | Adds an element |
| insert() | Adds an element at a position |
| extend() | Adds multiple elements |
| remove() | Removes a specified element |
| pop() | Removes and returns an element |
| clear() | Removes all elements |
| index() | Returns the element position |
| count() | Counts occurrences |
| sort() | Sorts the list |
| reverse() | Reverses the list |
| copy() | Creates a shallow copy |

Example:

```python
numbers = [10, 20, 30, 20]

print(numbers.count(20))

numbers.remove(20)
print(numbers)

numbers.pop()
print(numbers)
```

Output:

```text
2
[10, 30, 20]
[10, 30]
```

### K. Mutability

Mutability means whether an object can be changed after creation.

Lists are mutable.

Example:

```python
numbers = [10, 20, 30]

numbers[0] = 100

print(numbers)
```

Output:

```text
[100, 20, 30]
```

### L. Aliasing

Aliasing occurs when two variables refer to the same object.

Example:

```python
a = [10, 20, 30]
b = a

b[0] = 100

print(a)
print(b)
```

Output:

```text
[100, 20, 30]
[100, 20, 30]
```

Both variables refer to the same list.

## 25. Tuples

A tuple is an ordered and immutable collection of elements.

Tuples allow duplicate values.

Example:

```python
numbers = (10, 20, 30, 40)

print(numbers)
print(numbers[0])
print(numbers[-1])
```

Output:

```text
(10, 20, 30, 40)
10
40
```

### A. Creating Tuples

```python
a = (10, 20, 30)
b = ("Python", "Java")
c = (10,)
d = ()

print(a)
print(b)
print(c)
print(d)
```

Output:

```text
(10, 20, 30)
('Python', 'Java')
(10,)
()
```

A single-element tuple requires a trailing comma.

### B. Accessing Tuple Elements

```python
fruits = ("Apple", "Mango", "Banana")

print(fruits[0])
print(fruits[1])
```

Output:

```text
Apple
Mango
```

### C. Updating Tuple Elements

Tuples are immutable, so their elements cannot be directly updated.

A tuple can be converted into a list, modified, and converted back.

Example:

```python
numbers = (10, 20, 30)

temp = list(numbers)
temp[1] = 25

numbers = tuple(temp)

print(numbers)
```

Output:

```text
(10, 25, 30)
```

### D. Deleting Tuples

Individual elements cannot be deleted, but the entire tuple can be deleted.

Example:

```python
numbers = (10, 20, 30)

del numbers

print("Tuple deleted")
```

Output:

```text
Tuple deleted
```

### E. Tuple Assignment and Unpacking

Tuple unpacking assigns tuple values to multiple variables.

Example:

```python
student = ("Sahil", 22, "MCA")

name, age, course = student

print(name)
print(age)
print(course)
```

Output:

```text
Sahil
22
MCA
```

### F. Returning Multiple Values

A function can return multiple values as a tuple.

Example:

```python
def calculate(a, b):
    return a + b, a - b

sum_value, difference = calculate(20, 10)

print(sum_value)
print(difference)
```

Output:

```text
30
10
```

### G. Nested Tuples

A tuple containing other tuples is called a nested tuple.

Example:

```python
data = ((10, 20), (30, 40))

print(data[0])
print(data[1][0])
```

Output:

```text
(10, 20)
30
```

### H. Basic Tuple Operations

```python
a = (10, 20)
b = (30, 40)

print(a + b)
print(a * 2)
print(20 in a)
print(len(a))
```

Output:

```text
(10, 20, 30, 40)
(10, 20, 10, 20)
True
2
```

### I. Tuple Methods

| Method | Description |
|---|---|
| count() | Counts occurrences |
| index() | Returns element position |

Example:

```python
numbers = (10, 20, 10, 30)

print(numbers.count(10))
print(numbers.index(20))
```

Output:

```text
2
1
```

## 26. Sets

A set is an unordered collection of unique elements.

Sets do not allow duplicate values.

Example:

```python
numbers = {10, 20, 30, 20}

print(numbers)
```

Output:

```text
{10, 20, 30}
```

Note: Set output order is not guaranteed.

### A. Adding Elements

```python
numbers = {10, 20, 30}

numbers.add(40)

print(numbers)
```

Output:

```text
{10, 20, 30, 40}
```

### B. Removing Elements

```python
numbers = {10, 20, 30}

numbers.remove(20)

print(numbers)
```

Output:

```text
{10, 30}
```

### C. Union

Union combines elements from both sets.

```python
a = {1, 2, 3}
b = {3, 4, 5}

print(a.union(b))
```

Output:

```text
{1, 2, 3, 4, 5}
```

### D. Intersection

Intersection returns common elements.

```python
a = {1, 2, 3}
b = {2, 3, 4}

print(a.intersection(b))
```

Output:

```text
{2, 3}
```

### E. Difference

Difference returns elements present in the first set but not in the second.

```python
a = {1, 2, 3}
b = {2, 3, 4}

print(a.difference(b))
```

Output:

```text
{1}
```

### F. Symmetric Difference

Returns elements that are present in either set, but not in both.

```python
a = {1, 2, 3}
b = {2, 3, 4}

print(a.symmetric_difference(b))
```

Output:

```text
{1, 4}
```

### G. Common Set Methods

| Method | Description |
|---|---|
| add() | Adds an element |
| update() | Adds multiple elements |
| remove() | Removes an element |
| discard() | Removes an element if present |
| pop() | Removes an arbitrary element |
| clear() | Removes all elements |
| union() | Combines sets |
| intersection() | Returns common elements |
| difference() | Returns different elements |

## 27. Dictionaries

A dictionary stores data in key-value pairs.

Dictionaries are mutable and keys must be unique.

Example:

```python
student = {
    "name": "Sahil",
    "age": 22,
    "course": "MCA"
}

print(student)
print(student["name"])
```

Output:

```text
{'name': 'Sahil', 'age': 22, 'course': 'MCA'}
Sahil
```

### A. Adding Dictionary Items

```python
student = {"name": "Sahil"}

student["age"] = 22

print(student)
```

Output:

```text
{'name': 'Sahil', 'age': 22}
```

### B. Updating Dictionary Items

```python
student = {"name": "Sahil", "age": 22}

student["age"] = 23

print(student)
```

Output:

```text
{'name': 'Sahil', 'age': 23}
```

### C. Removing Dictionary Items

```python
student = {
    "name": "Sahil",
    "age": 22
}

student.pop("age")

print(student)
```

Output:

```text
{'name': 'Sahil'}
```

### D. Looping Through a Dictionary

```python
student = {
    "name": "Sahil",
    "age": 22
}

for key, value in student.items():
    print(key, value)
```

Output:

```text
name Sahil
age 22
```

### E. Built-in Dictionary Methods

| Method | Description |
|---|---|
| keys() | Returns all keys |
| values() | Returns all values |
| items() | Returns key-value pairs |
| get() | Returns the value of a key |
| update() | Updates dictionary items |
| pop() | Removes a specified key |
| popitem() | Removes the last inserted pair |
| clear() | Removes all items |
| copy() | Creates a shallow copy |
| setdefault() | Returns a value or inserts a default |

Example:

```python
student = {
    "name": "Sahil",
    "age": 22
}

print(student.keys())
print(student.values())
print(student.get("name"))
print(student.items())
```

Output:

```text
dict_keys(['name', 'age'])
dict_values(['Sahil', 22])
Sahil
dict_items([('name', 'Sahil'), ('age', 22)])
```

---

# Unit 3: Regular Expressions and Modules

## 28. Regular Expressions

A Regular Expression (Regex) is a sequence of characters used to define a search pattern.

Regex is used to search, match, extract, and replace text in strings.

Python provides the built-in `re` module for regular expressions.

### Importance of Regular Expressions

- Searching for specific text.
- Validating email addresses.
- Checking mobile numbers.
- Extracting information from strings.
- Replacing unwanted text.
- Finding patterns in large text files.

### Importing the re Module

```python
import re
```

### Common Regex Special Characters

| Character | Meaning |
|---|---|
| . | Matches any character except newline by default |
| ^ | Matches the beginning of a string |
| $ | Matches the end of a string |
| * | Zero or more repetitions |
| + | One or more repetitions |
| ? | Zero or one repetition |
| [] | Character set |
| {} | Specifies repetition count |
| \d | Matches a digit |
| \D | Matches a non-digit |
| \w | Matches a word character |
| \W | Matches a non-word character |
| \s | Matches whitespace |
| \S | Matches non-whitespace |

### Example: Finding Digits

```python
import re

text = "My age is 22"

result = re.findall(r"\d", text)

print(result)
```

Output:

```text
['2', '2']
```

### Types of Regular Expression Functions

Python provides several functions in the `re` module.

| Function | Description |
|---|---|
| match() | Checks for a match at the beginning |
| search() | Searches for the first match anywhere |
| findall() | Returns all matches in a list |
| finditer() | Returns an iterator of match objects |
| split() | Splits a string using a pattern |
| sub() | Replaces matched text |

### A. match() Function

The `match()` function checks whether a pattern matches at the beginning of a string.

Syntax:

```python
re.match(pattern, string)
```

Example:

```python
import re

text = "Python is easy"

result = re.match("Python", text)

if result:
    print("Pattern matched")
else:
    print("Pattern not matched")
```

Output:

```text
Pattern matched
```

### B. search() Function

The `search()` function searches for the first occurrence of a pattern anywhere in a string.

Example:

```python
import re

text = "I am learning Python"

result = re.search("Python", text)

if result:
    print("Pattern found")
```

Output:

```text
Pattern found
```

### C. findall() Function

The `findall()` function returns all matches as a list.

Example:

```python
import re

text = "My numbers are 10, 20 and 30"

result = re.findall(r"\d+", text)

print(result)
```

Output:

```text
['10', '20', '30']
```

### D. finditer() Function

The `finditer()` function returns an iterator containing match objects.

Example:

```python
import re

text = "A1 B2 C3"

for match in re.finditer(r"\d", text):
    print(match.group())
```

Output:

```text
1
2
3
```

### E. split() Function

The `split()` function splits a string based on a pattern.

Example:

```python
import re

text = "Apple,Mango;Banana"

result = re.split(r"[,;]", text)

print(result)
```

Output:

```text
['Apple', 'Mango', 'Banana']
```

### F. sub() Function

The `sub()` function replaces matched text with another value.

Example:

```python
import re

text = "I like Java"

result = re.sub("Java", "Python", text)

print(result)
```

Output:

```text
I like Python
```

### Example: Check Whether a String Starts with A

```python
import re

text = "Apple"

result = re.match(r"^A", text)

if result:
    print("String starts with A")
else:
    print("String does not start with A")
```

Output:

```text
String starts with A
```

## 29. Modules in Python

A module is a Python file containing functions, classes, and variables that can be reused in another program.

Modules help organize code and avoid repetition.

### Advantages of Modules

- Code reusability.
- Better code organization.
- Easy maintenance.
- Reduced code duplication.
- Access to predefined functions.

### Using import Keyword

The `import` keyword is used to include a module.

Example:

```python
import math

print(math.sqrt(36))
```

Output:

```text
6.0
```

### Using from Keyword

The `from` keyword imports specific functions or objects from a module.

Example:

```python
from math import sqrt, pi

print(sqrt(25))
print(pi)
```

Output:

```text
5.0
3.141592653589793
```

### Module Aliasing

An alias gives a module a shorter or alternative name.

Example:

```python
import math as m

print(m.factorial(5))
```

Output:

```text
120
```

## 30. Namespace in Python

A namespace is a system that stores names and their corresponding objects.

It helps Python identify variables and functions.

### Types of Namespaces

1. Built-in Namespace: Contains built-in names such as `print()` and `len()`.
2. Global Namespace: Contains names defined at the module level.
3. Local Namespace: Contains names defined inside a function.
4. Enclosing Namespace: Contains names in an outer function when functions are nested.

Example:

```python
name = "Global"

def display():
    name = "Local"
    print(name)

display()
print(name)
```

Output:

```text
Local
Global
```

### LEGB Rule

Python searches for variable names in the following order:

- Local
- Enclosing
- Global
- Built-in

## 31. Python Packages and Libraries

A package is a way of organizing related Python modules into a directory structure.

Python also provides external libraries for data analysis, scientific computing, machine learning, and visualization.

### A. NumPy

NumPy stands for Numerical Python.

It is used for numerical and scientific calculations.

Installation:

```bash
pip install numpy
```

Example:

```python
import numpy as np

numbers = np.array([10, 20, 30, 40])

print(numbers)
print(numbers.mean())
print(numbers.sum())
```

Output:

```text
[10 20 30 40]
25.0
100
```

### B. Pandas

Pandas is a Python library used for data manipulation and analysis.

It provides Series and DataFrame data structures.

Installation:

```bash
pip install pandas
```

Example:

```python
import pandas as pd

data = {
    "Name": ["Sahil", "Rahul"],
    "Marks": [85, 90]
}

df = pd.DataFrame(data)

print(df)
```

Output:

```text
    Name  Marks
0  Sahil     85
1  Rahul     90
```

### C. Scikit-learn

Scikit-learn is a machine learning library used for classification, regression, clustering, and model evaluation.

Installation:

```bash
pip install scikit-learn
```

Example:

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()

print(type(model).__name__)
```

Output:

```text
LinearRegression
```

### D. Matplotlib

Matplotlib is a Python library used for data visualization.

It helps create graphs and charts.

Installation:

```bash
pip install matplotlib
```

Example:

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4]
y = [10, 20, 30, 40]

plt.plot(x, y)

plt.title("Simple Line Graph")
plt.xlabel("X Values")
plt.ylabel("Y Values")

plt.show()
```

Output:

A line graph is displayed showing the relationship between the X and Y values.

---

# Unit 4: Object-Oriented Programming

## 32. Introduction to Object-Oriented Programming

Object-Oriented Programming (OOP) is a programming approach based on classes and objects.

It helps organize programs into reusable and manageable structures.

### Main Concepts of OOP

1. Class
2. Object
3. Inheritance
4. Polymorphism
5. Encapsulation
6. Abstraction

## 33. Classes in Python

A class is a blueprint used to create objects.

It defines attributes and methods.

Syntax:

```python
class ClassName:
    statements
```

Example:

```python
class Student:
    name = "Sahil"
    age = 22

    def display(self):
        print(self.name)
        print(self.age)

student = Student()
student.display()
```

Output:

```text
Sahil
22
```

## 34. Objects in Python

An object is an instance of a class.

It can access the attributes and methods defined in its class.

Example:

```python
class Car:
    def start(self):
        print("Car started")

car1 = Car()
car2 = Car()

car1.start()
car2.start()
```

Output:

```text
Car started
Car started
```

## 35. Constructor and self Keyword

A constructor is a special method that initializes an object.

Python uses the `__init__()` method as an initializer.

The `self` parameter refers to the current object.

Example:

```python
class Student:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def display(self):
        print("Name:", self.name)
        print("Age:", self.age)

s1 = Student("Sahil", 22)
s1.display()
```

Output:

```text
Name: Sahil
Age: 22
```

## 36. Instances as Arguments

Objects can be passed as arguments to functions or methods.

Example:

```python
class Student:
    def __init__(self, name):
        self.name = name

def display(student):
    print(student.name)

s1 = Student("Sahil")

display(s1)
```

Output:

```text
Sahil
```

## 37. Instances as Return Values

A function can return an object.

Example:

```python
class Student:
    def __init__(self, name):
        self.name = name

def create_student():
    return Student("Sahil")

s1 = create_student()

print(s1.name)
```

Output:

```text
Sahil
```

## 38. Built-in Class Attributes

Python classes provide built-in attributes that give information about a class.

Common attributes:

| Attribute | Description |
|---|---|
| __name__ | Class name |
| __doc__ | Class documentation |
| __module__ | Module name |
| __dict__ | Namespace dictionary |
| __bases__ | Base classes |

Example:

```python
class Student:
    """Student class example"""

    def display(self):
        print("Hello")

print(Student.__name__)
print(Student.__doc__)
print(Student.__module__)
```

Output:

```text
Student
Student class example
__main__
```

## 39. Inheritance

Inheritance allows one class to acquire properties and methods from another class.

The existing class is called the parent class.

The new class is called the child class.

Example:

```python
class Animal:
    def eat(self):
        print("Animal is eating")

class Dog(Animal):
    def bark(self):
        print("Dog is barking")

d = Dog()

d.eat()
d.bark()
```

Output:

```text
Animal is eating
Dog is barking
```

### Types of Inheritance

1. Single Inheritance
2. Multiple Inheritance
3. Multilevel Inheritance
4. Hierarchical Inheritance
5. Hybrid Inheritance

## 40. Method Overriding

Method overriding occurs when a child class provides its own implementation of a method already defined in the parent class.

Example:

```python
class Animal:
    def sound(self):
        print("Animal makes a sound")

class Dog(Animal):
    def sound(self):
        print("Dog barks")

d = Dog()
d.sound()
```

Output:

```text
Dog barks
```

## 41. Encapsulation

Encapsulation means combining data and methods into a single class.

It helps control access to data.

Python uses naming conventions to indicate different levels of access.

Example:

```python
class Student:
    def __init__(self, name):
        self.name = name

    def display(self):
        print(self.name)

s = Student("Sahil")
s.display()
```

Output:

```text
Sahil
```

## 42. Data Hiding

Data hiding means restricting direct access to internal data.

Python supports name mangling using double underscores.

Example:

```python
class Bank:
    def __init__(self):
        self.__balance = 5000

    def show_balance(self):
        print(self.__balance)

account = Bank()
account.show_balance()
```

Output:

```text
5000
```

Note: Double underscores trigger name mangling. They do not provide strict security or absolute privacy.

## 43. Exception Handling

An exception is an error that occurs during program execution.

Exception handling prevents a program from terminating unexpectedly.

Python uses:

- try
- except
- else
- finally
- raise

### A. try and except

The `try` block contains code that may generate an exception.

The `except` block handles the exception.

Example:

```python
try:
    a = 10
    b = 0

    print(a / b)

except ZeroDivisionError:
    print("Cannot divide by zero")
```

Output:

```text
Cannot divide by zero
```

### B. Multiple except Blocks

A program can handle different exception types using multiple except blocks.

Example:

```python
try:
    number = int("abc")

except ValueError:
    print("Invalid number")

except TypeError:
    print("Type error")
```

Output:

```text
Invalid number
```

### C. else Block

The `else` block executes when no exception occurs.

Example:

```python
try:
    a = 10
    b = 2

    result = a / b

except ZeroDivisionError:
    print("Cannot divide by zero")

else:
    print("Result:", result)
```

Output:

```text
Result: 5.0
```

### D. finally Block

The `finally` block executes whether an exception occurs or not.

Example:

```python
try:
    print("Inside try block")

except:
    print("Error occurred")

finally:
    print("Finally block executed")
```

Output:

```text
Inside try block
Finally block executed
```

### E. raise Keyword

The `raise` keyword is used to generate an exception manually.

Example:

```python
age = 15

if age < 18:
    raise ValueError("Age must be 18 or above")
```

Output:

```text
ValueError: Age must be 18 or above
```

---

# Python Quick Revision

## Important Built-in Functions

| Function | Purpose |
|---|---|
| print() | Displays output |
| input() | Accepts user input |
| type() | Returns data type |
| len() | Returns length |
| range() | Generates a sequence |
| int() | Converts to integer |
| float() | Converts to float |
| str() | Converts to string |
| max() | Returns maximum value |
| min() | Returns minimum value |
| sum() | Returns sum |
| sorted() | Returns sorted list |
| abs() | Returns absolute value |

## Difference Between List, Tuple, Set and Dictionary

| Feature | List | Tuple | Set | Dictionary |
|---|---|---|---|---|
| Syntax | [] | () | {} | {key: value} |
| Ordered | Yes | Yes | No | Yes (insertion order) |
| Mutable | Yes | No | Yes | Yes |
| Duplicates | Allowed | Allowed | Not allowed | Keys must be unique |
| Access | Index | Index | No indexing | Key |

## Important Python Concepts

- Python is case-sensitive.
- Indentation defines code blocks.
- Lists are mutable.
- Tuples are immutable.
- Sets store unique elements.
- Dictionaries store key-value pairs.
- Functions improve code reusability.
- Recursion occurs when a function calls itself.
- Modules contain reusable Python code.
- Regular expressions are used for pattern matching.
- Classes are blueprints for objects.
- Inheritance supports code reuse.
- Exception handling manages runtime errors.

---

# Technologies Used

- Python 3
- Ubuntu Linux
- Visual Studio Code
- Git
- GitHub

# Learning Objectives

- Understand Python programming fundamentals.
- Learn variables, data types, operators, and control statements.
- Develop problem-solving and logical thinking skills.
- Understand functions and data structures.
- Work with regular expressions and Python modules.
- Learn object-oriented programming concepts.
- Practice Python through real code examples.

# Author

**Sahil Rakshe**

MCA Student | Python Programming Learner

GitHub: https://github.com/SahilRakshe14

---

*This repository is maintained for learning, practice, revision, and academic reference.*
