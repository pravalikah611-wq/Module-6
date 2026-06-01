# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

---

## 🧠 ALGORITHM

1. **Create Class `Beans`**:
   - Define `type()` method that prints `"Vegetable"`.
   - Define `color()` method that prints `"Green"`.

2. **Create Class `Mango`**:
   - Define `type()` method that prints `"Fruit"`.
   - Define `color()` method that prints `"Yellow"`.

3. **Define Generic Function `func(obj)`**:
   - Call `obj.type()` and `obj.color()` — this works with both `Beans` and `Mango` objects, showcasing **polymorphism**.

4. **Create Objects**:
   - Instantiate `Beans` and `Mango`.
   - Pass them to `func()` and execute the program.

---

## 💻 Program:

class Beans:
    def type(self):
        return "Vegetable"

    def color(self):
        return "Green"

class Mango:
    def type(self):
        return "Fruit"

    def color(self):
        return "Yellow"

def check(obj):
    print(obj.type())
    print(obj.color())

b = Beans()
m = Mango()

check(b)
check(m)

<img width="1823" height="746" alt="image" src="https://github.com/user-attachments/assets/21a7ff37-1ae5-41bd-98c9-f02e5e4ded5a" />


## Output:

<img width="1823" height="746" alt="image" src="https://github.com/user-attachments/assets/a5a5d4d9-d22e-4326-b625-88ba857027d8" />


## Result:

Program executed successfully showing type and color using polymorphism.
