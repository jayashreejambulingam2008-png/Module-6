```
DONE BY: JAYASHREE J
REGISTER NUMBER: 212225040145
```
# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```
from abc import ABC, abstractmethod
import math

class Shape(ABC):
    @abstractmethod
    def calculate_area(self):
        pass

class Rectangle(Shape):
    def __init__(self, length=10, breadth=5):
        self.length = length
        self.breadth = breadth

    def calculate_area(self):
        return self.length * self.breadth

class Circle(Shape):
    def __init__(self, radius=7):
        self.radius = radius

    def calculate_area(self):
        return math.pi * self.radius * self.radius

r = Rectangle()
c = Circle()

print("Area of Rectangle:", r.calculate_area())
print("Area of Circle:", c.calculate_area())
```
## Output
<img width="915" height="243" alt="image" src="https://github.com/user-attachments/assets/fc65b48e-d9cf-4b08-8df7-b3577ab92557" />

## Result
Hence the given task to create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle` has been done successfully.

# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```
class Rectangle:
    def __init__(self, length, breadth):
        self.__length = length
        self.__breadth = breadth

    def display(self):
        print("Length:", self.__length)
        print("Breadth:", self.__breadth)

obj = Rectangle(10, 5)
obj.display()
```
## Output
<img width="916" height="253" alt="image" src="https://github.com/user-attachments/assets/21714b72-46b2-4ab8-aa02-bf7c8d6c4148" />

## Result
Hence the given task to implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth` has been done successfully.

