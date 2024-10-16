<p><strong>Chapter 7: Python Syntax Reference</strong></p>

<p>Python is a high-level, interpreted programming language that is widely used for various purposes such as web development, data analysis, machine learning, and more. Its syntax is designed to be simple, readable, and easy to learn. In this chapter, we will explore the basic syntax elements of Python, including variables, data types, control structures, functions, and more.</p>

<h3>7.1 Variables and Data Types</h3>

<p>In Python, a variable is a name given to a value. Variables are used to store and manipulate data in a program. Python has several built-in data types, including:</p>

<ul>
<li><strong>Integers</strong>: Whole numbers, either positive, negative, or zero.</li>
<li><strong>Floats</strong>: Decimal numbers.</li>
<li><strong>Strings</strong>: Sequences of characters, such as words or sentences.</li>
<li><strong>Boolean</strong>: A logical value that can be either True or False.</li>
<li><strong>List</strong>: A collection of items that can be of any data type.</li>
<li><strong>Tuple</strong>: A collection of items that can be of any data type, but is immutable.</li>
<li><strong>Dictionary</strong>: A collection of key-value pairs.</li>
</ul>

<p>Here are some examples of declaring variables and data types in Python:</p>

<p>```python</p>

<h1>Declare an integer variable</h1>

<p>x = 10</p>

<h1>Declare a float variable</h1>

<p>y = 3.14</p>

<h1>Declare a string variable</h1>

<p>name = "John"</p>

<h1>Declare a boolean variable</h1>

<p>is_admin = True</p>

<h1>Declare a list variable</h1>

<p>fruits = ["apple", "banana", "cherry"]</p>

<h1>Declare a tuple variable</h1>

<p>colors = ("red", "green", "blue")</p>

<h1>Declare a dictionary variable</h1>

<p>person = {"name": "Jane", "age": 30}
```</p>

<h3>7.2 Control Structures</h3>

<p>Control structures are used to control the flow of a program. Python has several control structures, including:</p>

<ul>
<li><strong>If-Else Statements</strong>: Used to execute different blocks of code based on a condition.</li>
<li><strong>For Loops</strong>: Used to iterate over a sequence of items.</li>
<li><strong>While Loops</strong>: Used to execute a block of code repeatedly while a condition is true.</li>
</ul>

<p>Here are some examples of control structures in Python:</p>

<p>```python</p>

<h1>If-else statement</h1>

<p>x = 10
if x &gt; 5:
    print("x is greater than 5")
else:
    print("x is less than or equal to 5")</p>

<h1>For loop</h1>

<p>fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)</p>

<h1>While loop</h1>

<p>x = 0
while x &lt; 5:
    print(x)
    x += 1
```</p>

<h3>7.3 Functions</h3>

<p>Functions are reusable blocks of code that can be called multiple times from different parts of a program. Python has several built-in functions, including:</p>

<ul>
<li><strong>Print Function</strong>: Used to print output to the console.</li>
<li><strong>Len Function</strong>: Used to get the length of a sequence.</li>
<li><strong>Max Function</strong>: Used to get the maximum value in a sequence.</li>
<li><strong>Min Function</strong>: Used to get the minimum value in a sequence.</li>
</ul>

<p>Here are some examples of functions in Python:</p>

<p>```python</p>

<h1>Print function</h1>

<p>print("Hello, World!")</p>

<h1>Len function</h1>

<p>fruits = ["apple", "banana", "cherry"]
print(len(fruits))</p>

<h1>Max function</h1>

<p>numbers = [10, 20, 30, 40, 50]
print(max(numbers))</p>

<h1>Min function</h1>

<p>numbers = [10, 20, 30, 40, 50]
print(min(numbers))
```</p>

<h3>7.4 Modules</h3>

<p>Modules are pre-written code that can be imported into a program to perform specific tasks. Python has several built-in modules, including:</p>

<ul>
<li><strong>Math Module</strong>: Provides mathematical functions such as sin, cos, and tan.</li>
<li><strong>Random Module</strong>: Provides functions for generating random numbers.</li>
<li><strong>Time Module</strong>: Provides functions for working with time and dates.</li>
</ul>

<p>Here are some examples of modules in Python:</p>

<p>```python</p>

<h1>Import math module</h1>

<p>import math</p>

<h1>Use math module functions</h1>

<p>print(math.sin(3.14))
print(math.cos(3.14))</p>

<h1>Import random module</h1>

<p>import random</p>

<h1>Use random module functions</h1>

<p>print(random.randint(1, 10))</p>

<h1>Import time module</h1>

<p>import time</p>

<h1>Use time module functions</h1>

<p>print(time.time())
```</p>

<h3>7.5 Exception Handling</h3>

<p>Exception handling is used to handle errors that occur during the execution of a program. Python has several built-in exception types, including:</p>

<ul>
<li><strong>ValueError</strong>: Raised when a value is invalid.</li>
<li><strong>TypeError</strong>: Raised when a value is of the wrong type.</li>
<li><strong>ZeroDivisionError</strong>: Raised when a division by zero occurs.</li>
</ul>

<p>Here are some examples of exception handling in Python:</p>

<p>```python</p>

<h1>Try-except block</h1>

<p>try:
    x = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero!")</p>

<h1>Try-except-else block</h1>

<p>try:
    x = 10 / 2
except ZeroDivisionError:
    print("Cannot divide by zero!")
else:
    print("Division successful!")</p>

<h1>Try-except-finally block</h1>

<p>try:
    x = 10 / 2
except ZeroDivisionError:
    print("Cannot divide by zero!")
finally:
    print("Division complete!")
```</p>

<p>In this chapter, we have covered the basic syntax elements of Python, including variables, data types, control structures, functions, modules, and exception handling. By mastering these concepts, you will be able to write efficient and effective Python code.</p>
