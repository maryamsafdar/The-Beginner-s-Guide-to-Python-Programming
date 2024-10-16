<p><strong>Chapter 10.4: Practical Examples of Modules</strong></p>

<p>In the previous chapters, we have discussed the concept of modules, their types, and how to create and use them in programming. In this chapter, we will explore some practical examples of modules based on different scenarios. These examples will help you understand how modules can be applied in real-world situations.</p>

<p><strong>Example 1: Math Module</strong></p>

<p>Suppose we want to create a math module that provides basic mathematical operations such as addition, subtraction, multiplication, and division. We can create a module called <code>math_module.py</code> with the following code:</p>

<p>```python</p>

<h1>math_module.py</h1>

<p>def add(a, b):
    return a + b</p>

<p>def subtract(a, b):
    return a - b</p>

<p>def multiply(a, b):
    return a * b</p>

<p>def divide(a, b):
    if b == 0:
        raise ValueError("Cannot divide by zero")
    return a / b
```</p>

<p>We can then import this module in another script and use its functions:</p>

<p>```python</p>

<h1>main.py</h1>

<p>import math_module</p>

<p>result = math_module.add(5, 3)
print(result)  # Output: 8</p>

<p>result = math_module.subtract(10, 4)
print(result)  # Output: 6</p>

<p>result = math_module.multiply(7, 2)
print(result)  # Output: 14</p>

<p>result = math_module.divide(9, 3)
print(result)  # Output: 3.0
```</p>

<p><strong>Example 2: Database Module</strong></p>

<p>Suppose we want to create a database module that provides functions to connect to a database, execute queries, and retrieve data. We can create a module called <code>database_module.py</code> with the following code:</p>

<p>```python</p>

<h1>database_module.py</h1>

<p>import sqlite3</p>

<p>def connect<em>to</em>database(db<em>name):
    return sqlite3.connect(db</em>name)</p>

<p>def execute_query(conn, query):
    cursor = conn.cursor()
    cursor.execute(query)
    return cursor.fetchall()</p>

<p>def retrieve<em>data(conn, query):
    return execute</em>query(conn, query)
```</p>

<p>We can then import this module in another script and use its functions:</p>

<p>```python</p>

<h1>main.py</h1>

<p>import database_module</p>

<p>conn = database<em>module.connect</em>to_database("example.db")
cursor = conn.cursor()</p>

<p>cursor.execute("CREATE TABLE users (id INTEGER PRIMARY KEY, name TEXT NOT NULL)")</p>

<p>data = database<em>module.retrieve</em>data(conn, "SELECT * FROM users")
print(data)  # Output: []
```</p>

<p><strong>Example 3: File Handling Module</strong></p>

<p>Suppose we want to create a file handling module that provides functions to read and write files. We can create a module called <code>file_handling_module.py</code> with the following code:</p>

<p>```python</p>

<h1>file<em>handling</em>module.py</h1>

<p>def read<em>file(file</em>name):
    with open(file_name, "r") as file:
        return file.read()</p>

<p>def write<em>file(file</em>name, content):
    with open(file_name, "w") as file:
        file.write(content)
```</p>

<p>We can then import this module in another script and use its functions:</p>

<p>```python</p>

<h1>main.py</h1>

<p>import file<em>handling</em>module</p>

<p>content = file<em>handling</em>module.read_file("example.txt")
print(content)  # Output: "Hello, World!"</p>

<p>file<em>handling</em>module.write_file("example.txt", "Goodbye, World!")
```</p>

<p><strong>Example 4: Web Scraping Module</strong></p>

<p>Suppose we want to create a web scraping module that provides functions to extract data from a website. We can create a module called <code>web_scraping_module.py</code> with the following code:</p>

<p>```python</p>

<h1>web<em>scraping</em>module.py</h1>

<p>import requests
from bs4 import BeautifulSoup</p>

<p>def extract<em>data(url):
    response = requests.get(url)
    soup = BeautifulSoup(response.content, "html.parser")
    return soup.find</em>all("h1")
```</p>

<p>We can then import this module in another script and use its functions:</p>

<p>```python</p>

<h1>main.py</h1>

<p>import web<em>scraping</em>module</p>

<p>data = web<em>scraping</em>module.extract_data("https://www.example.com")
print(data)  # Output: [<h1>Example</h1>]
```</p>

<p><strong>Example 5: Machine Learning Module</strong></p>

<p>Suppose we want to create a machine learning module that provides functions to train and predict models. We can create a module called <code>machine_learning_module.py</code> with the following code:</p>

<p>```python</p>

<h1>machine<em>learning</em>module.py</h1>

<p>import numpy as np
from sklearn.linear_model import LinearRegression</p>

<p>def train_model(X, y):
    model = LinearRegression()
    model.fit(X, y)
    return model</p>

<p>def predict_model(model, X):
    return model.predict(X)
```</p>

<p>We can then import this module in another script and use its functions:</p>

<p>```python</p>

<h1>main.py</h1>

<p>import machine<em>learning</em>module</p>

<p>X = np.array([[1, 2], [3, 4]])
y = np.array([2, 4])</p>

<p>model = machine<em>learning</em>module.train<em>model(X, y)
prediction = machine</em>learning<em>module.predict</em>model(model, X)
print(prediction)  # Output: [3. 5.]
```</p>

<p>These examples demonstrate how modules can be used to organize and reuse code in different scenarios. By creating modules for specific tasks, we can make our code more modular, maintainable, and efficient.</p>
