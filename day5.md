# Day 5 ~ Dictionaries and Tuples

Now we will be exploring two more data types in Python - dictionaries and tuples. These data types are useful in different ways, and understanding their properties and methods is essential for building advanced applications.

## Creating and Manipulating Dictionaries

Dictionaries are unordered collections of key-value pairs enclosed within curly braces {}. They are used to store and manipulate data in a structured format.

Here's an example of creating and accessing a dictionary:

```py
person = {'name': 'John', 'age': 30, 'city': 'New York'}
print(person['name'])   # Output: 'John'
```

We can add, update or remove items from a dictionary using the following methods:

### Adding an item

```py
person['email'] = 'john@example.com'
```

### Updating an item

```py
person['age'] = 35
```

### Removing an item

```py
del person['city']
```

## Tuples and Their Methods

Tuples are ordered collections of items enclosed within parentheses (). They are similar to lists, but unlike lists, tuples are immutable, which means they cannot be modified after creation.

Here's an example of creating and accessing a tuple:

```py
my_tuple = (1, 2, 3, 4, 5)
print(my_tuple[0])   # Output: 1
```

We can use the following methods to manipulate tuples:

### count()

The count() method returns the number of times a specified item appears in a tuple.

```py
my_tuple = (1, 2, 3, 4, 5, 1)
print(my_tuple.count(1))   # Output: 2
```

### index()

The index() method returns the index of the first occurrence of a specified item in a tuple.

```py
my_tuple = (1, 2, 3, 4, 5)
print(my_tuple.index(3))   # Output: 2
```

## Basic File Input/Output (I/O)

File Input/Output (I/O) is a core functionality of any programming language, and Python provides built-in functions to read and write files. In this section, we'll cover the basics of file I/O in Python.

### Opening Files

Before we can read or write to a file, we need to open it first. We use the built-in open() function to open a file in Python. The open() function takes two arguments: the filename and the mode in which to open the file.

```py
file = open('example.txt', 'r')   # opens the file in read mode
```

The open() function returns a file object that we can use to read or write to the file.

### Reading from Files
Once we've opened a file, we can read its contents using the read() method.

```py
file = open('example.txt', 'r')   # opens the file in read mode
data = file.read()   # reads the entire file contents
print(data)
```

The read() method reads the entire contents of the file and returns it as a string.

We can also read a file line by line using the readline() method.

```py
file = open('example.txt', 'r')   # opens the file in read mode
line = file.readline()   # reads the first line of the file
print(line)
```

The readline() method reads a single line from the file and returns it as a string.

### Writing to Files

To write to a file, we need to open the file in write mode using the open() function with the mode argument set to 'w'. If the file does not exist, Python will create it.

```py
file = open('example.txt', 'w')   # opens the file in write mode
file.write('Hello, world!')   # writes the string to the file
file.close()   # closes the file
```

The write() method writes a string to the file. We must remember to close the file using the close() method once we're done writing to it.

### Appending to Files

If we want to add new data to an existing file without overwriting its existing contents, we can open the file in append mode using the open() function with the mode argument set to 'a'.

```py
file = open('example.txt', 'a')   # opens the file in append mode
file.write('\nHello, again!')   # writes a new line to the file
file.close()   # closes the file
```

The write() method in append mode adds the new data to the end of the file without modifying its existing contents.

### Closing Files

After we're done reading from or writing to a file, we need to close the file using the close() method. This frees up system resources and ensures that any changes made to the file are saved.

```py
file = open('example.txt', 'r')
data = file.read()
file.close()
```

It's good practice to close a file immediately after we're done using it to avoid any data corruption issues.

### Using the with Statement

To avoid the hassle of opening and closing a file manually, we can use the with statement in Python. The with statement automatically closes the file once we're done working with it.

```py
with open('example.txt', 'r') as file:
    data = file.read()
```

We can use the with statement with any file I/O operation, including reading, writing, and appending. Here's an example of how to use the with statement to write to a file:

```py
with open('example.txt', 'w') as file:
    file.write('Hello, world!')
```

In this example, we opened the example.txt file in write mode using the with statement. We then wrote the string 'Hello, world!' to the file using the write() method. When we're done working with the file, the with statement automatically closes the file for us.

### Working with Binary Files

Python can also work with binary files, such as images, videos, and audio files. To open a file in binary mode, we use the 'b' character in the mode argument when calling the open() function.

```py
with open('example.png', 'rb') as file:
    data = file.read()
```

In this example, we opened the example.png file in binary mode using the 'rb' mode argument. We then read the entire contents of the file into the data variable using the read() method.

## Conclusion

In conclusion, we have introduced dictionaries and tuples, two more data types in Python that are useful in different ways. We also learned about basic file I/O, which is essential for reading and writing files in Python. These concepts and techniques are fundamental to building advanced applications in Python.
