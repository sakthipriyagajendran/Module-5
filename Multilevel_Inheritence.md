# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
# Base class
class Person:
    
    def __init__(self):
        self.name = input("Enter name: ")

# Derived class 1
class Age(Person):
    
    def __init__(self):
        super().__init__()
        self.age = int(input("Enter age: "))

# Derived class 2
class Location(Age):
    
    def __init__(self):
        super().__init__()
        self.location = input("Enter location: ")
    
    def display(self):
        print("\n--- Person Details ---")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Location:", self.location)

# Creating object
p = Location()

# Displaying details
p.display()

## Sample Output
<img width="384" height="401" alt="image" src="https://github.com/user-attachments/assets/2a5c8cb0-4518-42d9-80a2-c0b33bd584d6" />


**RESULT:**

Thus,the program was implemented and executed successfully,and the required output was obtained.
