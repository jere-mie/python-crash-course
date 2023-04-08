# Day 6 ~ Object-Oriented Programming

Today, we're going to dive into the world of Object-Oriented Programming (OOP) in Python. OOP is a programming paradigm that uses objects and classes to organize and structure code. It's a powerful way to create modular and reusable code, and it's used extensively in Python.

## Classes and Objects

In Python, a class is a blueprint for creating objects. A class defines a set of attributes and methods that describe the behavior and properties of the objects created from it. Here's a simple example of a class in Python:

```py
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def say_hello(self):
        print(f"Hello, my name is {self.name} and I'm {self.age} years old.")
```

In this example, we defined a class called Person that has two attributes (name and age) and one method (say_hello()). The __init__() method is a special method that gets called when a new object is created from the class. It initializes the object's attributes with the values passed as arguments. The say_hello() method is a simple method that prints out a greeting using the object's name and age attributes.

To create a new object from the Person class, we use the following syntax:

```py
person = Person("John", 30)
```

In this example, we created a new Person object called person with the name "John" and the age 30. We can then call the say_hello() method on the person object like this:

```py
person.say_hello()
```

This will output the following message:

```
Hello, my name is John and I'm 30 years old.
```

## Inheritance and Polymorphism

Inheritance is a key concept in OOP that allows us to create new classes based on existing ones. When a class inherits from another class, it inherits all of its attributes and methods. We can then add new attributes and methods to the subclass, or override existing ones.

Here's an example of a subclass of the Person class:

```py
class Student(Person):
    def __init__(self, name, age, major):
        super().__init__(name, age)
        self.major = major
    
    def say_hello(self):
        print(f"Hello, my name is {self.name} and I'm {self.age} years old. I'm studying {self.major}.")
```

In this example, we defined a new class called Student that inherits from the Person class. We added a new attribute (major) and overrode the say_hello() method to include the major attribute in the output.

We can create a new Student object in the same way we created a Person object:

```py
student = Student("Jane", 20, "Computer Science")
```

And we can call the say_hello() method on the student object:

```py
student.say_hello()
```

This will output the following message:

```
Hello, my name is Jane and I'm 20 years old. I'm studying Computer Science.
```

Polymorphism is another important concept in OOP that allows us to use objects of different classes in the same way. Polymorphism is achieved through inheritance and method overriding, as we saw in the example above.

## Using Python's Built-In Classes

Python comes with a number of built-in classes that we can use in our programs. These classes provide functionality for common tasks, such as working with files, managing dates and times, and manipulating strings.

Here's an example of using Python's built-in datetime class to work with dates and times:

```py
import datetime

now = datetime.datetime.now()
print(now.strftime("Today is %A, %B %d, %Y"))
```

In this example, we imported the datetime module and used the datetime.now() method to get the current date and time. We then used the strftime() method to format the date and time string in a readable format.

Here's another example of using Python's built-in csv module to read and write CSV files:

```py
import csv

with open('data.csv', 'w', newline='') as file:
    writer = csv.writer(file)
    writer.writerow(['Name', 'Age', 'Gender'])
    writer.writerow(['John', '30', 'Male'])
    writer.writerow(['Jane', '25', 'Female'])

with open('data.csv', newline='') as file:
    reader = csv.reader(file)
    for row in reader:
        print(row)
```

In this example, we used the csv module to write a CSV file called data.csv with three rows of data. We then used the csv.reader() method to read the contents of the CSV file and print them to the console.

Python's built-in classes provide a wide range of functionality that can help us write more efficient and readable code. By using these classes and understanding how they work, we can write programs that are easier to maintain and scale.

## Conclusion

Today we delved into the world of Object-Oriented Programming (OOP) and learned about classes, objects, inheritance, and polymorphism. We saw how OOP can help us write more organized, modular, and reusable code, making it easier to maintain and scale our programs. We also explored how to use Python's built-in classes, which provide a wide range of functionalities for common tasks such as working with files, managing dates and times, and manipulating strings. By mastering these concepts, we can become more proficient in Python programming and take on more complex challenges with confidence.
