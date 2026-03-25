# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
# Parent class 1
class Add:
    
    def get_values(self):
        self.a = float(input("Enter first number: "))
        self.b = float(input("Enter second number: "))
    
    def addition(self):
        print("Addition:", self.a + self.b)


# Parent class 2
class Subtract:
    
    def subtraction(self):
        print("Subtraction:", self.a - self.b)


# Parent class 3
class Division:
    
    def division(self):
        if self.b != 0:
            print("Division:", self.a / self.b)
        else:
            print("Division not possible (cannot divide by zero)")


# Child class (Multiple Inheritance)
class Calculator(Add, Subtract, Division):
    
    def display(self):
        self.get_values()
        print("\n--- Results ---")
        self.addition()
        self.subtraction()
        self.division()


# Creating object
calc = Calculator()

# Calling method
calc.display()
## Output Example

<img width="379" height="362" alt="image" src="https://github.com/user-attachments/assets/03061540-ac6c-4b84-a627-194913e36b5a" />

**RESULT:**
Thus,the program was implemented and executed successfully,and the required output was obtained.
