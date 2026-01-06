# Functions
A function is defined as a block of code that runs only when it is called.
The importance of function syntax is:
Starts with the keyword def
Followed by the function name and parentheses (which may include parameters)
Ends with a colon :
The function body is indented, which is critical in Python.
Functions encapsulate reusable code and improve program structure.

## Function Syntax and Structure:
def function_name(parameters):
    # function body
function calls and how Python’s built-in input() function works inside custom functions.
Examples include passing strings and numeric values as arguments.

Arbitrary Arguments and Keyword Arguments:
Arbitrary arguments (*args) allow passing an arbitrary number of positional arguments.
Keyword arguments (**kwargs) allow passing arbitrary keyworded (named) arguments as dictionaries.

## Nested Functions:
Outer function contains an inner function, both with their own code blocks.
Useful for encapsulation and creating closures.
Example:
def outer():
    print("This is outer function")
    def inner():
        print("This is inner function")
    inner()
    
Modules and Collection of Functions:
A module is described as a collection of related functions grouped into a single Python file.
Modules facilitate code reuse and organization.
Example usage and import statements are mentioned but not elaborated in detail.

## Lambda Functions:
Syntax:
lambda arguments: expression
Lambda functions are a core part of advanced functional programming in Python.
Useful for short, throwaway functions used inline with map, filter, etc.
Emphasized that Lambda functions do not have a name unless assigned to a variable.

# Advance Functions
##
map():	Applies a function to all items in an iterable and returns a new iterable with transformed items
filter():	Applies a function that returns a boolean to filter items, returning only those where function is True
The reduce() function applies a function cumulatively to items in an iterable, reducing it to a single value.
Example: summing a list of numbers:
reduce(lambda x, y: x + y, [1, 2, 3, 4, 5])  # returns 15

## Generators and yield Statement:
Introduces generator functions, which use the yield statement instead of return.
Key points about generators:
yield pauses function execution, saving the state for resumption.
When the generator is iterated, it resumes from the last yield.
Generators produce items one at a time, useful for memory-efficient iteration over large datasets.
Multiple yield statements can exist in one generator function.
The use of yield contrasts with return, which exits the function completely.
