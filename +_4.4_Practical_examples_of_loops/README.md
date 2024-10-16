<p><strong>Chapter 4.4: Practical Examples of Loops</strong></p>

<p>In the previous chapters, we have discussed the different types of loops available in programming languages, including for loops, while loops, and do-while loops. In this chapter, we will explore some practical examples of loops to help you understand their usage and implementation.</p>

<p><strong>Example 1: Printing Numbers from 1 to 10</strong></p>

<p>One of the simplest examples of a loop is printing numbers from 1 to 10. We can use a for loop to achieve this.</p>

<p>```python</p>

<h1>Example 1: Printing numbers from 1 to 10</h1>

<p>for i in range(1, 11):
    print(i)
```</p>

<p>In this example, we use the <code>range()</code> function to generate a sequence of numbers from 1 to 10. The <code>for</code> loop then iterates over this sequence and prints each number.</p>

<p><strong>Example 2: Calculating the Sum of Numbers</strong></p>

<p>Another example of a loop is calculating the sum of numbers. We can use a while loop to achieve this.</p>

<p>```python</p>

<h1>Example 2: Calculating the sum of numbers</h1>

<p>num = 1
total = 0
while num &lt;= 10:
    total += num
    num += 1
print("The sum of numbers from 1 to 10 is:", total)
```</p>

<p>In this example, we initialize a variable <code>num</code> to 1 and a variable <code>total</code> to 0. We then use a while loop to iterate from 1 to 10, adding each number to the <code>total</code> variable. Finally, we print the sum of numbers.</p>

<p><strong>Example 3: Printing the First 5 Letters of the Alphabet</strong></p>

<p>We can use a for loop to print the first 5 letters of the alphabet.</p>

<p>```python</p>

<h1>Example 3: Printing the first 5 letters of the alphabet</h1>

<p>for letter in "ABCDE":
    print(letter)
```</p>

<p>In this example, we use a for loop to iterate over the string "ABCDE". The loop then prints each letter of the string.</p>

<p><strong>Example 4: Finding the Largest Number in a List</strong></p>

<p>We can use a for loop to find the largest number in a list.</p>

<p>```python</p>

<h1>Example 4: Finding the largest number in a list</h1>

<p>numbers = [12, 45, 7, 23, 56, 89, 34]
max<em>num = numbers[0]
for num in numbers:
    if num &gt; max</em>num:
        max<em>num = num
print("The largest number in the list is:", max</em>num)
```</p>

<p>In this example, we initialize a variable <code>max_num</code> to the first number in the list. We then use a for loop to iterate over the list, updating the <code>max_num</code> variable if we find a larger number.</p>

<p><strong>Example 5: Simulating a Bank Account</strong></p>

<p>We can use a while loop to simulate a bank account.</p>

<p>```python</p>

<h1>Example 5: Simulating a bank account</h1>

<p>balance = 1000
while True:
    print("Current balance:", balance)
    action = input("Do you want to deposit (D), withdraw (W), or exit (E)? ")
    if action.upper() == "D":
        amount = float(input("Enter the amount to deposit: "))
        balance += amount
    elif action.upper() == "W":
        amount = float(input("Enter the amount to withdraw: "))
        if amount &lt;= balance:
            balance -= amount
        else:
            print("Insufficient balance!")
    elif action.upper() == "E":
        break
    else:
        print("Invalid action!")
```</p>

<p>In this example, we use a while loop to simulate a bank account. The loop continues until the user chooses to exit. The user can deposit or withdraw money, and the balance is updated accordingly.</p>

<p>These examples demonstrate the practical usage of loops in programming. By using loops, we can perform repetitive tasks efficiently and effectively.</p>
