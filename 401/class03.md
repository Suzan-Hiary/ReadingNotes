# Reading and Writing Files in Python

one of common tasks we can do it in python is reading and writing files.


### open : 
When you want to work with a file, the first thing to do is to open it. This is done by invoking the ** open() ** built-in function. ** open() ** has a single required argument that is the path to the file.


you open the file using the file name and extended 

example :

               file = open('dog_breeds.txt') 


the ** open() ** method take a seconed parameter which is optionaly there is many option to select what you want to do with the opened file such as :

* r : for reading 
* w : for writing 
* b : for binary  
* a : for append 


also you can use two things with each other "wb" write and binary " the file.

## The Reading method :

* ** .readlines() : ** This reads the remaining lines from the file object and returns them as a list.

* ** .readline(size=-1) ** : This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read.
* ** .read(size=-1) ** : This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read.

## The write methods : 
* ** .write(string) ** :This writes the string to the file. 
* ** .writelines(seq) ** : This writes the sequence to the file. No line endings are appended to each sequence item. It’s up to you to add the appropriate line ending(s). 


## Close () the file :

You should always make sure that an open file is properly closed.
It’s important to remember that it’s your responsibility to close the file. In most cases, upon termination of an application or script, a file will be closed eventually. However, there is no guarantee when exactly that will happen. This can lead to unwanted behavior including resource leaks. It’s also a best practice within Python (Pythonic) to make sure that your code behaves in a way that is well defined and reduces any unwanted behavior.

 example:
                   reader = open('dog_breeds.txt')
                       try:
                   # Further file processing goes here
                   finally:
                    reader.close()   

               

 # Python Exceptions          : 

 A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception.

## **  Exceptions versus Syntax Errors **    

Syntax errors occur when the parser detects an incorrect statement. 
This time, you ran into an exception error. This type of error occurs whenever syntactically correct Python code results in an error. The last line of the message indicated what type of exception error you ran into.

example:

           >>> print( 0 / 0 ))
  
            File "<stdin>", line 1
            print( 0 / 0 ))
                  ^
            SyntaxError: invalid syntax




## ** Raising an Exception ** :
We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.

If you want to throw an error when a certain condition occurs using raise, you could go about it like this:

                    x = 10
                     if x > 5:
                 raise Exception('x should not exceed 5. 
                  The value of x was: {}'.format(x))



## The AssertionError Exception :

Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError exception.



[refernce](https://realpython.com/python-exceptions/)