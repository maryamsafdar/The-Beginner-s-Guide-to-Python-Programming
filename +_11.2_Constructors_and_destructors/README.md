<p><strong>Chapter 11.2: Constructors and Destructors</strong></p>

<p>In this chapter, we will delve into the world of constructors and destructors in C++. These special member functions play a crucial role in the initialization and cleanup of objects, and understanding their usage is essential for writing robust and efficient C++ code.</p>

<p><strong>What are Constructors?</strong></p>

<p>A constructor is a special member function of a class that is used to initialize objects when they are created. It has the same name as the class and does not have a return type, not even <code>void</code>. Constructors are called when an object is created using the <code>new</code> keyword or when an object is passed by value to a function.</p>

<p><strong>Types of Constructors</strong></p>

<p>There are two types of constructors in C++:</p>

<ol>
<li><strong>Default Constructor</strong>: A default constructor is a constructor that takes no arguments. It is used to initialize objects when no specific values are provided.</li>
<li><strong>Parameterized Constructor</strong>: A parameterized constructor is a constructor that takes one or more arguments. It is used to initialize objects with specific values.</li>
</ol>

<p><strong>Example of a Default Constructor</strong></p>

<p>```cpp
class Person {
public:
    Person() {
        name = "John";
        age = 30;
    }</p>

<pre><code>void display() {
    cout &lt;&lt; "Name: " &lt;&lt; name &lt;&lt; endl;
    cout &lt;&lt; "Age: " &lt;&lt; age &lt;&lt; endl;
}
</code></pre>

<p>private:
    string name;
    int age;
};</p>

<p>int main() {
    Person p;
    p.display();
    return 0;
}
```</p>

<p>In this example, the <code>Person</code> class has a default constructor that initializes the <code>name</code> and <code>age</code> members with default values.</p>

<p><strong>Example of a Parameterized Constructor</strong></p>

<p>```cpp
class Person {
public:
    Person(string name, int age) {
        this->name = name;
        this->age = age;
    }</p>

<pre><code>void display() {
    cout &lt;&lt; "Name: " &lt;&lt; name &lt;&lt; endl;
    cout &lt;&lt; "Age: " &lt;&lt; age &lt;&lt; endl;
}
</code></pre>

<p>private:
    string name;
    int age;
};</p>

<p>int main() {
    Person p("Jane", 25);
    p.display();
    return 0;
}
```</p>

<p>In this example, the <code>Person</code> class has a parameterized constructor that takes two arguments, <code>name</code> and <code>age</code>, and initializes the corresponding members.</p>

<p><strong>What are Destructors?</strong></p>

<p>A destructor is a special member function of a class that is used to clean up resources when an object is destroyed. It has the same name as the class but with a tilde (~) prefix and does not have a return type, not even <code>void</code>. Destructors are called when an object is destroyed using the <code>delete</code> keyword or when an object goes out of scope.</p>

<p><strong>Example of a Destructor</strong></p>

<p>```cpp
class File {
public:
    File(string filename) {
        file = fopen(filename.c_str(), "r");
    }</p>

<pre><code>~File() {
    fclose(file);
}

void read() {
    // Read from file
}
</code></pre>

<p>private:
    FILE* file;
};</p>

<p>int main() {
    File f("example.txt");
    f.read();
    return 0;
}
```</p>

<p>In this example, the <code>File</code> class has a destructor that closes the file when the object is destroyed.</p>

<p><strong>Best Practices</strong></p>

<p>Here are some best practices to keep in mind when using constructors and destructors:</p>

<ul>
<li>Use constructors to initialize objects with default values or specific values.</li>
<li>Use destructors to clean up resources when objects are destroyed.</li>
<li>Avoid using <code>new</code> and <code>delete</code> in favor of smart pointers or containers.</li>
<li>Use the Rule of Five (or Rule of Zero) to ensure that your class has a consistent set of special member functions.</li>
</ul>

<p>By following these best practices and understanding the usage of constructors and destructors, you can write robust and efficient C++ code that is easy to maintain and debug.</p>

<p><strong>Conclusion</strong></p>

<p>In this chapter, we have covered the basics of constructors and destructors in C++. We have seen how to use constructors to initialize objects with default values or specific values and how to use destructors to clean up resources when objects are destroyed. We have also discussed best practices for using constructors and destructors, including the Rule of Five and the Rule of Zero. By mastering the concepts presented in this chapter, you will be well on your way to writing high-quality C++ code.</p>
