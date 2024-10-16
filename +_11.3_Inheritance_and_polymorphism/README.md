<p><strong>Chapter 11: Inheritance and Polymorphism</strong></p>

<p>Inheritance and polymorphism are two fundamental concepts in object-oriented programming (OOP) that enable developers to create complex and reusable code. In this chapter, we will delve into the world of inheritance and polymorphism, exploring their definitions, benefits, and applications.</p>

<p><strong>11.1 Introduction to Inheritance</strong></p>

<p>Inheritance is a mechanism that allows one class to inherit the properties and behavior of another class. The class that inherits the properties and behavior is called the subclass or derived class, while the class being inherited from is called the superclass or base class. Inheritance enables code reuse, making it easier to create new classes that build upon existing ones.</p>

<p><strong>11.2 Types of Inheritance</strong></p>

<p>There are several types of inheritance, including:</p>

<ul>
<li><strong>Single Inheritance</strong>: A subclass inherits from a single superclass.</li>
<li><strong>Multiple Inheritance</strong>: A subclass inherits from multiple superclasses.</li>
<li><strong>Multilevel Inheritance</strong>: A subclass inherits from a superclass that itself inherits from another superclass.</li>
<li><strong>Hierarchical Inheritance</strong>: A superclass has multiple subclasses.</li>
<li><strong>Hybrid Inheritance</strong>: A combination of multiple inheritance types.</li>
</ul>

<p><strong>11.3 Inheritance in Programming</strong></p>

<p>In programming, inheritance is implemented using the <code>extends</code> keyword in languages like Java and C++, or the <code>class</code> keyword with a colon followed by the superclass name in languages like Python.</p>

<p>```java
// Java example
public class Animal {
    public void sound() {
        System.out.println("The animal makes a sound.");
    }
}</p>

<p>public class Dog extends Animal {
    public void sound() {
        System.out.println("The dog barks.");
    }
}
```</p>

<p>```python</p>

<h1>Python example</h1>

<p>class Animal:
    def sound(self):
        print("The animal makes a sound.")</p>

<p>class Dog(Animal):
    def sound(self):
        print("The dog barks.")
```</p>

<p><strong>11.4 Polymorphism</strong></p>

<p>Polymorphism is the ability of an object to take on multiple forms. This can be achieved through method overriding or method overloading.</p>

<ul>
<li><strong>Method Overriding</strong>: A subclass provides a different implementation of a method that is already defined in its superclass.</li>
<li><strong>Method Overloading</strong>: A class provides multiple methods with the same name but different parameters.</li>
</ul>

<p><strong>11.5 Types of Polymorphism</strong></p>

<p>There are two types of polymorphism:</p>

<ul>
<li><strong>Compile-time Polymorphism</strong>: The type of the object is determined at compile time.</li>
<li><strong>Runtime Polymorphism</strong>: The type of the object is determined at runtime.</li>
</ul>

<p><strong>11.6 Polymorphism in Programming</strong></p>

<p>In programming, polymorphism is implemented using method overriding and method overloading.</p>

<p>```java
// Java example
public class Animal {
    public void sound() {
        System.out.println("The animal makes a sound.");
    }
}</p>

<p>public class Dog extends Animal {
    @Override
    public void sound() {
        System.out.println("The dog barks.");
    }
}</p>

<p>public class Cat extends Animal {
    @Override
    public void sound() {
        System.out.println("The cat meows.");
    }
}
```</p>

<p>```python</p>

<h1>Python example</h1>

<p>class Animal:
    def sound(self):
        print("The animal makes a sound.")</p>

<p>class Dog(Animal):
    def sound(self):
        print("The dog barks.")</p>

<p>class Cat(Animal):
    def sound(self):
        print("The cat meows.")
```</p>

<p><strong>11.7 Benefits of Inheritance and Polymorphism</strong></p>

<p>Inheritance and polymorphism offer several benefits, including:</p>

<ul>
<li><strong>Code Reuse</strong>: Inheritance enables code reuse, making it easier to create new classes that build upon existing ones.</li>
<li><strong>Easier Maintenance</strong>: Inheritance and polymorphism make it easier to modify and extend existing code.</li>
<li><strong>Improved Flexibility</strong>: Inheritance and polymorphism enable developers to create more flexible and adaptable code.</li>
</ul>

<p><strong>11.8 Conclusion</strong></p>

<p>Inheritance and polymorphism are two fundamental concepts in object-oriented programming that enable developers to create complex and reusable code. By understanding the benefits and applications of inheritance and polymorphism, developers can write more efficient, maintainable, and flexible code.</p>

<p><strong>11.9 Exercises</strong></p>

<ol>
<li>Create a class hierarchy using inheritance, where a <code>Vehicle</code> class has a <code>Car</code> and <code>Truck</code> subclass.</li>
<li>Implement method overriding and method overloading in a class hierarchy.</li>
<li>Create a program that demonstrates the benefits of inheritance and polymorphism.</li>
</ol>

<p><strong>11.10 References</strong></p>

<ul>
<li>[1] "Object-Oriented Programming Concepts" by Microsoft</li>
<li>[2] "Inheritance and Polymorphism" by Oracle</li>
<li>[3] "Object-Oriented Programming" by Wikipedia</li>
</ul>
