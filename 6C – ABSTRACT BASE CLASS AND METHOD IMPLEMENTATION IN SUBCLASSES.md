# Experiment No: 6c – Abstract Base Class and Method Implementation in Subclasses

## AIM  
To define an abstract base class `Polygon` with an abstract method `sides()` and implement this method in various subclasses.

---

## ALGORITHM  
1. Import `ABC` and `abstractmethod` from `abc` module.
2. Define the abstract base class `Polygon` using `ABC`.
3. Define the abstract method `sides()` inside `Polygon`.
4. Create subclasses like `Triangle`, `Square`, `Pentagon`, and `Hexagon` that inherit from `Polygon`.
5. Override and implement the `sides()` method in each subclass.
6. Create objects of each subclass.
7. Call the `sides()` method for each object to demonstrate polymorphism.

---

## 🧾 PROGRAM

```python
from abc import ABC, abstractmethod

class Polygon(ABC):
    @abstractmethod
    def sides(self):
        pass

class Triangle(Polygon):
    def sides(self):
        print("Triangle has 3 sides")

class Square(Polygon):
    def sides(self):
        print("I have 4 sides")

class Pentagon(Polygon):
    def sides(self):
        print("Pentagon has 5 sides")

class Hexagon(Polygon):
    def sides(self):
        print("Hexagon has 6 sides")

# Creating objects and invoking sides method
t = Triangle()
t.sides()

s = Square()
s.sides()

p = Pentagon()
p.sides()

h = Hexagon()
h.sides()

```

### OUTPUT


### RESULT
