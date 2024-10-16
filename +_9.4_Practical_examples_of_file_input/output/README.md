<p><strong>Chapter 9.4: Practical Examples of File Input/Output</strong></p>

<p>In the previous chapters, we have discussed the basics of file input/output operations in programming. We have covered the different types of files, file modes, and how to perform various operations such as reading, writing, and appending to files. In this chapter, we will put our knowledge into practice by exploring some practical examples of file input/output operations.</p>

<p><strong>Example 1: Reading and Writing a Text File</strong></p>

<p>In this example, we will create a text file and read its contents. We will then modify the contents and write them back to the file.</p>

<p>```python</p>

<h1>Open the file in read mode</h1>

<p>with open('example.txt', 'r') as file:
    # Read the contents of the file
    contents = file.read()
    print(contents)</p>

<h1>Modify the contents</h1>

<p>modified_contents = "This is the modified contents of the file."</p>

<h1>Open the file in write mode</h1>

<p>with open('example.txt', 'w') as file:
    # Write the modified contents to the file
    file.write(modified_contents)
```</p>

<p><strong>Example 2: Reading and Writing a CSV File</strong></p>

<p>In this example, we will create a CSV file and read its contents. We will then modify the contents and write them back to the file.</p>

<p>```python
import csv</p>

<h1>Create a list of data</h1>

<p>data = [
    ['Name', 'Age'],
    ['John', 25],
    ['Alice', 30]
]</p>

<h1>Open the file in write mode</h1>

<p>with open('example.csv', 'w', newline='') as file:
    # Create a CSV writer
    writer = csv.writer(file)
    # Write the data to the file
    writer.writerows(data)</p>

<h1>Open the file in read mode</h1>

<p>with open('example.csv', 'r') as file:
    # Create a CSV reader
    reader = csv.reader(file)
    # Read the contents of the file
    for row in reader:
        print(row)
```</p>

<p><strong>Example 3: Reading and Writing a JSON File</strong></p>

<p>In this example, we will create a JSON file and read its contents. We will then modify the contents and write them back to the file.</p>

<p>```python
import json</p>

<h1>Create a dictionary of data</h1>

<p>data = {
    'name': 'John',
    'age': 25
}</p>

<h1>Open the file in write mode</h1>

<p>with open('example.json', 'w') as file:
    # Write the data to the file
    json.dump(data, file)</p>

<h1>Open the file in read mode</h1>

<p>with open('example.json', 'r') as file:
    # Read the contents of the file
    contents = json.load(file)
    print(contents)
```</p>

<p><strong>Example 4: Appending to a File</strong></p>

<p>In this example, we will append data to an existing file.</p>

<p>```python</p>

<h1>Open the file in append mode</h1>

<p>with open('example.txt', 'a') as file:
    # Write data to the file
    file.write("This is the appended data.\n")
```</p>

<p><strong>Example 5: Reading a File Line by Line</strong></p>

<p>In this example, we will read a file line by line.</p>

<p>```python</p>

<h1>Open the file in read mode</h1>

<p>with open('example.txt', 'r') as file:
    # Read the file line by line
    for line in file:
        print(line.strip())
```</p>

<p><strong>Example 6: Writing a File with Encoding</strong></p>

<p>In this example, we will write a file with a specific encoding.</p>

<p>```python</p>

<h1>Open the file in write mode with encoding</h1>

<p>with open('example.txt', 'w', encoding='utf-8') as file:
    # Write data to the file
    file.write("This is the data written with encoding.")
```</p>

<p><strong>Example 7: Reading a File with Encoding</strong></p>

<p>In this example, we will read a file with a specific encoding.</p>

<p>```python</p>

<h1>Open the file in read mode with encoding</h1>

<p>with open('example.txt', 'r', encoding='utf-8') as file:
    # Read the contents of the file
    contents = file.read()
    print(contents)
```</p>

<p><strong>Example 8: Creating a Temporary File</strong></p>

<p>In this example, we will create a temporary file.</p>

<p>```python
import tempfile</p>

<h1>Create a temporary file</h1>

<p>with tempfile.TemporaryFile() as file:
    # Write data to the file
    file.write(b"This is the data written to the temporary file.")
    # Seek to the beginning of the file
    file.seek(0)
    # Read the contents of the file
    contents = file.read()
    print(contents)
```</p>

<p><strong>Example 9: Deleting a File</strong></p>

<p>In this example, we will delete a file.</p>

<p>```python
import os</p>

<h1>Delete the file</h1>

<p>os.remove('example.txt')
```</p>

<p>In this chapter, we have explored various practical examples of file input/output operations. We have learned how to read and write different types of files, append to files, read files line by line, write files with encoding, read files with encoding, create temporary files, and delete files. These examples will help you to understand how to perform file input/output operations in your programming projects.</p>
