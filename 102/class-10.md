# **  Error Handling & Debugging : ** 

JavaScript can be hard to learn and everyone makes 
mistakes when writing it. this reading notes will explain and  show you how to find the errors in your code. It will also teach you how 
to write scripts that deal with potential errors gracefully. 


When writing a long script, nobody gets everything right in their first attempt. The error 
messages that a browser gives look cryptic at first, but they can help you determine what 
went wrong in your JavaScript and how to fix it. In this chapter you will learn about:  

## ** ORDER OF EXECUTION:**


To find the source of an error, it helps to know how scripts are processed. 
The order in which statements are executed can be complex; some tasks 
cannot complete until another statement or function has been run: 

![](https://www.oreilly.com/library/view/javascript-and-jquery/9781118531648/images/p452-001.jpg)


This script above creates a greeting message, then 
writes it to an alert box (see right-hand page). In 
order to create that greeting, two functions are used: 
greetUser () and getName () . 
You might think that the order of execution (the 
order in which statements are processed) would be 
as numbered: one through to four. However, it is a 
little more complicated. 
To complete step one, the interpreter needs the 
results of the functions in steps two and three 
(because the message contains values returned by 
those functions). The order of execution is more like 
this: 1, 2, 3, 2, 1, 4.  

** 1. The greeting variable gets its value from the 
greetUser() function. **

** 2. greetUser() creates the message by combining 
the string 'He 11 o ' with the result of getName (). **

** 3. getName () returns the name to greetUser(). **

** 2. greetUser() now knows the name, and combines 
it with the string. It then returns the message to the 
statement that called it in step 1. **

**1. The value of the greeting is stored in memory. **

**4. This greeting variable is written to an alert box. **





## ** EXECUTION CONTEXTS **

The JavaScript interpreter uses the concept of execution contexts. 
There is one global execution context; plus, each function creates a new 
new execution context. They correspond to variable scope.  

** GLOBAL CONTEXT **
Code that is in the script, but not in a function. 
There is only one global context in any page.  

** FUNCTION CONTEXT **
Code that is being run within a function. 
Each function has its own function context. 

EVAL CONTEXT (NOT SHOWN) 
Text is executed like code in an internal function 
called eva l {) (which is not covered in this book).


** VARIABLE SCOPE **

The first two execution contexts correspond with the 
notion of scope (which you met on p98): 
Q GLOBAL SCOPE 
If a variable is declared outside a function, it can 
be used anywhere because it has global scope. 
If you do not use the var keyword when creating 
a variable, it is placed in global scope. 
FUNCTION-LEVEL SCOPE 
When a variable is declared within a function, 
it can only be used within that function. This is 
because it has function-level scope. 


## EXECUTION CONTEXT & HOISTING :

Each time a script enters a new execution context, there are two phases 
of activity:

** 1: PREPARE **

• The new scope is created 

• Variables, functions, and arguments are created 

• The value of the this keyword is determined  


** 2: EXECUTE **

• Now it can assign values to variables 

• Reference functions and run their code 

• Execute statements

## ** UNDERSTANDING SCOPE ** 


![](https://dmitripavlutin.com/static/0e8cc3fa4620de81448ac019ae55208b/05127/javascript-scope-cover-2.png)


In the interpreter, each execution context has its own va ri ables object. 
It holds the variables, functions, and parameters available within it. 
Each execution context can also access its parent's v a ri ables object. 


Functions in JavaScript are said to have lexical scope. 
They are linked to the object they were defined within. 
So, for each execution context, the scope is the 
current execution context's variables object, plus the 
variables object for each parent execution context 


### UNDERSTANDING ERRORS :

If a JavaScript statement generates an error, then it throws an exception. 
At that point, the interpreter stops and looks for exception-handl ing code. 
If you are anticipating that something in your code 
may cause an error, you can use a set of statements 
to handle the error (you meet them on p480). 
This is important because if the error is not handled, 
the script will just stop processing and the user will 
not know why. So exception-handling code should 
inform users when there is a problem

## ERROR OBJECTS :


Error objects can help you find where your mistakes are 
and browsers have tools to help you read them.  

     Syntax Error 
     SYNTAX IS NOT CORRECT 

    This is caused by incorrect use of the rules of the 
    language. It is often the result of a simple typo



 ### HOW TO DEAL WITH ERROR
   Now that you know what an error is and how the browser treats them, there are two things you can do with the errors. 

**1: DEBUG THE SCRIPT TO FIX ERRORS **
If you come across an error while writing a script 
(or when someone reports a bug), you will need to 
debug the code, track down the source of the error, 
and fix it. 
You will find that the developer tools available in 
every major modern browser will help you with 
this task. In this chapter, you will learn about the 
developer tools in Chrome and Firefox. (The tools in 
Chrome are identical to those in Opera.) 
IE and Safari also have their own tools (but there is 
not space to cover them all).  


*** 2: HANDLE ERRORS GRACEFULLY **
You can handle errors gracefully using try, catch, 
throw, and f i na 1 ly statements. 
Sometimes, an error may occur in the script for a 
reason beyond your control. For example, you might 
request data from a third party, and their server 
may not respond. In such cases, it is particularly 
important to write error-handling code. 
In the latter part of the chapter, you will learn how to 
gracefully check whether something will work, and 
offer an alternative option if it fails. 


