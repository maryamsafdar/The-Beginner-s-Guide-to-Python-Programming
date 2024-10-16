<p><strong>Chapter 5.4: Practical Examples of Functions</strong></p>

<p>In the previous chapters, we have discussed the concept of functions, their types, and how to create and use them in various programming languages. In this chapter, we will explore some practical examples of functions to help you understand their real-world applications.</p>

<p><strong>Example 1: Calculating the Area of a Rectangle</strong></p>

<p>Suppose we want to write a program that calculates the area of a rectangle given its length and width. We can create a function called <code>calculate_area</code> that takes two parameters, <code>length</code> and <code>width</code>, and returns the calculated area.</p>

<p>```python
def calculate_area(length, width):
    """
    Calculate the area of a rectangle.</p>

<pre><code>Args:
    length (float): The length of the rectangle.
    width (float): The width of the rectangle.

Returns:
    float: The calculated area of the rectangle.
"""
return length * width
</code></pre>

<h1>Example usage:</h1>

<p>length = 5
width = 3
area = calculate_area(length, width)
print(f"The area of the rectangle is {area} square units.")
```</p>

<p>In this example, the <code>calculate_area</code> function takes two parameters, <code>length</code> and <code>width</code>, and returns their product, which is the calculated area of the rectangle.</p>

<p><strong>Example 2: Converting Celsius to Fahrenheit</strong></p>

<p>Suppose we want to write a program that converts a temperature from Celsius to Fahrenheit. We can create a function called <code>convert_celsius_to_fahrenheit</code> that takes a single parameter, <code>celsius</code>, and returns the converted temperature in Fahrenheit.</p>

<p>```python
def convert<em>celsius</em>to_fahrenheit(celsius):
    """
    Convert a temperature from Celsius to Fahrenheit.</p>

<pre><code>Args:
    celsius (float): The temperature in Celsius.

Returns:
    float: The converted temperature in Fahrenheit.
"""
return (celsius * 9/5) + 32
</code></pre>

<h1>Example usage:</h1>

<p>celsius = 25
fahrenheit = convert<em>celsius</em>to_fahrenheit(celsius)
print(f"{celsius} degrees Celsius is equal to {fahrenheit} degrees Fahrenheit.")
```</p>

<p>In this example, the <code>convert_celsius_to_fahrenheit</code> function takes a single parameter, <code>celsius</code>, and returns the converted temperature in Fahrenheit using the formula <code>(celsius * 9/5) + 32</code>.</p>

<p><strong>Example 3: Checking if a Number is Even or Odd</strong></p>

<p>Suppose we want to write a program that checks if a given number is even or odd. We can create a function called <code>check_even_or_odd</code> that takes a single parameter, <code>number</code>, and returns a string indicating whether the number is even or odd.</p>

<p>```python
def check<em>even</em>or_odd(number):
    """
    Check if a number is even or odd.</p>

<pre><code>Args:
    number (int): The number to check.

Returns:
    str: A string indicating whether the number is even or odd.
"""
if number % 2 == 0:
    return "The number is even."
else:
    return "The number is odd."
</code></pre>

<h1>Example usage:</h1>

<p>number = 10
result = check<em>even</em>or_odd(number)
print(result)
```</p>

<p>In this example, the <code>check_even_or_odd</code> function takes a single parameter, <code>number</code>, and returns a string indicating whether the number is even or odd using the modulo operator (<code>%</code>).</p>

<p><strong>Example 4: Finding the Maximum of Three Numbers</strong></p>

<p>Suppose we want to write a program that finds the maximum of three given numbers. We can create a function called <code>find_max</code> that takes three parameters, <code>a</code>, <code>b</code>, and <code>c</code>, and returns the maximum of the three numbers.</p>

<p>```python
def find_max(a, b, c):
    """
    Find the maximum of three numbers.</p>

<pre><code>Args:
    a (int): The first number.
    b (int): The second number.
    c (int): The third number.

Returns:
    int: The maximum of the three numbers.
"""
return max(a, b, c)
</code></pre>

<h1>Example usage:</h1>

<p>a = 10
b = 20
c = 30
max<em>value = find</em>max(a, b, c)
print(f"The maximum of {a}, {b}, and {c} is {max_value}.")
```</p>

<p>In this example, the <code>find_max</code> function takes three parameters, <code>a</code>, <code>b</code>, and <code>c</code>, and returns the maximum of the three numbers using the built-in <code>max</code> function.</p>

<p><strong>Example 5: Calculating the Sum of an Array</strong></p>

<p>Suppose we want to write a program that calculates the sum of an array of numbers. We can create a function called <code>calculate_sum</code> that takes an array as a parameter and returns the calculated sum.</p>

<p>```python
def calculate_sum(numbers):
    """
    Calculate the sum of an array of numbers.</p>

<pre><code>Args:
    numbers (list): The array of numbers.

Returns:
    float: The calculated sum of the array.
"""
return sum(numbers)
</code></pre>

<h1>Example usage:</h1>

<p>numbers = [1, 2, 3, 4, 5]
sum<em>value = calculate</em>sum(numbers)
print(f"The sum of the array is {sum_value}.")
```</p>

<p>In this example, the <code>calculate_sum</code> function takes an array as a parameter and returns the calculated sum using the built-in <code>sum</code> function.</p>

<p>In conclusion, functions are a powerful tool in programming that can help us write more efficient, modular, and reusable code. By using functions, we can break down complex tasks into smaller, manageable pieces and make our code more maintainable and scalable.</p>
