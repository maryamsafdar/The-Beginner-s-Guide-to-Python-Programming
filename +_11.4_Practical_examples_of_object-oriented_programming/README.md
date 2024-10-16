<p><strong>Chapter 11: Practical Examples of Object-Oriented Programming</strong></p>

<p>In the previous chapters, we have discussed the fundamental concepts of object-oriented programming (OOP) such as classes, objects, inheritance, polymorphism, encapsulation, and abstraction. In this chapter, we will put these concepts into practice by providing 11 practical examples of OOP.</p>

<p><strong>11.1 Example 1: Bank Account System</strong></p>

<p>In this example, we will create a simple bank account system using OOP concepts. We will create a <code>BankAccount</code> class with attributes such as account number, account holder's name, and balance. We will also create methods to deposit and withdraw money from the account.</p>

<p>```python
class BankAccount:
    def <strong>init</strong>(self, account<em>number, account</em>holder, balance=0):
        self.account<em>number = account</em>number
        self.account<em>holder = account</em>holder
        self.balance = balance</p>

<pre><code>def deposit(self, amount):
    self.balance += amount
    print(f"Deposited ${amount} into account {self.account_number}")

def withdraw(self, amount):
    if amount &gt; self.balance:
        print("Insufficient balance")
    else:
        self.balance -= amount
        print(f"Withdrew ${amount} from account {self.account_number}")
</code></pre>

<h1>Create a bank account object</h1>

<p>account = BankAccount("123456789", "John Doe", 1000)
account.deposit(500)
account.withdraw(200)
```</p>

<p><strong>11.2 Example 2: Shape Classes</strong></p>

<p>In this example, we will create a hierarchy of shape classes using inheritance. We will create a <code>Shape</code> class with attributes such as color and area. We will then create subclasses <code>Circle</code>, <code>Rectangle</code>, and <code>Triangle</code> that inherit from the <code>Shape</code> class.</p>

<p>```python
class Shape:
    def <strong>init</strong>(self, color):
        self.color = color</p>

<pre><code>def area(self):
    pass
</code></pre>

<p>class Circle(Shape):
    def <strong>init</strong>(self, color, radius):
        super().<strong>init</strong>(color)
        self.radius = radius</p>

<pre><code>def area(self):
    return 3.14 * self.radius ** 2
</code></pre>

<p>class Rectangle(Shape):
    def <strong>init</strong>(self, color, width, height):
        super().<strong>init</strong>(color)
        self.width = width
        self.height = height</p>

<pre><code>def area(self):
    return self.width * self.height
</code></pre>

<p>class Triangle(Shape):
    def <strong>init</strong>(self, color, base, height):
        super().<strong>init</strong>(color)
        self.base = base
        self.height = height</p>

<pre><code>def area(self):
    return 0.5 * self.base * self.height
</code></pre>

<h1>Create shape objects</h1>

<p>circle = Circle("red", 5)
rectangle = Rectangle("blue", 4, 6)
triangle = Triangle("green", 3, 7)</p>

<p>print(f"Circle area: {circle.area()}")
print(f"Rectangle area: {rectangle.area()}")
print(f"Triangle area: {triangle.area()}")
```</p>

<p><strong>11.3 Example 3: Employee Hierarchy</strong></p>

<p>In this example, we will create a hierarchy of employee classes using inheritance. We will create a <code>Employee</code> class with attributes such as name, age, and salary. We will then create subclasses <code>Manager</code> and <code>Developer</code> that inherit from the <code>Employee</code> class.</p>

<p>```python
class Employee:
    def <strong>init</strong>(self, name, age, salary):
        self.name = name
        self.age = age
        self.salary = salary</p>

<pre><code>def display_details(self):
    print(f"Name: {self.name}")
    print(f"Age: {self.age}")
    print(f"Salary: ${self.salary}")
</code></pre>

<p>class Manager(Employee):
    def <strong>init</strong>(self, name, age, salary, department):
        super().<strong>init</strong>(name, age, salary)
        self.department = department</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Department: {self.department}")
</code></pre>

<p>class Developer(Employee):
    def <strong>init</strong>(self, name, age, salary, programming<em>languages):
        super().<strong>init</strong>(name, age, salary)
        self.programming</em>languages = programming_languages</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Programming languages: {self.programming_languages}")
</code></pre>

<h1>Create employee objects</h1>

<p>manager = Manager("John Doe", 30, 50000, "Marketing")
developer = Developer("Jane Doe", 25, 40000, ["Python", "Java"])</p>

<p>manager.display<em>details()
print()
developer.display</em>details()
```</p>

<p><strong>11.4 Example 4: University System</strong></p>

<p>In this example, we will create a university system using OOP concepts. We will create a <code>University</code> class with attributes such as name and location. We will then create subclasses <code>Department</code> and <code>Course</code> that inherit from the <code>University</code> class.</p>

<p>```python
class University:
    def <strong>init</strong>(self, name, location):
        self.name = name
        self.location = location</p>

<pre><code>def display_details(self):
    print(f"Name: {self.name}")
    print(f"Location: {self.location}")
</code></pre>

<p>class Department(University):
    def <strong>init</strong>(self, name, location, courses):
        super().<strong>init</strong>(name, location)
        self.courses = courses</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Courses: {self.courses}")
</code></pre>

<p>class Course(University):
    def <strong>init</strong>(self, name, location, credits):
        super().<strong>init</strong>(name, location)
        self.credits = credits</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Credits: {self.credits}")
</code></pre>

<h1>Create university objects</h1>

<p>university = University("ABC University", "New York")
department = Department("Computer Science", "New York", ["Algorithms", "Data Structures"])
course = Course("Algorithms", "New York", 3)</p>

<p>university.display<em>details()
print()
department.display</em>details()
print()
course.display_details()
```</p>

<p><strong>11.5 Example 5: Bank Transaction System</strong></p>

<p>In this example, we will create a bank transaction system using OOP concepts. We will create a <code>BankTransaction</code> class with attributes such as transaction type and amount. We will then create subclasses <code>Deposit</code> and <code>Withdrawal</code> that inherit from the <code>BankTransaction</code> class.</p>

<p>```python
class BankTransaction:
    def <strong>init</strong>(self, transaction<em>type, amount):
        self.transaction</em>type = transaction_type
        self.amount = amount</p>

<pre><code>def display_details(self):
    print(f"Transaction type: {self.transaction_type}")
    print(f"Amount: ${self.amount}")
</code></pre>

<p>class Deposit(BankTransaction):
    def <strong>init</strong>(self, amount):
        super().<strong>init</strong>("Deposit", amount)</p>

<pre><code>def display_details(self):
    super().display_details()
    print("Deposit successful")
</code></pre>

<p>class Withdrawal(BankTransaction):
    def <strong>init</strong>(self, amount):
        super().<strong>init</strong>("Withdrawal", amount)</p>

<pre><code>def display_details(self):
    super().display_details()
    print("Withdrawal successful")
</code></pre>

<h1>Create bank transaction objects</h1>

<p>deposit = Deposit(500)
withdrawal = Withdrawal(200)</p>

<p>deposit.display<em>details()
print()
withdrawal.display</em>details()
```</p>

<p><strong>11.6 Example 6: Hotel Reservation System</strong></p>

<p>In this example, we will create a hotel reservation system using OOP concepts. We will create a <code>Hotel</code> class with attributes such as name and location. We will then create subclasses <code>Room</code> and <code>Reservation</code> that inherit from the <code>Hotel</code> class.</p>

<p>```python
class Hotel:
    def <strong>init</strong>(self, name, location):
        self.name = name
        self.location = location</p>

<pre><code>def display_details(self):
    print(f"Name: {self.name}")
    print(f"Location: {self.location}")
</code></pre>

<p>class Room(Hotel):
    def <strong>init</strong>(self, name, location, room<em>number):
        super().<strong>init</strong>(name, location)
        self.room</em>number = room_number</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Room number: {self.room_number}")
</code></pre>

<p>class Reservation(Hotel):
    def <strong>init</strong>(self, name, location, room<em>number, check</em>in<em>date, check</em>out<em>date):
        super().<strong>init</strong>(name, location)
        self.room</em>number = room<em>number
        self.check</em>in<em>date = check</em>in<em>date
        self.check</em>out<em>date = check</em>out_date</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Room number: {self.room_number}")
    print(f"Check-in date: {self.check_in_date}")
    print(f"Check-out date: {self.check_out_date}")
</code></pre>

<h1>Create hotel objects</h1>

<p>hotel = Hotel("ABC Hotel", "New York")
room = Room("ABC Hotel", "New York", 101)
reservation = Reservation("ABC Hotel", "New York", 101, "2022-01-01", "2022-01-05")</p>

<p>hotel.display<em>details()
print()
room.display</em>details()
print()
reservation.display_details()
```</p>

<p><strong>11.7 Example 7: Library System</strong></p>

<p>In this example, we will create a library system using OOP concepts. We will create a <code>Library</code> class with attributes such as name and location. We will then create subclasses <code>Book</code> and <code>Member</code> that inherit from the <code>Library</code> class.</p>

<p>```python
class Library:
    def <strong>init</strong>(self, name, location):
        self.name = name
        self.location = location</p>

<pre><code>def display_details(self):
    print(f"Name: {self.name}")
    print(f"Location: {self.location}")
</code></pre>

<p>class Book(Library):
    def <strong>init</strong>(self, name, location, author, publication<em>date):
        super().<strong>init</strong>(name, location)
        self.author = author
        self.publication</em>date = publication_date</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Author: {self.author}")
    print(f"Publication date: {self.publication_date}")
</code></pre>

<p>class Member(Library):
    def <strong>init</strong>(self, name, location, membership<em>number):
        super().<strong>init</strong>(name, location)
        self.membership</em>number = membership_number</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Membership number: {self.membership_number}")
</code></pre>

<h1>Create library objects</h1>

<p>library = Library("ABC Library", "New York")
book = Book("ABC Library", "New York", "John Doe", "2020-01-01")
member = Member("ABC Library", "New York", "123456")</p>

<p>library.display<em>details()
print()
book.display</em>details()
print()
member.display_details()
```</p>

<p><strong>11.8 Example 8: Weather Forecast System</strong></p>

<p>In this example, we will create a weather forecast system using OOP concepts. We will create a <code>WeatherForecast</code> class with attributes such as location and temperature. We will then create subclasses <code>Sunny</code> and <code>Rainy</code> that inherit from the <code>WeatherForecast</code> class.</p>

<p>```python
class WeatherForecast:
    def <strong>init</strong>(self, location, temperature):
        self.location = location
        self.temperature = temperature</p>

<pre><code>def display_details(self):
    print(f"Location: {self.location}")
    print(f"Temperature: {self.temperature}")
</code></pre>

<p>class Sunny(WeatherForecast):
    def <strong>init</strong>(self, location, temperature):
        super().<strong>init</strong>(location, temperature)
        self.sunshine_hours = 8</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Sunshine hours: {self.sunshine_hours}")
</code></pre>

<p>class Rainy(WeatherForecast):
    def <strong>init</strong>(self, location, temperature):
        super().<strong>init</strong>(location, temperature)
        self.rainfall_inches = 2</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Rainfall inches: {self.rainfall_inches}")
</code></pre>

<h1>Create weather forecast objects</h1>

<p>forecast = WeatherForecast("New York", 75)
sunny = Sunny("New York", 75)
rainy = Rainy("New York", 75)</p>

<p>forecast.display<em>details()
print()
sunny.display</em>details()
print()
rainy.display_details()
```</p>

<p><strong>11.9 Example 9: Online Shopping System</strong></p>

<p>In this example, we will create an online shopping system using OOP concepts. We will create a <code>Product</code> class with attributes such as name and price. We will then create subclasses <code>Electronics</code> and <code>Fashion</code> that inherit from the <code>Product</code> class.</p>

<p>```python
class Product:
    def <strong>init</strong>(self, name, price):
        self.name = name
        self.price = price</p>

<pre><code>def display_details(self):
    print(f"Name: {self.name}")
    print(f"Price: ${self.price}")
</code></pre>

<p>class Electronics(Product):
    def <strong>init</strong>(self, name, price, brand):
        super().<strong>init</strong>(name, price)
        self.brand = brand</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Brand: {self.brand}")
</code></pre>

<p>class Fashion(Product):
    def <strong>init</strong>(self, name, price, size):
        super().<strong>init</strong>(name, price)
        self.size = size</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Size: {self.size}")
</code></pre>

<h1>Create product objects</h1>

<p>product = Product("Laptop", 1000)
electronics = Electronics("Laptop", 1000, "Dell")
fashion = Fashion("Shirt", 20, "Large")</p>

<p>product.display<em>details()
print()
electronics.display</em>details()
print()
fashion.display_details()
```</p>

<p><strong>11.10 Example 10: Restaurant System</strong></p>

<p>In this example, we will create a restaurant system using OOP concepts. We will create a <code>Restaurant</code> class with attributes such as name and location. We will then create subclasses <code>Menu</code> and <code>Order</code> that inherit from the <code>Restaurant</code> class.</p>

<p>```python
class Restaurant:
    def <strong>init</strong>(self, name, location):
        self.name = name
        self.location = location</p>

<pre><code>def display_details(self):
    print(f"Name: {self.name}")
    print(f"Location: {self.location}")
</code></pre>

<p>class Menu(Restaurant):
    def <strong>init</strong>(self, name, location, dishes):
        super().<strong>init</strong>(name, location)
        self.dishes = dishes</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Dishes: {self.dishes}")
</code></pre>

<p>class Order(Restaurant):
    def <strong>init</strong>(self, name, location, order<em>number):
        super().<strong>init</strong>(name, location)
        self.order</em>number = order_number</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Order number: {self.order_number}")
</code></pre>

<h1>Create restaurant objects</h1>

<p>restaurant = Restaurant("ABC Restaurant", "New York")
menu = Menu("ABC Restaurant", "New York", ["Pizza", "Burger"])
order = Order("ABC Restaurant", "New York", 12345)</p>

<p>restaurant.display<em>details()
print()
menu.display</em>details()
print()
order.display_details()
```</p>

<p><strong>11.11 Example 11: Game Development System</strong></p>

<p>In this example, we will create a game development system using OOP concepts. We will create a <code>Game</code> class with attributes such as name and genre. We will then create subclasses <code>Platformer</code> and <code>Puzzle</code> that inherit from the <code>Game</code> class.</p>

<p>```python
class Game:
    def <strong>init</strong>(self, name, genre):
        self.name = name
        self.genre = genre</p>

<pre><code>def display_details(self):
    print(f"Name: {self.name}")
    print(f"Genre: {self.genre}")
</code></pre>

<p>class Platformer(Game):
    def <strong>init</strong>(self, name, genre, difficulty):
        super().<strong>init</strong>(name, genre)
        self.difficulty = difficulty</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Difficulty: {self.difficulty}")
</code></pre>

<p>class Puzzle(Game):
    def <strong>init</strong>(self, name, genre, level<em>count):
        super().<strong>init</strong>(name, genre)
        self.level</em>count = level_count</p>

<pre><code>def display_details(self):
    super().display_details()
    print(f"Level count: {self.level_count}")
</code></pre>

<h1>Create game objects</h1>

<p>game = Game("ABC Game", "Action")
platformer = Platformer("ABC Game", "Action", "Hard")
puzzle = Puzzle("ABC Game", "Puzzle", 10)</p>

<p>game.display<em>details()
print()
platformer.display</em>details()
print()
puzzle.display_details()
```</p>

<p>In this chapter, we have provided 11 practical examples of object-oriented programming. These examples demonstrate how OOP concepts such as classes, objects, inheritance, polymorphism, encapsulation, and abstraction can be applied to real-world scenarios. By studying these examples, readers can gain a deeper understanding of OOP principles and how to apply them in their own programming projects.</p>
