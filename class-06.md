<<<<<<< HEAD
# HTML Tables :


***HTML tables allow web developers to arrange data into rows and columns.*** 

### Define an HTML Table:

The ** <table> ** tag defines an HTML table.

Each table row is defined with a **<tr> **tag. Each table header is defined with a <th> tag. Each table data/cell is defined with a** <td>** tag.

By default, the text in** <th> **elements are bold and centered.

By default, the text in **<td> **elements are regular and left-aligned.

#### ** Example**:   
A simple HTML table:

      <table style="width:100%">
      <tr>
          <th>Firstname</th>
        <th>Lastname</th>
        <th>Age</th>
      </tr>
       <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
      </tr>
       <tr>
         <td>Eve</td>
          <td>Jackson</td>
          <td>94</td>
         </tr>
    </table>

 ![img](https://cdn.educba.com/academy/wp-content/uploads/2019/10/Create-Tables-in-HTML.png) 

**HTML Table - Add a Border**

To add a border to a table, use the CSS border property:

     table, th, td {
      border: 1px solid black;
     }

#### HTML Table - Collapsed Borders

To let the borders collapse into one border, add the CSS border-collapse property:

**Example**

       table, th, td {
      border: 1px solid black;
       border-collapse: collapse;
      }

# JavaScript Object Methods :

The this Keyword
=======
# *** class-06 content : ***

JavaScript | 
---------|
[Object Literals]() | 
[Document Object Model](BOXES.md)      | 
[problem Domian](BOXES.md)      | 


# *** 1- Object Literals : ***

** WHAT IS AN OBJECT? **

Objects group together a set of variables and functions to create a model 
of a something you would recognize from the real world. In an object, 
variables and functions take on new names. 

 variables | Function |
---------|-------------|
if is a part of an object, it is called a property | if a function is part of an object, it is called a method|
 Properties tell us about the object,|Methods represent tasks that are associated with the object. |
such as the name of a hotel or the number of rooms it has. Each individual hotel might have a different name and a different number of rooms.   |. For example, you can check how many rooms are available by subtracting the number of booked rooms from the total number of rooms. |



 **javaScript objects are containers for named values called properties or methods.**

#### *** Example ***

     var person = {
      firstName: "John",
      lastName: "Doe",
     age: 50,
     eyeColor: "blue"
    };



Property  | Property Value
---------|-----------|
firstName|	John|
lastName	|Doe|
age	|50|
eyeColor|	blue|
fullName|	function() {return this.firstName + " " + this.lastName;}| 


** Accessing Object Properties **
* objectName.propertyName 
* objectName["propertyName"] 

### The this Keyword
>>>>>>> 249a47c51cc543bffcc31763b082cf711003d524
In a function definition, this refers to the "owner" of the function.

In the example above, this is the person object that "owns" the fullName function.

In other words, this.firstName means the firstName property of this object.

Read more about the this keyword at JS this Keyword.

<<<<<<< HEAD
Example

      const person = {
      firstName: "John",
     lastName: "Doe",
     id: 5566,
     fullName: function() {
       return this.firstName + " " + this.lastName;
     }
     };

The this Keyword
In a function definition, this refers to the "owner" of the function.

In the example above, this is the person object that "owns" the fullName function.

In other words, this.firstName means the firstName property of this object.

Read more about the this keyword at JS this Keyword.

JavaScript Methods
JavaScript methods are actions that can be performed on objects.

A JavaScript method is a property containing a function definition.




# Domain Modeling
Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

## Model epic fails videos
Imagine you've been tasked to build a program that models the popularity of epic fail videos. After months of painstaking research, you've determined that the two essential metrics for gauging popularity are an epic rating and whether or not the video has animals.

Since you'll be modeling the popularity of many types of videos—parkour epic fails, corgi epic fails, etc.—you'll want to build self-contained objects with the same attributes and behaviors. That way, when you need to change the algorithm for determining popularity, the changes will be small and targeted.



As you read this article, type out and run all code samples you come across. Do not copy and paste. Writing out and testing your code will help you remember how to implement domain models in JavaScript later.

Define a constructor and initialize properties
To define the same properties between many objects, you'll want to use a constructor function. Below is a table that summarizes a JavaScript representation of an EpicFailVideo object.

Property	|Data	|Type
--------|---------|------|
epicRating|	1 to 10	|Number|
hasAnimals|	true or false	|Boolean|


**Here's an implementation of the EpicFailVideo constructor function.**

       var EpicFailVideo = function(epicRating, hasAnimals) {
       this.epicRating = epicRating;
           this.hasAnimals = hasAnimals;
       }

         var parkourFail = new EpicFailVideo(7, false);
          var corgiFail = new EpicFailVideo(4, true);

         console.log(parkourFail);
        console.log(corgiFail);
=======

# *** 2- Document Object Model : ***

The Document Object Model (DOM) specifies 
how browsers should create a model of an HTML 
page and how JavaScript can access and update the 
contents of a web page while it is in the browser window. 

The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules. 
It is implemented by all major browser makers, and covers two primary areas:  

* MAKING A MODEL OF THE 
HTM L PAGE 
* ACCESSING AND CHANGING 
THE HTML PAGE  

### THE DOM TREE IS A MODEL OF A WEB PAGE

As a browser loads a web page, it creates a model of that page. 
The model is called a DOM tree, and it is stored in the browsers' memory. 
It consists of four main types of nodes. 

THE DOCUMENT NODE |ELEMENT NODES 
---------------------|------------------|


**Each node is an object with methods and properties. 
Scripts access and update this DOM tree (not the source HTML file). 
Any changes made to the DOM tree are reflected in the browser. ** 

### DOM TREE 
![dom tree](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5a/DOM-model.svg/1200px-DOM-model.svg.png) 



## *** WORKING WITH THE DOM TREE ***

**Accessing and updating the DOM tree involves two steps:**  

* Locate the node that represents the element you want to work with. 
* Use its text content, child elements, and attributes. 

** STEP 1: ACCESS THE ELEMENTS  **  

**STEP 2: WORK W ITH THOSE ELEMENTS** 




## *** ACCESSING ELEMENTS *** :
 
 DOM queries may return one element, or they may return a Nodelist, 
which is a collection of nodes.  
Sometimes you will just want to access one 
individual element (or a fragment of the page that 
is stored within that one element). Other times you 
may want to select a group of element s, for example, 
every <hl> element in the page or every <1 i> 
element within a particular list.  


## *** NODELISTS: DOM QUERIES THAT RETURN MORE THAN ONE ELEMENT : *** 

When a** DOM method ** can return more than one element, it returns a 
Nodelist *(even if it only finds one matching element).*  

 Nodelist is a collection of element nodes. Each 
node is given an index number (a number that starts 
at zero, just like an array). 
The order in which the element nodes are stored in a 
Node List is the same order that they appeared in the 
HTML page. 
When a DOM query returns a Nodelist, you may 
want to: 

• Select one element from the NodeList. 

• Loop through each item in the Nodelist and 
perform the same statements on each of the 
element nodes. 



[referance](file:///C:/Users/STUDENT/Downloads/Javascript_and_jquery_interactive_jon_du.pdf) 
>>>>>>> 249a47c51cc543bffcc31763b082cf711003d524
