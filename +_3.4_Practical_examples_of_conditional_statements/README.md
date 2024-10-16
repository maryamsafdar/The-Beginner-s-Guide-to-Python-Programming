<p><strong>Chapter 7: Practical Examples of Conditional Statements</strong></p>

<p>In the previous chapter, we discussed the basics of conditional statements in programming. We learned about the different types of conditional statements, including if-else statements, switch statements, and nested conditional statements. In this chapter, we will explore practical examples of conditional statements to help you understand how they are used in real-world programming scenarios.</p>

<p><strong>7.1 Example 1: Checking User Input</strong></p>

<p>Let's consider a simple example where we want to check if a user has entered a valid age. We can use an if-else statement to achieve this.</p>

<p>```python</p>

<h1>Get user input</h1>

<p>age = int(input("Enter your age: "))</p>

<h1>Check if the age is valid</h1>

<p>if age &gt;= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
```</p>

<p>In this example, we first get the user's age using the input() function. We then check if the age is greater than or equal to 18 using an if-else statement. If the age is valid, we print a message indicating that the user is an adult. Otherwise, we print a message indicating that the user is a minor.</p>

<p><strong>7.2 Example 2: Handling Multiple Conditions</strong></p>

<p>Let's consider a scenario where we want to check if a user has entered a valid grade. We can use an if-else statement with multiple conditions to achieve this.</p>

<p>```python</p>

<h1>Get user input</h1>

<p>grade = input("Enter your grade (A, B, C, D, F): ")</p>

<h1>Check if the grade is valid</h1>

<p>if grade.upper() == "A":
    print("You got an A.")
elif grade.upper() == "B":
    print("You got a B.")
elif grade.upper() == "C":
    print("You got a C.")
elif grade.upper() == "D":
    print("You got a D.")
elif grade.upper() == "F":
    print("You got an F.")
else:
    print("Invalid grade.")
```</p>

<p>In this example, we first get the user's grade using the input() function. We then check if the grade is valid using an if-else statement with multiple conditions. If the grade is valid, we print a message indicating the grade. Otherwise, we print a message indicating that the grade is invalid.</p>

<p><strong>7.3 Example 3: Using Switch Statements</strong></p>

<p>Let's consider a scenario where we want to check if a user has entered a valid day of the week. We can use a switch statement to achieve this.</p>

<p>```python</p>

<h1>Get user input</h1>

<p>day = input("Enter the day of the week (Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday): ")</p>

<h1>Check if the day is valid using a switch statement</h1>

<p>match day:
    case "Monday":
        print("Today is Monday.")
    case "Tuesday":
        print("Today is Tuesday.")
    case "Wednesday":
        print("Today is Wednesday.")
    case "Thursday":
        print("Today is Thursday.")
    case "Friday":
        print("Today is Friday.")
    case "Saturday":
        print("Today is Saturday.")
    case "Sunday":
        print("Today is Sunday.")
    case _:
        print("Invalid day.")
```</p>

<p>In this example, we first get the user's day of the week using the input() function. We then check if the day is valid using a switch statement. If the day is valid, we print a message indicating the day. Otherwise, we print a message indicating that the day is invalid.</p>

<p><strong>7.4 Example 4: Using Nested Conditional Statements</strong></p>

<p>Let's consider a scenario where we want to check if a user has entered a valid age and grade. We can use nested conditional statements to achieve this.</p>

<p>```python</p>

<h1>Get user input</h1>

<p>age = int(input("Enter your age: "))
grade = input("Enter your grade (A, B, C, D, F): ")</p>

<h1>Check if the age and grade are valid</h1>

<p>if age &gt;= 18:
    if grade.upper() == "A":
        print("You are an adult and got an A.")
    elif grade.upper() == "B":
        print("You are an adult and got a B.")
    elif grade.upper() == "C":
        print("You are an adult and got a C.")
    elif grade.upper() == "D":
        print("You are an adult and got a D.")
    elif grade.upper() == "F":
        print("You are an adult and got an F.")
    else:
        print("Invalid grade.")
else:
    if grade.upper() == "A":
        print("You are a minor and got an A.")
    elif grade.upper() == "B":
        print("You are a minor and got a B.")
    elif grade.upper() == "C":
        print("You are a minor and got a C.")
    elif grade.upper() == "D":
        print("You are a minor and got a D.")
    elif grade.upper() == "F":
        print("You are a minor and got an F.")
    else:
        print("Invalid grade.")
```</p>

<p>In this example, we first get the user's age and grade using the input() function. We then check if the age and grade are valid using nested conditional statements. If the age and grade are valid, we print a message indicating the age and grade. Otherwise, we print a message indicating that the age or grade is invalid.</p>

<p>In conclusion, conditional statements are a fundamental concept in programming that allow us to make decisions based on certain conditions. In this chapter, we explored practical examples of conditional statements, including if-else statements, switch statements, and nested conditional statements. By understanding how to use these statements effectively, you can write more efficient and effective code.</p>
