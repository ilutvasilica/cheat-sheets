# 🐍 Python Cheat Sheet (Intermediate)

Quick reference for more advanced Python features 🚀

---

## 🔹 List Comprehensions
```python
# Generate a list of squares
squares = [x**2 for x in range(10)]

# Filter even numbers
evens = [x for x in range(10) if x % 2 == 0]

#Lambda
add = lambda a, b: a + b
print(add(5, 3))  # 8

#Map,filter
nums = [1, 2, 3, 4]

# Map → apply function
squares = list(map(lambda x: x**2, nums))

# Filter → keep only even
evens = list(filter(lambda x: x % 2 == 0, nums))

# Reduce → accumulate values
from functools import reduce
sum_all = reduce(lambda a, b: a + b, nums)

#OPP

class Dog:
    def __init__(self, name):
        self.name = name

    def bark(self):
        print(f"{self.name} says woof!")

dog = Dog("Rex")
dog.bark()  # Rex says woof!


#Inheritance

class Animal:
    def speak(self):
        print("Some sound")

class Cat(Animal):
    def speak(self):
        print("Meow")

c = Cat()
c.speak()  # Meow

#Module

# my_module.py
def greet(name):
    return f"Hello {name}"

# main.py
import my_module
print(my_module.greet("Ana"))

#Error Handling

try:
    x = int("abc")
except ValueError:
    print("Not a number!")
finally:
    print("Done")



