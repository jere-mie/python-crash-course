# Day 2 ~ Control Structures in Python: Conditional Statements and Loops

In Python, control structures are used to control the flow of a program. They allow us to execute certain blocks of code based on specific conditions or repeat certain blocks of code a certain number of times. In this article, we will cover two important control structures: conditional statements and loops.

## Conditional Statements: If-Else

Conditional statements allow us to execute certain blocks of code based on a specific condition. In Python, the most common conditional statement is the if statement. Here is an example:

```py
age = 18

if age >= 18:
    print("You are old enough to vote.")
else:
    print("You are not old enough to vote.")
```

In the above code, we use the if statement to check if the age variable is greater than or equal to 18. If it is, the program will print "You are old enough to vote." If it is not, the program will print "You are not old enough to vote."

We can also use the elif statement to check multiple conditions. Here is an example:

```py
age = 18

if age < 18:
    print("You are not old enough to vote.")
elif age == 18:
    print("You are now eligible to vote for the first time!")
else:
    print("You are eligible to vote.")
```

In the above code, we use the elif statement to check if the age variable is equal to 18. If it is, the program will print "You are now eligible to vote for the first time!" If it is not, the program will check if the age variable is less than 18. If it is, the program will print "You are not old enough to vote." If none of these conditions are met, the program will print "You are eligible to vote."

## Loops: For and While

Loops allow us to execute certain blocks of code repeatedly. In Python, there are two types of loops: for loops and while loops.

A for loop is used to iterate over a sequence of elements. Here is an example:

```py
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)
```

In the above code, we use a for loop to iterate over the fruits list and print each element.

A while loop is used to execute a block of code repeatedly as long as a specific condition is met. Here is an example:

```py
i = 0

while i < 5:
    print(i)
    i += 1
```

In the above code, we use a while loop to print the values of the i variable from 0 to 4.

## Conclusion

In this article, we covered two important control structures in Python: conditional statements and loops. We learned how to use the if-else statement to execute certain blocks of code based on specific conditions, and we learned how to use for and while loops to repeat certain blocks of code a certain number of times.
