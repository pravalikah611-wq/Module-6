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

## 💻 Program:

from abc import ABC, abstractmethod
import math

# Abstract class
class Shape(ABC):

    @abstractmethod
    def calculate_area(self):
        pass

# Subclass Rectangle
class Rectangle(Shape):
    def __init__(self, length, breadth):
        self.length = length
        self.breadth = breadth

    def calculate_area(self):
        return self.length * self.breadth

# Subclass Circle
class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius

    def calculate_area(self):
        return math.pi * self.radius * self.radius


# Creating objects
rect = Rectangle(10, 5)
circle = Circle(7)

# Display results
print("Area of Rectangle:", rect.calculate_area())
print("Area of Circle:", circle.calculate_area())

<img width="1786" height="836" alt="image" src="https://github.com/user-attachments/assets/1e5d41ca-a779-4d62-a314-d58d1dd28fe0" />

<img width="1631" height="677" alt="image" src="https://github.com/user-attachments/assets/56a15025-5fe0-43f6-8daf-526efac6602a" />

## Output:
<img width="1786" height="836" alt="image" src="https://github.com/user-attachments/assets/8397b24b-9b77-4d51-9744-0d79d4ed6aee" />


## Result:
The program successfully demonstrates abstraction in Python by creating an abstract class Shape and implementing the calculate_area method in its subclasses Rectangle and Circle.
