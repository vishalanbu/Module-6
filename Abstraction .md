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

## PROGRAM

```python
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


rectangle = Rectangle()
circle = Circle()

print("Area of Rectangle:", rectangle.calculate_area())
print("Area of Circle:", circle.calculate_area())
```

## OUTPUT

```text
Area of Rectangle: 50
Area of Circle: 153.93804002589985
```

## RESULT

Thus, the Python program successfully demonstrates an abstract class and abstract method using `Shape`, `Rectangle`, and `Circle`.
