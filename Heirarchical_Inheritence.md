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
```
class Details:
    def getName(self):
        self.name = input("Enter Name: ")

    def getAge(self):
        self.age = int(input("Enter Age: "))


class Employee(Details):
    def getEmployeeDetails(self):
        self.getName()
        self.getAge()
        self.employee_id = input("Enter Employee ID: ")
        self.department = input("Enter Department: ")

        print("\nEmployee Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Employee ID:", self.employee_id)
        print("Department:", self.department)


class Patient(Details):
    def getPatientDetails(self):
        self.getName()
        self.getAge()
        self.patient_id = input("Enter Patient ID: ")
        self.disease = input("Enter Disease: ")

        print("\nPatient Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)


e = Employee()
e.getEmployeeDetails()

p = Patient()
p.getPatientDetails()
```

## Sample Output
<img width="654" height="712" alt="image" src="https://github.com/user-attachments/assets/148d1195-b0a9-4bf0-b503-ff7632557d3b" />

## Result:
Thus, the Python program to demonstrate Hierarchical Inheritance for Employee and Patient details was executed successfully.
