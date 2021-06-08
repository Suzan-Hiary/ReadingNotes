# class-04 content :

* [** HTML links **](class-04.md)
* [** Layout **]()
* [** function**]()
* [** Reasons for Pair Programming **]()

+ ## HTML links: 

Links are created using the <a> element. Users can click on anything 
between the opening <a> tag and the closing </a> tag. You specify 
which page you want to link to using the href attribute.

** There are many ways to linking ** :

** 1- if you want to Linking to Other Sites **

      <a href="http://www.empireonline.com">
      Empire</a><


** 2- if you want to Linking to Other Pages 
on the Same Site ** 


    <a href="index.html">Home</a>


** 3-Email Links** 

    <a href="mailto:jon@example.org">Email Jon</a>
** 4-pening Links ina New Window**


    <a href="http://www.imdb.com" target="_blank">
    Internet Movie Database</a> (opens in new window)

** 5-Linking to a SpecificPart of the Same Page **

     <a href="#arc_shot">Arc Shot</a>


  ## ** Layout **:

  Website Layout
A website is often divided into headers, menus, content and a footer.

 The float property moves content to the left or right 
of the page and can be used to create multi-column 
layouts. (Floated items require a defined width.)

![img](https://miro.medium.com/max/1024/1*XCZZZmhQN4rHLw2dW14BZQ.png)

* ** Pages can be fixed width or liquid (stretchy) layouts **

**  Browsers display pages in normal flow unless you 
specify relative, absolute, or fixed positioning.**

** esigners keep pages within 960-1000 pixels wide, 
and indicate what the site is about within the top 600 
pixels (to demonstrate its relevance without scrolling).
Grids help create professional and flexible designs.
CSS Frameworks provide rules for common tasks.
 You can include multiple CSS files in one page.**


# ** function** :

## WHAT IS A FUNCTION?
Functions let you group a series of statements together to perform a 
specific task. If different parts of a script repeat the same task, you can 
reuse the function (rather than repeating the same set of statements). 


### ** ANONYMOUS FUNCTIONS & FUNCTION EXPRESSIONS ** :


Expressions produce a value. They can be used where values are expected. 
If a function is placed where a browser expects to see an expression, 
(e.g., as an argument to a function), then it gets treated as an expression. 

**FUNCTION DECLARATION** 
A function declaration creates a function that you 
can call later in your code. It is the type of function 
you have seen so far in this book. 
In order to call the function later in your code, you 
must give it a name, so these are known as named 
functions. Below, a function called area() is 
declared, which can then be called using its name. 

      function area (width, height) 
        return width * height; 
       }; 
         var size= area (3, 4) ; 

**FUNCTION EXPRESSION** 
If you put a function where the interpreter would 
expect to see an expression, then it is treated as an 
expression, and it is known as a function expression. 
In function expressions, the name is usually omitted. 
A function with no name is called an anonymous 
function. Below, the function is stored in a variable 
called area. It can be called like any function created 
with a function declaration. 

     var ar ea = f unction(width, height) { 
        r eturn width * height; 
     } ; 
           var size = area (3, 4) ; 


### IMMEDIATELY INVOKED FUNCTION EXPRESSIONS :
This way of writing a function is used in several different situations. 
Often functions are used to ensure that the variable names do not conflict 
with each other (especially if the page uses more than one script). 


+ ## ** Reasons for Pair Programming**


### ** How does pair programming work?**
While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.


### ** Why pair program?**
While learning to code, developers likely study several programming languages. Similar to a foreign language class, there are four fundamental skills that help anyone learn a new language: Listening: hearing and interpreting the vocabulary Speaking: using the correct words to communicate an idea Reading: understanding what written language intends to convey Writing: producing from scratch a meaningful

1. Greater efficiency 
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness 

[reference](https://www.codefellows.org/blog/6-reasons-for-pair-programming/) 
