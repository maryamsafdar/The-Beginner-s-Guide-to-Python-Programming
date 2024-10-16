<p><strong>Chapter 8.3: Dictionary Methods</strong></p>

<p>In the previous chapters, we have explored the basics of dictionaries in Python, including their creation, indexing, and updating. In this chapter, we will delve into the various methods provided by the dictionary class in Python. These methods enable us to perform a wide range of operations on dictionaries, making them a powerful tool for data manipulation and analysis.</p>

<h3>8.3.1: <code>clear()</code></h3>

<p>The <code>clear()</code> method is used to remove all items from a dictionary. This method does not take any arguments and returns <code>None</code>.</p>

<p>```python</p>

<h1>Create a dictionary</h1>

<p>person = {'name': 'John', 'age': 30, 'city': 'New York'}</p>

<h1>Print the original dictionary</h1>

<p>print("Original Dictionary:", person)</p>

<h1>Clear the dictionary</h1>

<p>person.clear()</p>

<h1>Print the dictionary after clearing</h1>

<p>print("Dictionary after clearing:", person)
```</p>

<p>Output:
<code>
Original Dictionary: {'name': 'John', 'age': 30, 'city': 'New York'}
Dictionary after clearing: {}
</code></p>

<h3>8.3.2: <code>copy()</code></h3>

<p>The <code>copy()</code> method is used to create a copy of a dictionary. This method returns a shallow copy of the dictionary, meaning that it creates a new dictionary with the same keys and values as the original dictionary.</p>

<p>```python</p>

<h1>Create a dictionary</h1>

<p>person = {'name': 'John', 'age': 30, 'city': 'New York'}</p>

<h1>Create a copy of the dictionary</h1>

<p>person_copy = person.copy()</p>

<h1>Modify the original dictionary</h1>

<p>person['age'] = 31</p>

<h1>Print the original dictionary and its copy</h1>

<p>print("Original Dictionary:", person)
print("Dictionary Copy:", person_copy)
```</p>

<p>Output:
<code>
Original Dictionary: {'name': 'John', 'age': 31, 'city': 'New York'}
Dictionary Copy: {'name': 'John', 'age': 30, 'city': 'New York'}
</code></p>

<h3>8.3.3: <code>fromkeys()</code></h3>

<p>The <code>fromkeys()</code> method is used to create a new dictionary with the specified keys and values. This method takes an iterable of keys and an optional value as arguments.</p>

<p>```python</p>

<h1>Create a dictionary with specified keys and values</h1>

<p>fruits = dict.fromkeys(['apple', 'banana', 'cherry'], 'fruit')</p>

<h1>Print the dictionary</h1>

<p>print("Dictionary:", fruits)
```</p>

<p>Output:
<code>
Dictionary: {'apple': 'fruit', 'banana': 'fruit', 'cherry': 'fruit'}
</code></p>

<h3>8.3.4: <code>get()</code></h3>

<p>The <code>get()</code> method is used to retrieve the value for a specified key from a dictionary. This method takes a key and an optional default value as arguments.</p>

<p>```python</p>

<h1>Create a dictionary</h1>

<p>person = {'name': 'John', 'age': 30, 'city': 'New York'}</p>

<h1>Retrieve the value for a specified key</h1>

<p>print("Name:", person.get('name'))
print("Age:", person.get('age'))
print("Occupation:", person.get('occupation', 'Unknown'))
```</p>

<p>Output:
<code>
Name: John
Age: 30
Occupation: Unknown
</code></p>

<h3>8.3.5: <code>items()</code></h3>

<p>The <code>items()</code> method is used to retrieve a view object that displays a list of all key-value pairs in a dictionary.</p>

<p>```python</p>

<h1>Create a dictionary</h1>

<p>person = {'name': 'John', 'age': 30, 'city': 'New York'}</p>

<h1>Retrieve a view object of key-value pairs</h1>

<p>print("Key-Value Pairs:", person.items())
```</p>

<p>Output:
<code>
Key-Value Pairs: dict_items([('name', 'John'), ('age', 30), ('city', 'New York')])
</code></p>

<h3>8.3.6: <code>keys()</code></h3>

<p>The <code>keys()</code> method is used to retrieve a view object that displays a list of all keys in a dictionary.</p>

<p>```python</p>

<h1>Create a dictionary</h1>

<p>person = {'name': 'John', 'age': 30, 'city': 'New York'}</p>

<h1>Retrieve a view object of keys</h1>

<p>print("Keys:", person.keys())
```</p>

<p>Output:
<code>
Keys: dict_keys(['name', 'age', 'city'])
</code></p>

<h3>8.3.7: <code>pop()</code></h3>

<p>The <code>pop()</code> method is used to remove and return a specified key-value pair from a dictionary. This method takes a key as an argument.</p>

<p>```python</p>

<h1>Create a dictionary</h1>

<p>person = {'name': 'John', 'age': 30, 'city': 'New York'}</p>

<h1>Remove and return a specified key-value pair</h1>

<p>print("Removed Key-Value Pair:", person.pop('age'))
print("Dictionary after removing:", person)
```</p>

<p>Output:
<code>
Removed Key-Value Pair: 30
Dictionary after removing: {'name': 'John', 'city': 'New York'}
</code></p>

<h3>8.3.8: <code>popitem()</code></h3>

<p>The <code>popitem()</code> method is used to remove and return a specified key-value pair from a dictionary. This method does not take any arguments.</p>

<p>```python</p>

<h1>Create a dictionary</h1>

<p>person = {'name': 'John', 'age': 30, 'city': 'New York'}</p>

<h1>Remove and return a specified key-value pair</h1>

<p>print("Removed Key-Value Pair:", person.popitem())
print("Dictionary after removing:", person)
```</p>

<p>Output:
<code>
Removed Key-Value Pair: ('age', 30)
Dictionary after removing: {'name': 'John', 'city': 'New York'}
</code></p>

<h3>8.3.9: <code>setdefault()</code></h3>

<p>The <code>setdefault()</code> method is used to retrieve the value for a specified key from a dictionary. If the key does not exist, it sets the key to the specified value and returns the value.</p>

<p>```python</p>

<h1>Create a dictionary</h1>

<p>person = {'name': 'John', 'age': 30, 'city': 'New York'}</p>

<h1>Retrieve the value for a specified key</h1>

<p>print("Name:", person.setdefault('name'))
print("Age:", person.setdefault('age'))
print("Occupation:", person.setdefault('occupation', 'Unknown'))
```</p>

<p>Output:
<code>
Name: John
Age: 30
Occupation: Unknown
</code></p>

<h3>8.3.10: <code>update()</code></h3>

<p>The <code>update()</code> method is used to update a dictionary with the specified key-value pairs. This method takes an iterable of key-value pairs as an argument.</p>

<p>```python</p>

<h1>Create a dictionary</h1>

<p>person = {'name': 'John', 'age': 30, 'city': 'New York'}</p>

<h1>Update the dictionary with specified key-value pairs</h1>

<p>person.update({'age': 31, 'country': 'USA'})</p>

<h1>Print the updated dictionary</h1>

<p>print("Updated Dictionary:", person)
```</p>

<p>Output:
<code>
Updated Dictionary: {'name': 'John', 'age': 31, 'city': 'New York', 'country': 'USA'}
</code></p>

<h3>8.3.11: <code>values()</code></h3>

<p>The <code>values()</code> method is used to retrieve a view object that displays a list of all values in a dictionary.</p>

<p>```python</p>

<h1>Create a dictionary</h1>

<p>person = {'name': 'John', 'age': 30, 'city': 'New York'}</p>

<h1>Retrieve a view object of values</h1>

<p>print("Values:", person.values())
```</p>

<p>Output:
<code>
Values: dict_values(['John', 30, 'New York'])
</code></p>

<p>In this chapter, we have explored the various methods provided by the dictionary class in Python. These methods enable us to perform a wide range of operations on dictionaries, making them a powerful tool for data manipulation and analysis.</p>
