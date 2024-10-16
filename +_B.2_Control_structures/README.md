<p><strong>Chapter 2: B.2 Control Structures</strong></p>

<p>Control structures are a fundamental aspect of programming that allow developers to control the flow of their code. They enable the creation of complex logic, decision-making, and repetition, making it possible to write efficient and effective programs. In this chapter, we will delve into the world of control structures, exploring the different types, their syntax, and practical examples.</p>

<p><strong>2.1 Conditional Statements</strong></p>

<p>Conditional statements are used to execute different blocks of code based on a specific condition or set of conditions. They are essential in programming, as they allow developers to make decisions and take actions accordingly.</p>

<h3>If-Else Statement</h3>

<p>The if-else statement is one of the most commonly used conditional statements. It consists of a condition and two blocks of code: one for when the condition is true and another for when the condition is false.</p>

<p><code>c
if (condition) {
    // code to execute when condition is true
} else {
    // code to execute when condition is false
}
</code></p>

<p>Example:</p>

<p><code>c
int x = 5;
if (x &gt; 10) {
    printf("x is greater than 10\n");
} else {
    printf("x is less than or equal to 10\n");
}
</code></p>

<h3>If-Else-If Statement</h3>

<p>The if-else-if statement is used when there are multiple conditions to check. It allows developers to check multiple conditions and execute different blocks of code accordingly.</p>

<p><code>c
if (condition1) {
    // code to execute when condition1 is true
} else if (condition2) {
    // code to execute when condition2 is true
} else {
    // code to execute when both conditions are false
}
</code></p>

<p>Example:</p>

<p><code>c
int x = 5;
if (x &gt; 10) {
    printf("x is greater than 10\n");
} else if (x == 5) {
    printf("x is equal to 5\n");
} else {
    printf("x is less than 5\n");
}
</code></p>

<p><strong>2.2 Loops</strong></p>

<p>Loops are used to execute a block of code repeatedly for a specified number of times or until a certain condition is met. They are essential in programming, as they allow developers to perform repetitive tasks efficiently.</p>

<h3>For Loop</h3>

<p>The for loop is used to execute a block of code repeatedly for a specified number of times. It consists of three parts: initialization, condition, and increment.</p>

<p><code>c
for (initialization; condition; increment) {
    // code to execute
}
</code></p>

<p>Example:</p>

<p><code>c
for (int i = 0; i &lt; 5; i++) {
    printf("Hello, World!\n");
}
</code></p>

<h3>While Loop</h3>

<p>The while loop is used to execute a block of code repeatedly while a certain condition is true. It consists of a condition and a block of code.</p>

<p><code>c
while (condition) {
    // code to execute
}
</code></p>

<p>Example:</p>

<p><code>c
int i = 0;
while (i &lt; 5) {
    printf("Hello, World!\n");
    i++;
}
</code></p>

<h3>Do-While Loop</h3>

<p>The do-while loop is used to execute a block of code repeatedly while a certain condition is true. It consists of a block of code and a condition.</p>

<p><code>c
do {
    // code to execute
} while (condition);
</code></p>

<p>Example:</p>

<p><code>c
int i = 0;
do {
    printf("Hello, World!\n");
    i++;
} while (i &lt; 5);
</code></p>

<p><strong>2.3 Switch Statement</strong></p>

<p>The switch statement is used to execute different blocks of code based on the value of a variable. It is similar to a series of if-else statements, but more concise and efficient.</p>

<p><code>c
switch (expression) {
    case value1:
        // code to execute when expression is equal to value1
        break;
    case value2:
        // code to execute when expression is equal to value2
        break;
    default:
        // code to execute when expression does not match any value
}
</code></p>

<p>Example:</p>

<p><code>c
int day = 3;
switch (day) {
    case 1:
        printf("Monday\n");
        break;
    case 2:
        printf("Tuesday\n");
        break;
    case 3:
        printf("Wednesday\n");
        break;
    default:
        printf("Invalid day\n");
}
</code></p>

<p>In conclusion, control structures are a fundamental aspect of programming that allow developers to control the flow of their code. They enable the creation of complex logic, decision-making, and repetition, making it possible to write efficient and effective programs. By mastering control structures, developers can write more robust, scalable, and maintainable code.</p>
