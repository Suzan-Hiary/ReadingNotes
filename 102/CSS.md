# Introducing CSS:

## **What is CSS?**
* CSS stands for Cascading Style Sheets
* CSS describes how HTML elements are to be displayed on screen, paper, or in other media
* CSS saves a lot of work. It can control the layout of multiple web pages all at once
* External stylesheets are stored in CSS files 

## ** Why Use CSS? **
CSS is used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.

## CSS Solved a Big Problem
HTML was NEVER intended to contain tags for formatting a web page!

HTML was created to describe the content of a web page, like:

<h1>This is a heading</h1>

<p>This is a paragraph.</p>

When tags like <font>, and color attributes were added to the HTML 3.2 specification, it started a nightmare for web developers. Development of large websites, where fonts and color information were added to every single page, became a long and expensive process.

To solve this problem, the World Wide Web Consortium (W3C) created CSS.

CSS removed the style formatting from the HTML page! 

![CSS LOGO](https://armyyazilim.com/wp-content/uploads/2019/10/css.png)

** EX: ** Here you can see a simple web page that is 
styled using CSS.

    <!DOCTYPE html>

    <html>
    <head>
     <title>Introducing CSS</title>
     <link href="css/example.css" type="text/css" 
     rel="stylesheet" />
    </head>

    <body>

     <h1>From Garden to Plate</h1>

     <p>
     A <i>potager</i> is a French term for an 
     ornamental vegetable or kitchen garden ...
      </p>
     <h2>What to Plant</h2>

     <p>Plants are chosen as much for their functionality 
        as for their color and form ... </p>

     </body>

     </html>

      body {
      font-family: Arial, Verdana, sans-serif;
      }
       h1, h2 {
     color: #ee3e80;}
     p {
          color: #665544;}








## Using External CSS:

**<link>**


The **<link>** element can be used 
in an HTML document to tell the 
browser where to find the CSS 
file used to style the page. It is an 
empty element (meaning it does 
not need a closing tag), and it 
lives inside the <head> element. 
It should use three attributes:

* **href**

This specifies the path to the 
CSS file (which is often placed in 
a folder called css or styles).

* **type**

This attribute specifies the type 
of document being linked to. The 
value should be text/css.

* **rel**

This specifies the relationship 
between the HTML page and 
the file it is linked to. The value 
should be stylesheet when 
linking to a CSS file.
An HTML page can use more 
than one CSS style sheet. To 
do this it could have a <link>
element for every CSS file it 
uses. For example, some authors 
use one CSS file to control the 
presentation (such as fonts and 
colors) and a second to control 
the layout.





CSS describes how HTML elements should be displayed.

** This tutorial will teach you CSS from basic to advanced.**


- CSS stands for Cascading Style Sheets
- CSS describes how HTML elements are to be displayed on - screen, paper, or in other media
- CSS saves a lot of work. It can control the layout of 
- multiple web pages all at once
- External stylesheets are stored in CSS files.

## CSS Syntax :

CSS is a rule-based language — you define rules specifying groups of styles that should be applied to particular elements or groups of elements on your web page. For example "I want the main heading on my page to be shown as large red text." 

### CSS Selectors :

Selector |	Example |	Example description
------|------|-------
#id	|#firstname	|Selects the element with id="firstname"
.class|	.intro|	Selects all elements with class="intro"
element.class|	p.intro|	Selects only <p> elements with class="intro"
*	|*|	Selects all elements
element	|p|	Selects all <p> elements
element,element,..|	div, p|	Selects all <div> elements and all <p> elements.


## How To Add CSS :
#### Three Ways to Insert CSS


* External CSS
* Internal CSS
* Inline CSS

## CSS Color Names:

* Tomato
* Orange
* DodgerBlue
* MediumSeaGreen
* Gray
* SlateBlue
* Violet
* LightGray


 ### [FOR MORE COLOR "colorhunt"  ](https://colorhunt.co/)