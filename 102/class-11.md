
=======
# HTML & CSS:

* [** HTML Images **]()
* [** Practical Information **](CSS.md)





## ** HTML Images ** :

Controlling the size and alignment of
your images using CSS keeps rules that
affect the presentation of your page in
the CSS and out of the HTML markup. 

![](https://static.javatpoint.com/htmlpages/images/html-image.png)


## 1- Controlling sizes ofimages in CSS :

You can control the size of an
image using the width and
height properties in CSS, just
like you can for any other box.  

       img.large {
           width: 500px;
           height: 500px;}

        img.medium {
           width: 250px;
           height: 250px;}

        img.small {
           width: 100px;
           height: 100px;}



## ** Aligining images : **

Rather than using the **<img>**
element's align attribute, web
page authors are increasingly
using the float property to align
images. There are two ways that
this is commonly achieved:

* 1: The float property is added
to the class that was created to
represent the size of the image


* 2: New classes are created with
names such as align-left or
align-right to align the images
to the left or right of the page.
These class names are used in
addition to classes that indicate
the size of the image. 


      img.align-left {
         float: left;
        margin-right: 10px;} 

     img.align-right {
        float: right;
        margin-left: 10px;}

     img.medium {
         width: 250px;
         height: 250px;}


## ** Centering images Using CSS :**


By default, images are inline
elements. This means that they
flow within the surrounding text.
In order to center an image, it
should be turned into a blocklevel element using the display
property with a value of block.  



     img.align-center {
            display: block;
            margin: 0px auto;}

     img.medium {
           width: 250px;
            height: 250px; }




  ## ** Background Images **
** (background-image) **

The background-image
property allows you to place
an image behind any HTML
element. This could be the entire
page or just part of the page. By
default, a background image will
repeat to fill the entire box.


        body {
                 background-image: url("images/pattern.gif");}




## ** Repeating Images **

* background-repeat
* background-attachment


### repeat 
The background image is
repeated both horizontally and
vertically (the default way it
is shown if the backgroundrepeat property isn't used).

 **1. repeat-x **

The image is repeated
horizontally only (as shown in
the first example on the left). 

** 2. repeat-y **

The image is repeated vertically
only 

** 3. no-repeat **

The image is only shown once.


** The background-attachment** 

property specifies whether a
background image should stay in
one position or move as the user
scrolls up and down the page. It
can have one of two values: 

* ** fixed **

The background image stays in
the same position on the page.

* **scroll**

The background image moves
up and down as the user scrolls
up and down the page


            body {
                    background-image: url("images/tulip.gif");
                    background-repeat: no-repeat;
                    background-attachment: fixed;}


## ** Background Position **
( background-position )

When an image is not being
repeated, you can use the
background-position
property to specify where in the
browser window the background
image should be placed.
This property usually has a pair
of values. The first represents
the horizontal position and the
second represents the vertical 


![](https://i.pinimg.com/originals/a9/84/0a/a9840a7ddb1d028748759e8c47c5796f.gif)


If you only specify one value,
the second value will default to
center.
You can also use a pair of pixels
or percentages. These represent
the distance from the top left
corner of the browser window
(or containing box). The top left
corner is equal to 0% 0%. The
example shown, with values of
50% 50%, centers the image 


## shorthand background :

The background property acts
like a shorthand for all of the
other background properties
you have just seen, and also the
background-color property.




             div {
                  background:
                          url(example-1.jpg)
                          top left no-repeat,
                          url(example-2.jpg)
                          bottom left no-repeat,
                          url(example-3.jpg)
                          centre top repeat-x;}



## ** Image Rollovers& Sprites **:

Using CSS, it is possible to create
a link or button that changes to a
second style when a user moves
their mouse over it (known as a
rollover) and a third style when
they click on it.
This is achieved by setting a
background image for the link or
button that has three different
styles of the same button (but
only allows enough space to
show one of them at a time).
You can see the image we are
using in this example on the
right. It actually features two
buttons on the one image.
When the user moves their
mouse over the element, or
clicks on it, the position of the
background image is moved to
show the relevant image.
When a single image is used
for several different parts of an
interface, it is known as a sprite.
You can add the logo and other
interface elements, as well as
buttons to the image.
The advantage of using sprites is
that the web browser only needs
to request one image rather than
many images, which can make
the web page load faster.


        a.button {
              height: 36px;
              background-image: url("images/button-sprite.jpg");
              text-indent: -9999px;
              display: inline-block;}

         a#add-to-basket {
              width: 174px;
             background-position: 0px 0px;}

       a#framing-options {
             width: 210px;
            background-position: -175px 0px;}

       a#add-to-basket:hover {
            background-position: 0px -40px;}

       a#framing-options:hover {
             background-position: -175px -40px;}

       a#add-to-basket:active {
             background-position: 0px -80px;}

       a#framing-options:active {
             background-position: -175px -80px;}



             Because the <a> element is
an inline element, we set the
display property of these links
to indicate that they should be
inline-block elements. This
allows us to specify the width
and height of each <a> element
so that it matches the size of its
corresponding button.  


[Reference ^^ ](file:///C:/Users/STUDENT/Downloads/duckett_html.pdf)
>>>>>>> cd19879cbc72007f8efc6c8ca194ca0f6ff83ffe
