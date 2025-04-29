# Experiment No: 6d – Class with Instance Variables and Methods

## AIM  
To create an `Employee` class with instance variables `name`, `salary`, and `project`, and implement behaviors using `work()` and `show()` methods.

---

## ALGORITHM  
1. Define a class named `Employee`.
2. Create a constructor `__init__()` to initialize name, salary, and project.
3. Define a method `show()` to print the name and salary.
4. Define another method `work()` to print which project the employee is working on.
5. Create an object of the `Employee` class and invoke both methods.

---

## 🧾 PROGRAM

```python
class Employee:
    # constructor
    def __init__(self, name, salary, project):
        # data members
        self.name = name
        self.salary = salary
        self.project = project

    # method to display employee's details
    def show(self):
        print("Name: ", self.name, 'Salary:', self.salary)

    # method to show what the employee is working on
    def work(self):
        print(self.name, 'is working on', self.project)

# creating an object of Employee class
emp = Employee("Jessa", 8000, 'NLP')
emp.show()
emp.work()

```

### OUTPUT
![image](https://github.com/user-attachments/assets/3f0f4923-6e67-47ba-8d87-767f0cafc7d8)

### RESULT
Thus, the Python program to demonstrate instance variables and methods in a class using the Employee class was successfully executed.
