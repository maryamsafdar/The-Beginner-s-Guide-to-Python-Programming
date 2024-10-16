<p><strong>Chapter 6: Manipulating Data with Lists in Python</strong></p>

<p><strong>6.2 Creating and Indexing Lists</strong></p>

<p>In this section, we will delve into the world of lists in Python, exploring how to create and index them. Lists are a fundamental data structure in Python, allowing you to store and manipulate collections of data.</p>

<h3>6.2.1 Creating Lists</h3>

<p>There are several ways to create lists in Python. Here are a few common methods:</p>

<h4>1. Using Square Brackets <code>[]</code></h4>

<p>One of the most straightforward ways to create a list is by using square brackets <code>[]</code>. You can initialize a list with values separated by commas, like this:</p>

<p>```python</p>

<h1>Create a list with values</h1>

<p>my<em>list = [1, 2, 3, 4, 5]
print(my</em>list)  # Output: [1, 2, 3, 4, 5]
```</p>

<h4>2. Using the <code>list()</code> Function</h4>

<p>You can also create a list using the <code>list()</code> function, which takes an iterable as an argument. For example:</p>

<p>```python</p>

<h1>Create a list from a string</h1>

<p>my<em>list = list("hello")
print(my</em>list)  # Output: ['h', 'e', 'l', 'l', 'o']
```</p>

<h4>3. Using the <code>range()</code> Function</h4>

<p>The <code>range()</code> function generates a sequence of numbers, which can be used to create a list. For example:</p>

<p>```python</p>

<h1>Create a list of numbers from 1 to 5</h1>

<p>my<em>list = list(range(1, 6))
print(my</em>list)  # Output: [1, 2, 3, 4, 5]
```</p>

<h3>6.2.2 Indexing Lists</h3>

<p>Once you have created a list, you can access its elements using indexing. Indexing allows you to retrieve a specific element from the list based on its position.</p>

<h4>1. Positive Indexing</h4>

<p>Positive indexing starts from 0, meaning the first element is at index 0, the second element is at index 1, and so on. Here's an example:</p>

<p>```python</p>

<h1>Create a list with values</h1>

<p>my<em>list = [1, 2, 3, 4, 5]
print(my</em>list[0])  # Output: 1
print(my<em>list[1])  # Output: 2
print(my</em>list[2])  # Output: 3
```</p>

<h4>2. Negative Indexing</h4>

<p>Negative indexing starts from the end of the list, meaning the last element is at index -1, the second-to-last element is at index -2, and so on. Here's an example:</p>

<p>```python</p>

<h1>Create a list with values</h1>

<p>my<em>list = [1, 2, 3, 4, 5]
print(my</em>list[-1])  # Output: 5
print(my<em>list[-2])  # Output: 4
print(my</em>list[-3])  # Output: 3
```</p>

<h4>3. Slicing Lists</h4>

<p>Slicing allows you to retrieve a subset of elements from a list. You can use the following syntax: <code>my_list[start:stop:step]</code>. Here's an example:</p>

<p>```python</p>

<h1>Create a list with values</h1>

<p>my<em>list = [1, 2, 3, 4, 5]
print(my</em>list[1:3])  # Output: [2, 3]
print(my_list[1:5:2])  # Output: [2, 4]
```</p>

<p>In this chapter, we have explored the basics of creating and indexing lists in Python. We have seen how to create lists using square brackets, the <code>list()</code> function, and the <code>range()</code> function. We have also learned how to access elements using positive and negative indexing, as well as how to slice lists to retrieve subsets of elements. In the next chapter, we will delve into more advanced list operations, such as modifying elements, inserting and deleting elements, and sorting lists.</p>
