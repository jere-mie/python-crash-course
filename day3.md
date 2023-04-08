# Day 3 ~ Functions and Modules in Python

Functions and modules are important concepts in Python programming. Functions allow us to write reusable code that can be called multiple times with different inputs, while modules allow us to organize our code into separate files for better maintainability. In this article, we will cover how to create and use functions and modules in Python.

## Functions

A function is a block of code that performs a specific task. In Python, we define a function using the def keyword, followed by the function name and a set of parentheses. Here is an example:

```py
def greet(name):
    print("Hello, " + name + "!")

greet("Alice")
greet("Bob")
```

In the above code, we define a function called greet that takes a single argument name and prints a greeting message. We then call the function twice with different arguments.

Functions can also return a value using the return keyword. Here is an example:

```py
def square(x):
    return x * x

result = square(5)
print(result)
```

In the above code, we define a function called square that takes a single argument x and returns the square of x. We then call the function with the argument 5 and store the result in a variable called result. We then print the value of result, which should be 25.

## Modules

A module is a file that contains Python code, usually organized around a specific topic or functionality. In Python, we can import a module using the import keyword, followed by the name of the module. Here is an example:

```py
import math

result = math.sqrt(25)
print(result)
```

In the above code, we import the math module, which contains various mathematical functions. We then use the sqrt function from the math module to compute the square root of 25 and store the result in a variable called result. We then print the value of result, which should be 5.

We can also create our own modules by defining functions and variables in a separate file and importing them into our main program. Here is an example:

```py
# file: mymodule.py

def greet(name):
    print("Hello, " + name + "!")

def square(x):
    return x * x
```

```py
# file: main.py

import mymodule

mymodule.greet("Alice")

result = mymodule.square(5)
print(result)
```

In the above code, we define a module called mymodule in a separate file. The module contains two functions: greet and square. We then import the mymodule module into our main program and use the greet function to print a greeting message. We also use the square function to compute the square of 5 and store the result in a variable called result. We then print the value of result, which should be 25.

## Conclusion

In this article, we covered how to create and use functions and modules in Python. We learned how to define functions using the def keyword and how to import modules using the import keyword. We also learned how to create our own modules by defining functions and variables in a separate file.
