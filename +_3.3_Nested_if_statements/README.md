<p><strong>Chapter 3.3: Nested If Statements</strong></p>

<p>In the previous chapters, we have explored the basics of conditional statements in programming. We have learned how to use if statements to make decisions based on conditions and how to use else statements to provide alternative actions when conditions are not met. However, in many real-world scenarios, we need to make decisions based on multiple conditions. This is where nested if statements come into play.</p>

<p><strong>What are Nested If Statements?</strong></p>

<p>Nested if statements are a type of conditional statement where an if statement is placed inside another if statement. This allows us to make decisions based on multiple conditions. The inner if statement is executed only when the outer if statement is true.</p>

<p><strong>Why Use Nested If Statements?</strong></p>

<p>Nested if statements are useful when we need to make decisions based on multiple conditions. For example, in a banking system, we might need to check if a customer is eligible for a loan based on their credit score, income, and employment history. We can use nested if statements to check each condition and provide a decision based on the results.</p>

<p><strong>Basic Syntax of Nested If Statements</strong></p>

<p>The basic syntax of nested if statements is as follows:
<code>python
if condition1:
    if condition2:
        # code to execute when both conditions are true
</code>
In this syntax, <code>condition1</code> is the outer condition, and <code>condition2</code> is the inner condition. The code inside the inner if statement is executed only when both conditions are true.</p>

<p><strong>Example of Nested If Statements</strong></p>

<p>Let's consider an example of a banking system where we need to check if a customer is eligible for a loan based on their credit score, income, and employment history. We can use nested if statements to check each condition and provide a decision based on the results.
```python
credit<em>score = 700
income = 50000
employment</em>history = 5</p>

<p>if credit<em>score &gt;= 700:
    if income &gt;= 50000:
        if employment</em>history &gt;= 5:
            print("You are eligible for a loan.")
        else:
            print("You are not eligible for a loan due to insufficient employment history.")
    else:
        print("You are not eligible for a loan due to insufficient income.")
else:
    print("You are not eligible for a loan due to insufficient credit score.")
```
In this example, we first check if the credit score is 700 or higher. If it is, we then check if the income is 50000 or higher. If it is, we then check if the employment history is 5 or higher. If all conditions are true, we print a message indicating that the customer is eligible for a loan.</p>

<p><strong>Best Practices for Using Nested If Statements</strong></p>

<p>Here are some best practices to keep in mind when using nested if statements:</p>

<ul>
<li>Use clear and concise variable names to make the code easier to read.</li>
<li>Use comments to explain the purpose of each condition and the code inside the if statement.</li>
<li>Use indentation to make the code easier to read.</li>
<li>Avoid using too many nested if statements, as they can make the code difficult to read and maintain.</li>
</ul>

<p><strong>Conclusion</strong></p>

<p>Nested if statements are a powerful tool for making decisions based on multiple conditions. By using nested if statements, we can create complex decision-making logic that is easy to read and maintain. Remember to use clear and concise variable names, comments, and indentation to make the code easier to read. With practice and experience, you will become proficient in using nested if statements to create complex decision-making logic.</p>
