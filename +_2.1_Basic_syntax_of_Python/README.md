<p><strong>Chapter 2.1: Basic Syntax of Python</strong></p>

<p>Python is a high-level, interpreted programming language that is widely used for various purposes such as web development, data analysis, machine learning, and more. Its simplicity and readability make it an ideal language for beginners and experts alike. In this chapter, we will explore the basic syntax of Python, which is essential for writing Python programs.</p>

<p><strong>Indentation</strong></p>

<p>Python uses indentation to define block-level structure. This means that you need to use spaces or tabs to indent your code to indicate that it belongs to a particular block. The most common way to indent in Python is by using four spaces. You can use either spaces or tabs, but it's recommended to stick to one convention throughout your code.</p>

<p><code>python
if True:
    print("This is a block of code")
    print("It belongs to the if statement")
</code></p>

<p>In the above example, the two <code>print</code> statements are indented under the <code>if</code> statement, indicating that they belong to the same block.</p>

<p><strong>Variables and Data Types</strong></p>

<p>In Python, you can assign a value to a variable using the assignment operator (=). The variable name should be a valid Python identifier, which means it should start with a letter or underscore and can contain letters, digits, and underscores.</p>

<p><code>python
x = 5  # Assigning an integer value to x
y = "Hello"  # Assigning a string value to y
</code></p>

<p>Python has several built-in data types, including:</p>

<ul>
<li>Integers: whole numbers, e.g., 1, 2, 3, etc.</li>
<li>Floats: decimal numbers, e.g., 3.14, -0.5, etc.</li>
<li>Strings: sequences of characters, e.g., "Hello", 'Hello', etc.</li>
<li>Boolean: a logical value that can be either True or False</li>
<li>List: a collection of items, e.g., [1, 2, 3], ["a", "b", "c"], etc.</li>
<li>Tuple: a collection of items that cannot be modified, e.g., (1, 2, 3), ("a", "b", "c"), etc.</li>
</ul>

<p><code>python
x = 5  # Integer
y = 3.14  # Float
z = "Hello"  # String
is_true = True  # Boolean
numbers = [1, 2, 3]  # List
fruits = ("apple", "banana", "cherry")  # Tuple
</code></p>

<p><strong>Operators</strong></p>

<p>Python supports various operators for performing arithmetic, comparison, logical, and assignment operations.</p>

<ul>
<li>Arithmetic operators:
<ul>
<li><code>+</code> (addition)</li>
<li><code>-</code> (subtraction)</li>
<li><code>*</code> (multiplication)</li>
<li><code>/</code> (division)</li>
<li><code>**</code> (exponentiation)</li>
<li><code>%</code> (modulus)</li>
</ul></li>
</ul>

<p><code>python
x = 5
y = 3
print(x + y)  # Output: 8
print(x - y)  # Output: 2
print(x * y)  # Output: 15
print(x / y)  # Output: 1.6666666666666667
print(x ** y)  # Output: 125
print(x % y)  # Output: 2
</code></p>

<ul>
<li>Comparison operators:
<ul>
<li><code>==</code> (equal to)</li>
<li><code>!=</code> (not equal to)</li>
<li><code>&gt;</code> (greater than)</li>
<li><code>&lt;</code> (less than)</li>
<li><code>&gt;=</code> (greater than or equal to)</li>
<li><code>&lt;=</code> (less than or equal to)</li>
</ul></li>
</ul>

<p><code>python
x = 5
y = 3
print(x == y)  # Output: False
print(x != y)  # Output: True
print(x &gt; y)  # Output: True
print(x &lt; y)  # Output: False
print(x &gt;= y)  # Output: True
print(x &lt;= y)  # Output: False
</code></p>

<ul>
<li>Logical operators:
<ul>
<li><code>and</code> (logical and)</li>
<li><code>or</code> (logical or)</li>
<li><code>not</code> (logical not)</li>
</ul></li>
</ul>

<p><code>python
x = True
y = False
print(x and y)  # Output: False
print(x or y)  # Output: True
print(not x)  # Output: False
</code></p>

<ul>
<li>Assignment operators:
<ul>
<li><code>=</code> (assignment)</li>
<li><code>+=</code> (addition assignment)</li>
<li><code>-=</code> (subtraction assignment)</li>
<li><code>*=</code> (multiplication assignment)</li>
<li><code>/=</code> (division assignment)</li>
<li><code>**=</code> (exponentiation assignment)</li>
<li><code>%=</code> (modulus assignment)</li>
</ul></li>
</ul>

<p><code>python
x = 5
x += 3  # x = 8
x -= 2  # x = 6
x *= 2  # x = 12
x /= 2  # x = 6.0
x **= 2  # x = 36
x %= 5  # x = 1
</code></p>

<p>In this chapter, we have covered the basic syntax of Python, including indentation, variables and data types, operators, and more. Understanding these concepts is essential for writing Python programs. In the next chapter, we will explore control structures in Python, including if-else statements, for loops, and while loops.</p>
