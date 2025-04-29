# Experiment No: 6e – Counter Class with Increment, Reset and Value Methods

## AIM:
To write a Python program to create a `Counter` class with an attribute `current` and implement the methods `increment()`, `value()`, and `reset()`.

---

## ALGORITHM:
1. Define a class named `Counter`.
2. Inside the class, initialize an attribute `current` to 0 using a constructor.
3. Define a method `increment()` to increase `current` by 1.
4. Define a method `value()` to return the current value of `current`.
5. Define a method `reset()` to reset `current` to 0.
6. Create an instance of the class.
7. Call the `increment()` method three times.
8. Print the current value using the `value()` method.

---

## PROGRAM:
```python
class Counter:
    def __init__(self):
        self.current = 0

    def increment(self):
        self.current += 1

    def value(self):
        return self.current

    def reset(self):
        self.current = 0

counter = Counter()
c = 0
while c < 3:
    counter.increment()
    c += 1
print(counter.value())

```

### OUTPUT


### RESULT
