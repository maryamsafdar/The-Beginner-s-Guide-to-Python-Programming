<p><strong>Chapter 8.2: Creating and Indexing Dictionaries</strong></p>

<p>In the world of programming, dictionaries are a fundamental data structure that allows us to store and manipulate collections of key-value pairs. In this chapter, we will delve into the world of dictionaries, exploring how to create and index them in Python.</p>

<p><strong>8.2.1 Introduction to Dictionaries</strong></p>

<p>A dictionary is an unordered collection of key-value pairs, where each key is unique and maps to a specific value. Dictionaries are also known as hash tables or associative arrays. They are a powerful data structure that allows us to store and retrieve data efficiently.</p>

<p><strong>8.2.2 Creating Dictionaries</strong></p>

<p>There are several ways to create a dictionary in Python. Here are a few examples:</p>

<h3>8.2.2.1 Using the <code>dict()</code> Function</h3>

<p>The <code>dict()</code> function is a built-in function in Python that allows us to create a dictionary from a list of key-value pairs. Here is an example:
```python</p>

<h1>Create a dictionary using the dict() function</h1>

<p>fruits = dict(apple=5, banana=10, orange=7)
print(fruits)  # Output: {'apple': 5, 'banana': 10, 'orange': 7}
```</p>

<h3>8.2.2.2 Using the Dictionary Literal Syntax</h3>

<p>We can also create a dictionary using the dictionary literal syntax, which is a more concise way of creating a dictionary. Here is an example:
```python</p>

<h1>Create a dictionary using the dictionary literal syntax</h1>

<p>fruits = {'apple': 5, 'banana': 10, 'orange': 7}
print(fruits)  # Output: {'apple': 5, 'banana': 10, 'orange': 7}
```</p>

<h3>8.2.2.3 Using the <code>dict.fromkeys()</code> Method</h3>

<p>The <code>dict.fromkeys()</code> method is a method that allows us to create a dictionary from a list of keys. Here is an example:
```python</p>

<h1>Create a dictionary using the dict.fromkeys() method</h1>

<p>fruits = dict.fromkeys(['apple', 'banana', 'orange'])
print(fruits)  # Output: {'apple': None, 'banana': None, 'orange': None}
```</p>

<h3>8.2.2.4 Using the <code>dict()</code> Function with a List of Key-Value Pairs</h3>

<p>We can also create a dictionary using the <code>dict()</code> function with a list of key-value pairs. Here is an example:
```python</p>

<h1>Create a dictionary using the dict() function with a list of key-value pairs</h1>

<p>fruits = dict([('apple', 5), ('banana', 10), ('orange', 7)])
print(fruits)  # Output: {'apple': 5, 'banana': 10, 'orange': 7}
```
<strong>8.2.3 Indexing Dictionaries</strong></p>

<p>Indexing a dictionary allows us to access the values associated with specific keys. There are several ways to index a dictionary in Python. Here are a few examples:</p>

<h3>8.2.3.1 Using the Key</h3>

<p>We can index a dictionary using the key. Here is an example:
```python</p>

<h1>Create a dictionary</h1>

<p>fruits = {'apple': 5, 'banana': 10, 'orange': 7}</p>

<h1>Index the dictionary using the key</h1>

<p>print(fruits['apple'])  # Output: 5
```</p>

<h3>8.2.3.2 Using the <code>get()</code> Method</h3>

<p>The <code>get()</code> method is a method that allows us to access the value associated with a key. Here is an example:
```python</p>

<h1>Create a dictionary</h1>

<p>fruits = {'apple': 5, 'banana': 10, 'orange': 7}</p>

<h1>Index the dictionary using the get() method</h1>

<p>print(fruits.get('apple'))  # Output: 5
```</p>

<h3>8.2.3.3 Using the <code>in</code> Operator</h3>

<p>The <code>in</code> operator is a operator that allows us to check if a key is present in the dictionary. Here is an example:
```python</p>

<h1>Create a dictionary</h1>

<p>fruits = {'apple': 5, 'banana': 10, 'orange': 7}</p>

<h1>Check if a key is present in the dictionary</h1>

<p>print('apple' in fruits)  # Output: True
```
<strong>8.2.4 Conclusion</strong></p>

<p>In this chapter, we have explored how to create and index dictionaries in Python. We have seen how to create dictionaries using the <code>dict()</code> function, the dictionary literal syntax, the <code>dict.fromkeys()</code> method, and the <code>dict()</code> function with a list of key-value pairs. We have also seen how to index dictionaries using the key, the <code>get()</code> method, and the <code>in</code> operator. With this knowledge, you should be able to create and index dictionaries in Python with ease.</p>

<p><strong>Exercise</strong></p>

<p>Create a dictionary that stores the names and ages of five people. Use the dictionary literal syntax to create the dictionary. Then, use the <code>get()</code> method to access the age of a person.</p>

<p><strong>Solution</strong></p>

<p>```python</p>

<h1>Create a dictionary</h1>

<p>people = {'John': 25, 'Jane': 30, 'Bob': 35, 'Alice': 20, 'Mike': 40}</p>

<h1>Use the get() method to access the age of a person</h1>

<p>print(people.get('John'))  # Output: 25
```</p>
