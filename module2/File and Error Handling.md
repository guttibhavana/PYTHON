# FILE HANDLING IN PYTHON

File handling allows data to be stored permanently in files instead of losing it when a program stops.
Python provides the built-in open() function to work with files.
file = open("data.txt", "mode")
File Modes:
`r` -- Read only                          
`w` -- Write (overwrites existing content) 
`a` -- Append (adds data at the end)       
`r+` -- Read and write                      
`w+` -- Write and read                     
`a+` -- Append and read  
## Reading from a File
Files can be read using methods such as:
read() – reads the entire file
readline() – reads one line at a time
readlines() – reads all lines as a list
The content of a file can be stored in a variable and printed to verify the data.

## Writing to a File
The write() function is used to write data into a file. When a file is opened in write mode, the existing data is removed and replaced with new data.

Append Mode
When a file is opened in append mode, new data is added at the end of the file without deleting existing data. This ensures that no previous information is lost.

File Pointer (Cursor)
The file pointer is like a cursor that indicates the current position in the file where data will be read or written.

seek() and tell()
seek() is used to move the file pointer to a specific position.
tell() returns the current position of the file pointer.
These methods help in controlling exactly where reading or writing takes place inside a file.

truncate()
The truncate() method deletes all file content from the current pointer position to the end of the file.

Closing a File
After completing file operations, the file must be closed using the close() method to free system resources.
with Statement
The with statement is used to open a file in a safe way. It automatically closes the file after the operations are completed.


# Exception Handling in Python
An exception is an error that occurs during the execution of a program. Instead of stopping the program abruptly, exceptions allow the program to handle errors gracefully.

Types of Errors
Compile-time errors (Syntax errors) – These occur due to incorrect code structure and must be fixed before the program runs.
Runtime errors – These occur while the program is running, such as dividing a number by zero.

## try and except
The try block contains code that may cause an error.
The except block handles the error so that the program does not crash.

## Multiple Exceptions
Different types of runtime errors can be handled separately using multiple except blocks or together in a single block.

else Block
The else block runs when no exception occurs in the try block.

## finally Block
The finally block always executes, whether an error occurs or not. It is used for cleanup tasks like closing files.

## Raising Exceptions
Python allows programmers to manually raise exceptions using the raise keyword when a specific condition is violated.

