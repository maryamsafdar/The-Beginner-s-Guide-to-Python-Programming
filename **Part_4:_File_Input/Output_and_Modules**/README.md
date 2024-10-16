<p><strong>Chapter 7: Part 4 - File Input/Output and Modules</strong></p>

<p><strong>Introduction</strong></p>

<p>In the previous chapters, we have learned about the basics of Python programming, data types, control structures, functions, and object-oriented programming. In this chapter, we will explore two essential topics in Python programming: file input/output and modules.</p>

<p><strong>File Input/Output</strong></p>

<p>File input/output is a crucial aspect of programming, as it allows us to read and write data to files. Python provides several ways to perform file input/output operations.</p>

<h3>Reading from a File</h3>

<p>To read from a file, we can use the <code>open()</code> function, which returns a file object. We can then use the <code>read()</code> method to read the contents of the file.</p>

<p>```python</p>

<h1>Open a file in read mode</h1>

<p>file = open("example.txt", "r")</p>

<h1>Read the contents of the file</h1>

<p>contents = file.read()</p>

<h1>Print the contents of the file</h1>

<p>print(contents)</p>

<h1>Close the file</h1>

<p>file.close()
```</p>

<p>Alternatively, we can use a <code>with</code> statement to ensure that the file is properly closed after we are done with it.</p>

<p>```python</p>

<h1>Open a file in read mode</h1>

<p>with open("example.txt", "r") as file:
    # Read the contents of the file
    contents = file.read()</p>

<pre><code># Print the contents of the file
print(contents)
</code></pre>

<p>```</p>

<h3>Writing to a File</h3>

<p>To write to a file, we can use the <code>open()</code> function with the <code>w</code> mode.</p>

<p>```python</p>

<h1>Open a file in write mode</h1>

<p>file = open("example.txt", "w")</p>

<h1>Write to the file</h1>

<p>file.write("Hello, World!")</p>

<h1>Close the file</h1>

<p>file.close()
```</p>

<p>Again, we can use a <code>with</code> statement to ensure that the file is properly closed after we are done with it.</p>

<p>```python</p>

<h1>Open a file in write mode</h1>

<p>with open("example.txt", "w") as file:
    # Write to the file
    file.write("Hello, World!")
```</p>

<h3>Appending to a File</h3>

<p>To append to a file, we can use the <code>open()</code> function with the <code>a</code> mode.</p>

<p>```python</p>

<h1>Open a file in append mode</h1>

<p>file = open("example.txt", "a")</p>

<h1>Write to the file</h1>

<p>file.write("Hello, World!")</p>

<h1>Close the file</h1>

<p>file.close()
```</p>

<h3>Reading and Writing CSV Files</h3>

<p>Python provides a <code>csv</code> module that allows us to read and write CSV files.</p>

<p>```python
import csv</p>

<h1>Open a CSV file in read mode</h1>

<p>with open("example.csv", "r") as file:
    # Create a CSV reader
    reader = csv.reader(file)</p>

<pre><code># Read the CSV file
for row in reader:
    print(row)
</code></pre>

<h1>Open a CSV file in write mode</h1>

<p>with open("example.csv", "w", newline="") as file:
    # Create a CSV writer
    writer = csv.writer(file)</p>

<pre><code># Write to the CSV file
writer.writerow(["Name", "Age"])
writer.writerow(["John", 25])
</code></pre>

<p>```</p>

<p><strong>Modules</strong></p>

<p>Modules are pre-written Python code that we can import into our programs to use their functionality. Python has a vast collection of modules that we can use to perform various tasks.</p>

<h3>Importing Modules</h3>

<p>To import a module, we can use the <code>import</code> statement.</p>

<p>```python
import math</p>

<h1>Use the math module</h1>

<p>print(math.pi)
```</p>

<p>Alternatively, we can import specific functions or variables from a module using the <code>from</code> keyword.</p>

<p>```python
from math import pi</p>

<h1>Use the pi variable</h1>

<p>print(pi)
```</p>

<h3>Creating Our Own Modules</h3>

<p>We can create our own modules by writing Python code in a file and saving it with a <code>.py</code> extension. We can then import this module into our programs.</p>

<p>```python</p>

<h1>mymodule.py</h1>

<p>def greet(name):
    print(f"Hello, {name}!")</p>

<h1>main.py</h1>

<p>import mymodule</p>

<h1>Use the greet function</h1>

<p>mymodule.greet("John")
```</p>

<p>In this chapter, we have learned about file input/output and modules in Python. We have seen how to read and write to files, how to use the <code>csv</code> module to read and write CSV files, and how to import and create our own modules. In the next chapter, we will explore more advanced topics in Python programming.</p>
