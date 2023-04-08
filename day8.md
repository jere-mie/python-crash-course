# Day 8 ~ Regular Expressions

Regular expressions (regex) are a powerful tool for working with text in Python. They allow you to search for and match patterns in strings, which can be useful in a wide range of applications. Today, we will cover the basics of regular expressions and how to use them in Python.

## What are regular expressions?

Regular expressions are a sequence of characters that define a search pattern. They are used to search for and match text based on patterns, rather than exact strings. Regular expressions are widely used in programming, text editors, and command-line utilities.

## Basic regular expression syntax

Regular expressions use a combination of special characters and symbols to define patterns. Here are some of the basic syntax elements used in regular expressions:

- `.` - Matches any character except a newline. For example, a.b would match "aab", "aeb", "acb", etc.
- `^` - Matches the beginning of a string. For example, ^hello would match "hello world", but not "world hello".
- `$` - Matches the end of a string. For example, world$ would match "hello world", but not "world hello".
- `*` - Matches zero or more occurrences of the preceding character or group. For example, ab*c would match "ac", "abc", "abbc", "abbbc", etc.
- `+` - Matches one or more occurrences of the preceding character or group. For example, ab+c would match "abc", "abbc", "abbbc", etc., but not "ac".
- `?` - Matches zero or one occurrence of the preceding character or group. For example, ab?c would match "ac" or "abc".
- `[]` - Matches any one of the enclosed characters. For example, [aeiou] would match any vowel.
- `()` - Groups the enclosed characters. For example, (abc)+ would match "abc", "abcabc", "abcabcabc", etc.

## Regular expression methods in Python

Python has a built-in module for working with regular expressions called re. Here are some of the most commonly used methods in the re module:

- `re.search(pattern, string)` - Searches the string for a match to the pattern.
- `re.match(pattern, string)` - Matches the pattern at the beginning of the string.
- `re.findall(pattern, string)` - Finds all occurrences of the pattern in the string and returns them as a list.
- `re.sub(pattern, repl, string)` - Substitutes all occurrences of the pattern in the string with the replacement string.

Here is an example of how to use the re module in Python:

```py
import re

text = "The quick brown fox jumps over the lazy dog"

# Search for the word "brown" in the text
match = re.search("brown", text)
if match:
    print("Found a match!")
else:
    print("No match")

# Replace the word "fox" with "cat"
new_text = re.sub("fox", "cat", text)
print(new_text)
```

In this example, we first import the re module. Then we define a string text which contains the sentence "The quick brown fox jumps over the lazy dog".

We use the re.search() method to search for the word "brown" in the text. If a match is found, we print "Found a match!". If no match is found, we print "No match".

Next, we use the re.sub() method to replace the word "fox" with "cat" in the text. We store the new text in the new_text variable and print it out.

## Conclusion

Today we learned about regular expressions and how they can be used to search for, match, and manipulate text in Python. We covered the basic syntax of regular expressions and how to use the re module to perform operations such as searching for matches and replacing text. Regular expressions can be a powerful tool for text processing and analysis, and by understanding the fundamentals of regular expressions, we can greatly expand our capabilities as Python programmers.
