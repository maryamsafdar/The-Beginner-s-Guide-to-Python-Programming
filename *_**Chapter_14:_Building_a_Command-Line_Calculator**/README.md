<p><strong>Chapter 14: Building a Command-Line Calculator</strong></p>

<p>In this chapter, we will explore the concept of building a command-line calculator using Python. A command-line calculator is a simple program that takes mathematical expressions as input from the user and evaluates them to produce the result. This type of calculator is useful for performing quick calculations without having to open a full-fledged calculator application.</p>

<p><strong>Why Build a Command-Line Calculator?</strong></p>

<p>There are several reasons why building a command-line calculator is a useful exercise:</p>

<ol>
<li><strong>Practice with User Input</strong>: Building a command-line calculator requires handling user input, which is an essential skill for any programmer. You will learn how to read input from the user, validate it, and use it to perform calculations.</li>
<li><strong>Understanding Mathematical Expressions</strong>: A command-line calculator needs to evaluate mathematical expressions, which involves understanding the order of operations, precedence, and syntax.</li>
<li><strong>Error Handling</strong>: A calculator needs to handle errors that may occur during calculation, such as division by zero or invalid input.</li>
</ol>

<p><strong>Designing the Calculator</strong></p>

<p>Before we start coding, let's design the calculator's functionality:</p>

<ol>
<li><strong>Supported Operations</strong>: The calculator will support basic arithmetic operations, including addition, subtraction, multiplication, and division.</li>
<li><strong>Input Format</strong>: The calculator will accept mathematical expressions in the form of strings, where the user can enter numbers and operators separated by spaces.</li>
<li><strong>Output Format</strong>: The calculator will display the result of the calculation as a string.</li>
</ol>

<p><strong>Implementing the Calculator</strong></p>

<p>Here is a simple implementation of the command-line calculator using Python:
```python
import re</p>

<p>def calculate(expression):
    """
    Evaluates a mathematical expression and returns the result.
    """
    try:
        result = eval(expression)
        return str(result)
    except ZeroDivisionError:
        return "Error: Division by zero is not allowed."
    except Exception as e:
        return f"Error: {str(e)}"</p>

<p>def main():
    print("Command-Line Calculator")
    print("------------------------")</p>

<pre><code>while True:
    expression = input("Enter a mathematical expression (or 'quit' to exit): ")
    if expression.lower() == 'quit':
        break

    # Validate input using regular expression
    pattern = r"^[\d\+\-\*\/\. ]+$"
    if not re.match(pattern, expression):
        print("Invalid input. Please enter a valid mathematical expression.")
        continue

    result = calculate(expression)
    print(f"Result: {result}")
</code></pre>

<p>if <strong>name</strong> == "<strong>main</strong>":
    main()
```
<strong>How the Code Works</strong></p>

<p>Here's a step-by-step explanation of the code:</p>

<ol>
<li>The <code>calculate</code> function takes a mathematical expression as input and evaluates it using the <code>eval</code> function. If the expression is valid, it returns the result as a string.</li>
<li>The <code>main</code> function is the entry point of the program. It prints a welcome message and enters a loop where it continuously prompts the user for input.</li>
<li>If the user enters 'quit', the program exits the loop and terminates.</li>
<li>If the user enters an invalid input, the program prints an error message and continues to the next iteration.</li>
<li>If the user enters a valid input, the program calls the <code>calculate</code> function to evaluate the expression and prints the result.</li>
</ol>

<p><strong>Testing the Calculator</strong></p>

<p>To test the calculator, save the code in a file named <code>calculator.py</code> and run it using Python:
<code>bash
$ python calculator.py
</code>
Enter some mathematical expressions, such as <code>2 + 3</code>, <code>4 * 5</code>, or <code>10 / 2</code>, to see the calculator in action.</p>

<p><strong>Conclusion</strong></p>

<p>In this chapter, we built a simple command-line calculator using Python. We learned how to handle user input, validate mathematical expressions, and evaluate them using the <code>eval</code> function. We also discussed error handling and how to display the result of the calculation. This calculator is a useful tool for performing quick calculations and is a great exercise for practicing user input and mathematical expression evaluation.</p>
