# Classes and Objects

## *** Classes : ***
Classes are essentially a template to create your objects. 





## *** Objects : *** 
are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. 


 ** A very basic class would look something like this: **

                class MyClass:

                variable = "blah"

                def function(self):
                    print("This is a message inside the class.")




To assign the class to an object : 

** write ** : myobjectx = MyClass() 

* Now the variable "myobjectx" holds an object of the class "MyClass" that contains the variable and the function defined within the class called "MyClass".

### Accessing Object Variables 

To access the variable inside of the newly created object "myobjectx"

you can use the dot notation 

** myobjectx.variable **

You can create multiple different objects that are of the same class(have the same variables and functions defined). However, each object contains independent copies of the variables defined in the class.


### Accessing Object Functions 

To access a function inside of an object you use notation similar to accessing a variable:

** myobjectx.function() **

## Thinking Recursively in Python :

Problems can often seem big and scary. But if we keep chipping away at them, more often than not we can break them down into smaller chunks trivial enough to solve.


#### Recursive Functions in Python :

A recursive function is a function defined in terms of itself via self-referential expressions. 
When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either:

Thread the state through each recursive call so that the current state is part of the current call’s execution context
Keep the state in global scope


## Python Testing with pytest: Fixtures and Coverage 

a library for testing Python code . pytest has become quite popular, in no small part because it's so easy to write tests and integrate those tests into your software development process.


** Fixtures **

When you're writing tests, you're rarely going to write just one or two. Rather, you're going to write an entire "test suite", with each test aiming to check a different path through your code. In many cases, this means you'll have a few tests with similar characteristics, something that pytest handles with "parametrized tests".

[referance](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)
