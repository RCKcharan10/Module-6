# Experiment No: 6a – Demonstrate Polymorphism Using Classes Cat and Dog

## AIM  
To write a Python program that demonstrates polymorphism using two classes, `Cat` and `Dog`, which share similar method names and structures.

---

## ALGORITHM  
1. Create a class `Cat` with:
   - Constructor `__init__` to set name and age.
   - Method `make_sound()` to print `'Meow'`.
   - Method `info()` to display cat details.
2. Create a class `Dog` with:
   - Constructor `__init__` to set name and age.
   - Method `make_sound()` to print `'Bark'`.
   - Method `info()` to display dog details.
3. Accept name and age for both `Cat` and `Dog` from the user.
4. Create objects of both classes and pack them into a tuple.
5. Iterate through the tuple and use the `animal` variable to call methods, demonstrating polymorphism.

---

## 🧾 PROGRAM

```python
class Cat:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    def make_sound(self):
        print('Meow')
    def info(self):
        print(f'I am a cat. My name is {self.name}. I am {self.age} years old.')

class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    def make_sound(self):
        print('Bark')
    def info(self):
        print(f'I am a dog. My name is {self.name}. I am {self.age} years old.')

s1 = input()
a1 = input()
s2 = input()
a2 = input()

cat1 = Cat(s1, a1)
dog1 = Dog(s2, a2)

for animal in (cat1, dog1):
    animal.make_sound()
    animal.info()
    animal.make_sound()

```

### OUTPUT
![image](https://github.com/user-attachments/assets/38cced9a-b7c0-44e4-a108-1996340be9b8)

### RESULT
Thus, the Python program demonstrating polymorphism using common method names in different classes has been executed successfully.
