# EX 1 : Python OOP: Abstract Class & Method Example

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
```python3
import math 
from abc import ABC
class type_shape(ABC): 
    def __init__(self):
        pass
    #create abstract method area()
    def area(self):
        pass

class Rectangle(type_shape):
  length = 6
  breadth = 4
  def area(self):
      return self.length*self.breadth

class Circle(type_shape):
  radius = 7
  def area(self):
      return 3.14*self.radius**2
class Square(type_shape):
  length = 4
  def area(self):
      return 4*self.length

class triangle:
  length = 5
  width = 4
  def area(self):
      return 0.5*self.length*self.width
r=Rectangle()
c=Circle()
s = Square() # object created for the class 'Square'
t = triangle() # object created for the class 'triangle'
print("Area of a rectangle:", r.area()) # call to 'area' method defined inside the class.
print("Area of a circle:", c.area()) # call to 'area' method defined inside the class.
print("Area of a square:", s.area()) # call to 'area' method defined inside the class.
print("Area of a triangle:", t.area()) # call to 'area' method defined inside the class.
```

## Output
<img width="1383" height="924" alt="image" src="https://github.com/user-attachments/assets/2bdfc7f0-25f4-4a54-95c0-de0899444128" />

## Result
Thus the python program to create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle` is completed successfully.
<br>
<br>

#  EX 2 : Python OOP: Encapsulation with Private Members

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
```python3
class Rectangle:
  __length = 0 #private variable
  __breadth = 0#private variable
  def __init__ (self,__length,__breadth):
    #constructor
    self.__length = 5
    self.__breadth = 3
    print(self.__length)
    print(self.__breadth)
 
rect = Rectangle(5,3)



```

## Output
<img width="1364" height="918" alt="image" src="https://github.com/user-attachments/assets/4f5c6da6-5ad0-4215-aca6-76c79454c927" />

## Result
Thus the python program to implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth` has been done successfully.




<br>
<br>


# EX 3 : Method Overriding-Fish and Shark Class Inheritance in Python

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
```python3
class Fish:
      def type(self):
          print("fish")

class Shark(Fish):
	def type(self):
	    print("shark")

obj_goldfish=Fish()
obj_hammerhead=Shark()
obj_goldfish.type()
obj_hammerhead.type()
```
## OUTPUT
<img width="1372" height="815" alt="image" src="https://github.com/user-attachments/assets/38b43872-d1b5-4e17-83d4-f4957adaa1d2" />

## RESULT
Thus the python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method is completed successfully.




<br>
<br>


# EX 4 : Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.

2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

---

## 💻 Program
```python3
class A:
    def __init__(self, value):
        self.value = value

    def __lt__(self, other):
        return self.value < other.value


ob1 = A(200)
ob2 = A(30)

if ob2 < ob1:
    print("ob2 is less than ob1")
else:
    print("ob2 is not less than ob1")
```
## Output
<img width="1095" height="811" alt="image" src="https://github.com/user-attachments/assets/6be1dec3-4a71-4871-8d9b-bdd4b64ab210" />

## Result
Thus the python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class is completed successfully.




<br>
<br>

# EX 5 : Python OOP: Polymorphism with Classes

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
```python3
class Beans(): 
     def type(self): 
       return ("Vegetable") 
     def color(self):
       return("Green") 
class Mango(): 
     def type(self): 
       return("Fruit") 
     def color(self): 
       return("Yellow")      
def func(o): 
      print(o.type())
      print(o.color())
obj_beans = Beans() 
obj_mango = Mango() 
func(obj_beans) 
func(obj_mango)
```
## Output
<img width="1366" height="925" alt="image" src="https://github.com/user-attachments/assets/27fb935f-8052-4f9c-be15-772ce31823f0" />

## Result
Thus the python program to create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism is completed successfully.
