# 🐟 Method Overriding-Fish and Shark Class Inheritance in Python

## 🧠 AIM:
To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

## 📋 ALGORITHM:

1. Define the `Fish` class with a method named `type()` that prints `"fish"`.
2. Define the `Shark` class as a subclass of `Fish`, and override the `type()` method to print `"shark"`.
3. Create an instance of the `Fish` class named `obj_goldfish`.
4. Create an instance of the `Shark` class named `obj_hammerhead`.
5. Use a `for` loop to iterate over both objects.
6. Within the loop, call the `type()` method using the loop variable.
7. Output will demonstrate method overriding: printing `"fish"` and `"shark"` accordingly.

## 💻 PROGRAM:
# Parent class
class Fish:
    def type(self):
        print("This is a general fish")

# Child class
class Shark(Fish):
    def type(self):
        print("This is a shark, a dangerous fish")

# Object creation
f = Fish()
s = Shark()

# Calling methods
f.type()
s.type()


<img width="1659" height="647" alt="image" src="https://github.com/user-attachments/assets/1f3605e5-9221-4510-bde7-fbb054efdaad" />


## OUTPUT:

<img width="1659" height="647" alt="image" src="https://github.com/user-attachments/assets/d74bd0dd-d555-45fe-80d4-3670667c0b15" />


## RESULT:
The program demonstrates inheritance and method overriding in Python, where the child class Shark overrides the type() method of the parent class Fish, and the output displays the method of the child class.
