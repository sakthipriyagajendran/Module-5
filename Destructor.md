# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program
class Student:
    
    # Constructor
    def __init__(self, name):
        self.name = name
        print("Student", self.name, "created.")
    
    # Method
    def display(self):
        print("Hello,", self.name)
    
    # Destructor
    def __del__(self):
        print("Student", self.name, "destroyed.")

# Creating object
s1 = Student("Shakthi")

# Calling method
s1.display()

# Deleting object
del s1

## 🧪 Output
<img width="370" height="239" alt="image" src="https://github.com/user-attachments/assets/b1f03952-fde8-49d0-be28-3a38d6128341" />

## Result
Thus,the program was implemented and executed successfully,and the required output was obtained.
