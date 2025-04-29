# Experiment No: 6b – Operator Overloading for Adding Two Objects

## AIM  
To write a Python program to demonstrate operator overloading for adding two objects using the `+` operator.

---

## ALGORITHM  
1. Create a class `product` with an initializer `__init__` to set the value.
2. Overload the `+` operator using `__add__` method.
3. In the `__add__` method:
   - If both values are numeric, return their sum.
   - If both values are strings, concatenate them.
   - Otherwise, raise `TypeError`.
4. Take input from the user (numeric and string).
5. Create instances of the class.
6. Add the objects and display the result.

---

## 🧾 PROGRAM

```python
class product:
    def __init__(self, val):
        self.val = val

    def __add__(self, other):
        if isinstance(self.val, (int, float)) and isinstance(other.val, (int, float)):
            return product(self.val + other.val)
        elif isinstance(self.val, str) and isinstance(other.val, str):
            return product(self.val + other.val)
        else:
            raise TypeError("Unsupported operand types for +")

# Integer addition
a = int(input())
b = int(input())
p1 = product(a)
p2 = product(b)
res = p1 + p2
print("amount : " + str(res.val))

# String concatenation
c = input()
d = input()
p3 = product(c)
p4 = product(d)
res2 = p3 + p4
print("location:  " + res2.val)

```

### OUTPUT
![image](https://github.com/user-attachments/assets/2d8336e2-0de8-42d9-9624-ccd2b61dc02c)

### RESULT
Thus, the Python program for operator overloading using the + operator with numeric and string types has been executed successfully.
