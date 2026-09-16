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

## 💻 Program

```python id="w3k9pt"
class Beans:

    def type(self):
        print("Vegetable")

    def color(self):
        print("Green")


class Mango:

    def type(self):
        print("Fruit")

    def color(self):
        print("Yellow")


def func(obj):
    obj.type()
    obj.color()


beans = Beans()
mango = Mango()

func(beans)
func(mango)
```

## OUTPUT

```text id="x6q2rm"
Vegetable
Green
Fruit
Yellow
```

## RESULT

Thus, the Python program successfully demonstrates **polymorphism** using the `Beans` and `Mango` classes with a generic function.
