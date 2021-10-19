## List Comprehensions : 

1_ ** Syntax ** 

my_new_list = [ expression for item in list ] 

List comprehension methods are an elegant way to create and manage lists. 
In Python, list comprehensions are a more compact way of creating lists. 
More flexible than for loops, list comprehension is usually faster than other methods.


## Create a List Using Loops and List Comprehension in Python :

To better illustrate how a list comprehension can be used to write more efficient Python code, we’ll take a look at a side by side comparison. 

In the following example, you’ll see two different techniques for creating a Python list. The first is a for loop. We’ll use it to construct a list of the powers of two.


## Create a List with range() :

Let’s start by creating a list of numbers using Python list comprehensions. We’ll take advantage of Python’s range() method as a way to create a list of digits.


You are here: Home / Basics / List Comprehensions in Python
List Comprehensions in Python
Author: Josh Petty
Last Updated: August 30, 2021

Table of Contents
Syntax
Create a List with range()
Create a List Using Loops and List Comprehension in Python
Multiplying Parts of a List
Show the first letter of each word using Python
Lower/Upper case converter using Python
Print numbers only from a given string
Parsing a file using list comprehension
Using functions in list comprehensions
In conclusion
Related Posts
Chances are you’ll use a lot of lists as a Python programmer. While we’re all big fans of for loops (and nested for loops), Python provides a more concise method for handling lists and list comprehension. 

In order to keep your code elegant and readable, it’s recommended that you use Python’s comprehension features.


 
List comprehension is a powerful and concise method for creating lists in Python that becomes essential the more you work with lists, and lists of lists.


## Syntax
Consider the following example:

my_new_list = [ expression for item in list ]

You can see from this example that three ingredients are necessary for a python list comprehension to work.

First is the expression we’d like to carry out. expression inside the square brackets.
Second is the object that the expression will work on. item inside the square brackets.
Finally, we need an iterable list of objects to build our new list from. list inside the square brackets.
To understand the list comprehension, imagine it like this: you’re going to perform an expression on each item in the list. The expression will determine what item is eventually stored in the output list. 

Not only can you perform expressions on an entire list in a single line of code, but, as we’ll see later, it’s possible to add conditional statements in the form of filters, which allows for more precision in the way lists are handled.

Notes about Lists Comprehensions
List comprehension methods are an elegant way to create and manage lists. 
In Python, list comprehensions are a more compact way of creating lists. 
More flexible than for loops, list comprehension is usually faster than other methods.
Create a List with range()
Let’s start by creating a list of numbers using Python list comprehensions. We’ll take advantage of Python’s range() method as a way to create a list of digits.



 
# construct a basic list using range() and list comprehensions
### syntax
####  [ expression for item in list ]
                digits = [x for x in range(10)]

                print(digits)
                Output

                [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

[referance](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)