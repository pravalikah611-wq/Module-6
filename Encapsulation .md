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

## 💻 Program:

class Rectangle:
    def __init__(self, length, breadth):
        self.__length = length      # private variable
        self.__breadth = breadth    # private variable

    # Setter method
    def set_dimensions(self, length, breadth):
        self.__length = length
        self.__breadth = breadth

    # Getter methods
    def get_length(self):
        return self.__length

    def get_breadth(self):
        return self.__breadth

    # Method to calculate area
    def area(self):
        return self.__length * self.__breadth


# Input from user
l = int(input("Enter length: "))
b = int(input("Enter breadth: "))

# Object creation
rect = Rectangle(l, b)

# Display results
print("Length:", rect.get_length())
print("Breadth:", rect.get_breadth())
print("Area:", rect.area())

<img width="1869" height="793" alt="image" src="https://github.com/user-attachments/assets/8909122a-4a27-4de0-bab7-3cc669d293f9" />


## Output:

<img width="1869" height="793" alt="image" src="https://github.com/user-attachments/assets/57ff174e-beba-43cc-ad9a-b3aab039fbd6" />


## Result:
Thus, the Python program using encapsulation with private variables __length and __breadth in the Rectangle class was successfully executed and the area of the rectangle was calculated.
