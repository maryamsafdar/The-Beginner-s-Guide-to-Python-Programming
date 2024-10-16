<p><strong>Chapter 12.4: Practical Examples of Exception Handling</strong></p>

<p>In the previous chapters, we have discussed the importance of exception handling in programming, the different types of exceptions, and how to handle them using try-catch blocks. In this chapter, we will explore some practical examples of exception handling in various programming scenarios.</p>

<h3>Example 1: Handling File Not Found Exception</h3>

<p>```python
def read_file(filename):
    try:
        with open(filename, 'r') as file:
            content = file.read()
            return content
    except FileNotFoundError:
        print(f"File {filename} not found.")
        return None</p>

<h1>Usage</h1>

<p>filename = 'example.txt'
content = read_file(filename)
if content is not None:
    print(content)
```</p>

<p>In this example, we have a function <code>read_file</code> that attempts to read a file. If the file is not found, a <code>FileNotFoundError</code> exception is raised, which is caught by the <code>except</code> block and handled by printing an error message.</p>

<h3>Example 2: Handling Division by Zero Exception</h3>

<p>```python
def divide_numbers(a, b):
    try:
        result = a / b
        return result
    except ZeroDivisionError:
        print("Cannot divide by zero.")
        return None</p>

<h1>Usage</h1>

<p>a = 10
b = 0
result = divide_numbers(a, b)
if result is not None:
    print(result)
```</p>

<p>In this example, we have a function <code>divide_numbers</code> that attempts to divide two numbers. If the divisor is zero, a <code>ZeroDivisionError</code> exception is raised, which is caught by the <code>except</code> block and handled by printing an error message.</p>

<h3>Example 3: Handling Type Conversion Exception</h3>

<p>```python
def convert<em>to</em>int(s):
    try:
        return int(s)
    except ValueError:
        print(f"Cannot convert {s} to integer.")
        return None</p>

<h1>Usage</h1>

<p>s = 'abc'
result = convert<em>to</em>int(s)
if result is not None:
    print(result)
```</p>

<p>In this example, we have a function <code>convert_to_int</code> that attempts to convert a string to an integer. If the string cannot be converted to an integer, a <code>ValueError</code> exception is raised, which is caught by the <code>except</code> block and handled by printing an error message.</p>

<h3>Example 4: Handling Network Connection Exception</h3>

<p>```python
import requests</p>

<p>def fetch<em>data(url):
    try:
        response = requests.get(url)
        response.raise</em>for_status()
        return response.json()
    except requests.exceptions.RequestException as e:
        print(f"Error fetching data: {e}")
        return None</p>

<h1>Usage</h1>

<p>url = 'https://api.example.com/data'
data = fetch_data(url)
if data is not None:
    print(data)
```</p>

<p>In this example, we have a function <code>fetch_data</code> that attempts to fetch data from a URL using the <code>requests</code> library. If there is a network connection issue, a <code>requests.exceptions.RequestException</code> exception is raised, which is caught by the <code>except</code> block and handled by printing an error message.</p>

<h3>Example 5: Handling Database Connection Exception</h3>

<p>```python
import sqlite3</p>

<p>def connect<em>to</em>database(db<em>name):
    try:
        conn = sqlite3.connect(db</em>name)
        return conn
    except sqlite3.Error as e:
        print(f"Error connecting to database: {e}")
        return None</p>

<h1>Usage</h1>

<p>db<em>name = 'example.db'
conn = connect</em>to<em>database(db</em>name)
if conn is not None:
    print("Connected to database successfully.")
```</p>

<p>In this example, we have a function <code>connect_to_database</code> that attempts to connect to a SQLite database. If there is an issue with the database connection, a <code>sqlite3.Error</code> exception is raised, which is caught by the <code>except</code> block and handled by printing an error message.</p>

<h3>Example 6: Handling User Input Validation Exception</h3>

<p>```python
def validate<em>user</em>input(input<em>str):
    try:
        if not input</em>str.isalpha():
            raise ValueError("Input must be a string of alphabets only.")
        return input_str
    except ValueError as e:
        print(f"Error: {e}")
        return None</p>

<h1>Usage</h1>

<p>input<em>str = 'abc123'
result = validate</em>user<em>input(input</em>str)
if result is not None:
    print(result)
```</p>

<p>In this example, we have a function <code>validate_user_input</code> that attempts to validate user input. If the input is not a string of alphabets only, a <code>ValueError</code> exception is raised, which is caught by the <code>except</code> block and handled by printing an error message.</p>

<h3>Example 7: Handling Custom Exception</h3>

<p>```python
class InsufficientBalanceError(Exception):
    pass</p>

<p>def withdraw_amount(amount):
    try:
        if amount &gt; 100:
            raise InsufficientBalanceError("Insufficient balance.")
        return amount
    except InsufficientBalanceError as e:
        print(f"Error: {e}")
        return None</p>

<h1>Usage</h1>

<p>amount = 150
result = withdraw_amount(amount)
if result is not None:
    print(result)
```</p>

<p>In this example, we have a custom exception <code>InsufficientBalanceError</code> that is raised when the withdrawal amount exceeds the balance. The exception is caught by the <code>except</code> block and handled by printing an error message.</p>

<h3>Example 8: Handling Multiple Exceptions</h3>

<p>```python
def divide_numbers(a, b):
    try:
        result = a / b
        return result
    except (ZeroDivisionError, TypeError):
        print("Error: Invalid input.")
        return None</p>

<h1>Usage</h1>

<p>a = 10
b = 'abc'
result = divide_numbers(a, b)
if result is not None:
    print(result)
```</p>

<p>In this example, we have a function <code>divide_numbers</code> that attempts to divide two numbers. If the divisor is zero or if the input is not a number, a <code>ZeroDivisionError</code> or <code>TypeError</code> exception is raised, respectively. Both exceptions are caught by the <code>except</code> block and handled by printing an error message.</p>

<h3>Example 9: Handling Exception with a Specific Message</h3>

<p>```python
def divide_numbers(a, b):
    try:
        result = a / b
        return result
    except ZeroDivisionError as e:
        print(f"Error: {e}. Please enter a non-zero value for the divisor.")
        return None</p>

<h1>Usage</h1>

<p>a = 10
b = 0
result = divide_numbers(a, b)
if result is not None:
    print(result)
```</p>

<p>In this example, we have a function <code>divide_numbers</code> that attempts to divide two numbers. If the divisor is zero, a <code>ZeroDivisionError</code> exception is raised, and a specific error message is printed.</p>

<h3>Example 10: Handling Exception with a Custom Error Code</h3>

<p>```python
class CustomError(Exception):
    def <strong>init</strong>(self, code, message):
        self.code = code
        self.message = message
        super().<strong>init</strong>(message)</p>

<p>def divide_numbers(a, b):
    try:
        result = a / b
        return result
    except ZeroDivisionError as e:
        raise CustomError(100, f"Error: {e}. Please enter a non-zero value for the divisor.")</p>

<h1>Usage</h1>

<p>a = 10
b = 0
try:
    result = divide_numbers(a, b)
except CustomError as e:
    print(f"Error code: {e.code}. Error message: {e.message}")
```</p>

<p>In this example, we have a custom exception <code>CustomError</code> that is raised when the divisor is zero. The exception includes a custom error code and a specific error message.</p>

<h3>Example 11: Handling Exception with a Retry Mechanism</h3>

<p>```python
import time</p>

<p>def divide<em>numbers(a, b):
    try:
        result = a / b
        return result
    except ZeroDivisionError:
        print("Error: Divisor is zero. Retrying in 5 seconds...")
        time.sleep(5)
        return divide</em>numbers(a, b)</p>

<h1>Usage</h1>

<p>a = 10
b = 0
result = divide_numbers(a, b)
if result is not None:
    print(result)
```</p>

<p>In this example, we have a function <code>divide_numbers</code> that attempts to divide two numbers. If the divisor is zero, a <code>ZeroDivisionError</code> exception is raised, and the function is retried after a 5-second delay.</p>

<h3>Example 12: Handling Exception with a Logging Mechanism</h3>

<p>```python
import logging</p>

<p>logging.basicConfig(level=logging.ERROR)</p>

<p>def divide_numbers(a, b):
    try:
        result = a / b
        return result
    except ZeroDivisionError as e:
        logging.error(f"Error: {e}. Please enter a non-zero value for the divisor.")
        return None</p>

<h1>Usage</h1>

<p>a = 10
b = 0
result = divide_numbers(a, b)
if result is not None:
    print(result)
```</p>

<p>In this example, we have a function <code>divide_numbers</code> that attempts to divide two numbers. If the divisor is zero, a <code>ZeroDivisionError</code> exception is raised, and an error message is logged using the <code>logging</code> module.</p>

<p>In conclusion, exception handling is a crucial aspect of programming that helps to ensure the reliability and robustness of software applications. By using try-catch blocks and handling exceptions in a meaningful way, developers can write more robust and maintainable code. The examples provided in this chapter demonstrate various scenarios where exception handling is essential, and how to handle exceptions in a way that is both effective and efficient.</p>
