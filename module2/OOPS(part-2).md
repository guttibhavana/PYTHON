## Inheritance:
Inheritance allows a child class to reuse properties and methods of a parent class, promoting code reuse and extension.

```class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def greet(self):
        print(f"Hello, my name is {self.name} and I am {self.age} years old.")
class Student(Person):
    def __init__(self, name, age, student_id):
        super().__init__(name, age)  # Inherit parent properties
        self.student_id = student_id
    
    def study(self):
        print(f"{self.name} is studying.")

#Using the classes
student = Student("Alice", 20, "S123")
student.greet()  # inherited method from Person
student.study()  # method from Student
```

## Polymorphism:
Polymorphism means "many forms"—the same method can behave differently depending on the object calling it.
```class Citizen:
    def work(self):
        print("Working in a general job.")

class Teacher(Citizen):
    def work(self):
        print("Teaching students.")

class Student(Citizen):
    def work(self):
        print("Studying for exams.")

Using polymorphism
people = [Citizen(), Teacher(), Student()]
for person in people:
    person.work()  # same method name, different behavior
```

## Encapsulation:
Encapsulation controls access to the internal state of an object using access modifiers:
Public: Accessible anywhere (name)
Protected: Accessible within class and subclasses (_name)
Private: Accessible only within class (__name)
```class BankAccount:
    def __init__(self, owner, balance):
        self.owner = owner      # public
        self._balance = balance # protected
        self.__pin = 1234       # private
    
    def deposit(self, amount):
        self._balance += amount
        print(f"Deposited {amount}, new balance: {self._balance}")
    
    def __show_pin(self):
        print(f"PIN is {self.__pin}")

account = BankAccount("Bob", 1000)
account.deposit(500)
print(account.__pin)  # Error! Private
```
## Access Modifiers & Variable Scope:
Local Variables: Defined inside a function; inaccessible outside.
Global Variables: Accessible throughout the program.
```global_var = "I am global"
def test_scope():
    local_var = "I am local"
    print(local_var)
    print(global_var)

test_scope()
print(local_var)  # Error! local_var not accessible outside
```

## Abstract Classes and Methods:
Abstract Classes cannot be instantiated directly. They define templates for subclasses with abstract methods.

```from abc import ABC, abstractmethod

class Vehicle(ABC):
    @abstractmethod
    def start_engine(self):
        pass  # must be implemented in child classes

class Car(Vehicle):
    def start_engine(self):
        print("Car engine started!")

class Bike(Vehicle):
    def start_engine(self):
        print("Bike engine started!")

vehicle = Vehicle()  # Error! Cannot instantiate abstract class
car = Car()
car.start_engine()
bike = Bike()
bike.start_engine()
```
