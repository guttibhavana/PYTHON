Object Oriented Programming (OOP) in Python

Object Oriented Programming (OOP) is a programming paradigm based on the concept of objects. Objects combine both data (attributes) and methods (functions) into a single unit. OOP focuses on modeling real-world entities and their interactions, unlike procedural programming which focuses only on functions and logic.
The main goal of OOP is to make programs more modular, reusable, flexible, and easy to maintain.

Core Principles of OOP

OOP is built on four main principles:
Encapsulation
Inheritance
Polymorphism
Abstraction

These four principles are known as the four pillars of Object Oriented Programming.

Class:
A class is a user-defined data type that binds data members (variables) and member functions (methods) into a single unit. It acts as a blueprint or template for creating objects.
A class defines:
What data an object will store
What actions an object can perform
Classes help in organizing code into logical and reusable components.

Object:
An object is an instance of a class. It represents a real-world entity and contains:
Properties (attributes) – store data
Methods – define behavior
Objects are created from classes through a process called instantiation.
Memory is allocated only when an object is created, not when the class is defined.

Constructor:
A constructor is a special method used to initialize an object’s data when it is created.
In Python, the constructor is named __init__().
The __init__() method is automatically called when an object is created. It is used to assign initial values to object attributes.
Python does not support multiple constructors (constructor overloading).
The self keyword refers to the current object and is used to access instance variables and methods.

Inheritance:
Inheritance allows one class (child or subclass) to acquire the properties and methods of another class (parent or superclass). It promotes code reuse and creates a hierarchical relationship between classes.
Types of Inheritance
Single Inheritance – One parent and one child class
Multilevel Inheritance – A chain of inheritance (grandparent → parent → child)
Multiple Inheritance – One child inherits from multiple parent classes
Hierarchical Inheritance – One parent with multiple child classes
Inheritance helps in building relationships among classes and reduces code duplication.

Polymorphism:
Polymorphism means “many forms”. It allows the same function or method name to behave differently in different situations.
Types of Polymorphism
Method Overloading – Multiple methods with the same name but different parameters (not supported directly in Python)
Method Overriding – A child class provides its own version of a method that is already defined in the parent class
Polymorphism improves flexibility and supports dynamic behavior in programs.

Encapsulation:
Encapsulation is the process of binding data and methods together and restricting direct access to some of the object’s components. It helps protect data from accidental modification.
It ensures data security and controlled access through methods.
Access Modifiers
Access modifiers control the visibility of data and methods in a class.
Python uses naming conventions instead of strict access rules:
Public – accessible from anywhere
Protected (_) – accessible within the class and its subclasses
Private (__) – accessible only inside the class
These conventions help in maintaining data safety and proper usage.

Abstraction:
Abstraction means hiding internal implementation details and showing only what is necessary. It helps in reducing complexity and improving code clarity.
Users interact with what an object does, not how it does it. This is useful for large and complex programs.

Conclusion:
Object Oriented Programming provides a powerful way to structure programs using real-world models. By using classes, objects, inheritance, polymorphism, encapsulation, and abstraction, Pyt
