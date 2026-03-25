# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
# Base class
class Details:
    
    def __init__(self):
        self.name = input("Enter name: ")
        self.age = int(input("Enter age: "))
    
    def display_details(self):
        print("Name:", self.name)
        print("Age:", self.age)


# Derived class 1
class Employee(Details):
    
    def __init__(self):
        super().__init__()
        self.emp_id = input("Enter Employee ID: ")
        self.salary = float(input("Enter Salary: "))
    
    def display_employee(self):
        print("\n--- Employee Details ---")
        self.display_details()
        print("Employee ID:", self.emp_id)
        print("Salary:", self.salary)


# Derived class 2
class Patient(Details):
    
    def __init__(self):
        super().__init__()
        self.patient_id = input("Enter Patient ID: ")
        self.disease = input("Enter Disease: ")
    
    def display_patient(self):
        print("\n--- Patient Details ---")
        self.display_details()
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)


# Creating objects
print("Enter Employee Information")
emp = Employee()
emp.display_employee()

print("\nEnter Patient Information")
pat = Patient()
pat.display_patient()
## Sample Output
<img width="368" height="779" alt="image" src="https://github.com/user-attachments/assets/bf10fc2c-c6b3-4e5c-9f16-a527bd31fa22" />


**RESULT:**

Thus,the program was implemented and executed successfully,and the required output was obtained.
