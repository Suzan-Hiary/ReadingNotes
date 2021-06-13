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
In a function definition, this refers to the "owner" of the function.

In the example above, this is the person object that "owns" the fullName function.

In other words, this.firstName means the firstName property of this object.

Read more about the this keyword at JS this Keyword.

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
