# Day 4 ~ Strings and Lists

Now we will be focusing on two important data types in Python - strings and lists. Both of these are widely used in various applications and are essential for any beginner to learn.

## String Manipulation

Strings are sequences of characters enclosed within quotes. They can be manipulated in various ways to extract, replace or modify specific parts of the string.

Here are a few commonly used string manipulation techniques:

### Indexing

Indexing is the process of accessing individual characters within a string using their position. In Python, indexing starts at 0. To access a specific character, we can use the square brackets [] with the index number inside them.

```py
string = "Python Crash Course"
print(string[0])   # Output: 'P'
print(string[6])   # Output: 'C'
```

### Slicing

Slicing is the process of extracting a portion of a string. We can specify a range of indexes within the square brackets [] to extract a part of the string.

```py
string = "Python Crash Course"
print(string[0:6])  # Output: 'Python'
print(string[7:])   # Output: 'Crash Course'
```

### Concatenation

Concatenation is the process of joining two or more strings. We can use the + operator to concatenate two or more strings.

```py
string1 = "Python"
string2 = " Crash Course"
print(string1 + string2)   # Output: 'Python Crash Course'
```

## String Methods

In addition to the above-mentioned techniques, Python provides several built-in methods to manipulate strings. Here are a few commonly used string methods:

### split()

The split() method splits a string into a list of substrings based on a specified delimiter. By default, the delimiter is a space character.

```py
string = "Python Crash Course"
print(string.split())   # Output: ['Python', 'Crash', 'Course']
```

### strip()

The strip() method removes any leading and trailing whitespace characters from a string.

```py
string = "   Python Crash Course   "
print(string.strip())   # Output: 'Python Crash Course'
```

### upper()

The upper() method converts all the characters in a string to uppercase.

```py
string = "Python Crash Course"
print(string.upper())   # Output: 'PYTHON CRASH COURSE'
```

## Lists and their Methods

Lists are a collection of items enclosed within square brackets []. They are used to store multiple items of different data types in a single variable.

Here are a few commonly used list methods:

### append()
The append() method adds an item to the end of a list.

```
my_list = [1, 2, 3]
my_list.append(4)
print(my_list)   # Output: [1, 2, 3, 4]
```

### remove()

The remove() method removes the first occurrence of a specified item from a list.

```
my_list = [1, 2, 3, 4]
my_list.remove(3)
print(my_list)   # Output: [1, 2, 4]
```

### sort()

The sort() method sorts the items of a list in ascending order.

```
my_list = [4, 2, 1, 3]
my_list.sort()
print(my_list)   # Output: [1, 2, 3, 4]
```

## Conclusion

To conclude, introduced us to string manipulation techniques such as indexing, slicing, and concatenation, along with built-in string methods like split(), strip(), and upper(). We also learned about lists, a collection of items, and their methods like append(), remove(), and sort(). These fundamental concepts and techniques are essential for any beginner in Python and will be used extensively in most Python applications.
