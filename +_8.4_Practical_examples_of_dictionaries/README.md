<p><strong>Chapter 8.4: Practical Examples of Dictionaries</strong></p>

<p>In the previous chapters, we have discussed the concept of dictionaries, their types, and their applications in various programming languages. In this chapter, we will explore some practical examples of dictionaries to help you understand their usage in real-world scenarios.</p>

<p><strong>Example 1: Student Information System</strong></p>

<p>Suppose we are developing a student information system that stores information about students, including their names, ages, and grades. We can use a dictionary to store this information, where each student's name is the key and their details are the value.</p>

<p>```python</p>

<h1>Student Information System</h1>

<p>students = {
    "John": {"age": 20, "grade": 85},
    "Alice": {"age": 22, "grade": 90},
    "Bob": {"age": 21, "grade": 78}
}</p>

<h1>Accessing student information</h1>

<p>print(students["John"]["age"])  # Output: 20
print(students["Alice"]["grade"])  # Output: 90
```</p>

<p><strong>Example 2: Shopping Cart</strong></p>

<p>Imagine we are building an e-commerce website that allows users to add items to their shopping cart. We can use a dictionary to store the items in the cart, where each item's name is the key and its quantity is the value.</p>

<p>```python</p>

<h1>Shopping Cart</h1>

<p>cart = {
    "Apple": 2,
    "Banana": 3,
    "Orange": 1
}</p>

<h1>Adding an item to the cart</h1>

<p>cart["Grapes"] = 4</p>

<h1>Removing an item from the cart</h1>

<p>del cart["Banana"]</p>

<h1>Accessing item quantity</h1>

<p>print(cart["Apple"])  # Output: 2
print(cart["Grapes"])  # Output: 4
```</p>

<p><strong>Example 3: Weather Forecast</strong></p>

<p>Suppose we are developing a weather forecasting system that stores information about different cities, including their temperatures and humidity levels. We can use a dictionary to store this information, where each city's name is the key and its weather details are the value.</p>

<p>```python</p>

<h1>Weather Forecast</h1>

<p>weather = {
    "New York": {"temperature": 25, "humidity": 60},
    "Los Angeles": {"temperature": 28, "humidity": 40},
    "Chicago": {"temperature": 22, "humidity": 50}
}</p>

<h1>Accessing weather information</h1>

<p>print(weather["New York"]["temperature"])  # Output: 25
print(weather["Los Angeles"]["humidity"])  # Output: 40
```</p>

<p><strong>Example 4: Game High Scores</strong></p>

<p>Imagine we are building a game that stores high scores for different players. We can use a dictionary to store this information, where each player's name is the key and their high score is the value.</p>

<p>```python</p>

<h1>Game High Scores</h1>

<p>high_scores = {
    "Player1": 1000,
    "Player2": 800,
    "Player3": 1200
}</p>

<h1>Updating a player's high score</h1>

<p>high_scores["Player1"] = 1100</p>

<h1>Accessing a player's high score</h1>

<p>print(high<em>scores["Player2"])  # Output: 800
print(high</em>scores["Player3"])  # Output: 1200
```</p>

<p><strong>Example 5: Configuration File</strong></p>

<p>Suppose we are developing a configuration file that stores settings for different applications. We can use a dictionary to store this information, where each application's name is the key and its settings are the value.</p>

<p>```python</p>

<h1>Configuration File</h1>

<p>config = {
    "Application1": {"theme": "dark", "language": "English"},
    "Application2": {"theme": "light", "language": "Spanish"},
    "Application3": {"theme": "dark", "language": "French"}
}</p>

<h1>Accessing application settings</h1>

<p>print(config["Application1"]["theme"])  # Output: dark
print(config["Application2"]["language"])  # Output: Spanish
```</p>

<p><strong>Example 6: Data Analysis</strong></p>

<p>Imagine we are analyzing a dataset that stores information about different products, including their prices and quantities. We can use a dictionary to store this information, where each product's name is the key and its details are the value.</p>

<p>```python</p>

<h1>Data Analysis</h1>

<p>data = {
    "Product1": {"price": 10.99, "quantity": 100},
    "Product2": {"price": 9.99, "quantity": 50},
    "Product3": {"price": 12.99, "quantity": 200}
}</p>

<h1>Calculating total revenue</h1>

<p>total<em>revenue = sum(product["price"] * product["quantity"] for product in data.values())
print(total</em>revenue)  # Output: 5999.8
```</p>

<p><strong>Example 7: Web Scraping</strong></p>

<p>Suppose we are building a web scraper that stores information about different websites, including their titles and URLs. We can use a dictionary to store this information, where each website's URL is the key and its details are the value.</p>

<p>```python</p>

<h1>Web Scraping</h1>

<p>websites = {
    "https://www.google.com": {"title": "Google", "description": "Search engine"},
    "https://www.facebook.com": {"title": "Facebook", "description": "Social media platform"},
    "https://www.twitter.com": {"title": "Twitter", "description": "Microblogging platform"}
}</p>

<h1>Accessing website information</h1>

<p>print(websites["https://www.google.com"]["title"])  # Output: Google
print(websites["https://www.facebook.com"]["description"])  # Output: Social media platform
```</p>

<p><strong>Example 8: Machine Learning</strong></p>

<p>Imagine we are building a machine learning model that stores information about different features, including their names and values. We can use a dictionary to store this information, where each feature's name is the key and its value is the value.</p>

<p>```python</p>

<h1>Machine Learning</h1>

<p>features = {
    "Feature1": 0.5,
    "Feature2": 0.8,
    "Feature3": 0.2
}</p>

<h1>Accessing feature value</h1>

<p>print(features["Feature1"])  # Output: 0.5
print(features["Feature2"])  # Output: 0.8
```</p>

<p>In conclusion, dictionaries are a powerful data structure that can be used in a wide range of applications, from simple data storage to complex machine learning models. By understanding how to use dictionaries effectively, you can write more efficient and readable code that is easier to maintain and scale.</p>
