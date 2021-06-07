# CSS Box Model:
In CSS, the term "box model" is used when talking about design and layout.

The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. The image below illustrates the box model:

![boxes](https://complete-concrete-concise.com/wp-content/uploads/2018/04/17-css-flow.png)


* **Content - **The content of the box, where text and images appear
* **Padding - **Clears an area around the content. The padding is transparent
* ** Border -** A border that goes around the padding and content
* **Margin -**  Clears an area outside the border. The margin is transparent.


** Example**   

Demonstration of the box model: 

    div {
     width: 300px;
     border: 15px solid green;
     padding: 50px;
     margin: 20px;
     }


### Width and Height of an Element:
In order to set the width and height of an element correctly in all browsers, you need to know how the box model works. 




    div {
     width: 320px;
     padding: 10px;
     border: 5px solid gray;
     margin: 0;
     }



[referance](https://www.w3schools.com/css/css_boxmodel.asp) 