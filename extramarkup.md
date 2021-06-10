# The Evolution of HTML:

Since the web was first created, there have 
been several different versions of HTML.

* ** HTML4** 
Released 1997
* **XHTML 1.0** 
Released 2000

* **HTML5**
Released 2000



 * Because there have been 
several versions of HTML, each 
web page should begin with a 
DOCTYPE declaration to tell a 
browser which version of HTML 
the page is using (although 
browsers usually display the 
page even if it is not included). 
We will therefore be including 
one in each example for the rest 
of the book. 

* ** HTML4**
<!DOCTYPE html PUBLIC
"-//W3C//DTD HTML 4.01 Transitional//EN"
"http://www.w3.org/TR/html4/loose.dtd">

* **HTML5** 
<!DOCTYPE html> 

* **XHTML 1.0**  
<!DOCTYPE html PUBLIC
"-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/
 xhtml1-transitional.dtd">


  * #### **  comment in HTML **:
 If you want to add a comment 
to your code that will not be 
visible in the user's browser, you 
can add the text between these 
characters:
<!-- comment goes here --> 
_
* #### ** Block Elements:** 
Some elements will always 
appear to start on a new line in 
the browser window. These are 
known as block level elements. 

**EX:**
<ul><li>Science: 21 Nov - 20 Feb 2010/11</li>
</UL>

-

* #### **Grouping Text & Elements In a Block**
The ** <div> ** element allows you to 
group a set of elements together 
in one block-level box. 

-

* #### ** Grouping Text & Elements Inline **
The ** <span> **element acts like 
an inline equivalent of the <div>
element. It is used to either:
1. Contain a section of text 
where there is no other suitable 
element to differentiate it from 
its surrounding text
2. Contain a number of inline 
elements

* ### <iframe > :
The **<iframe> **tag specifies an inline frame.

An inline frame is used to embed another document within the current** HTML **document.

**Tip:** Use CSS to style the** <iframe>**  

**Tip:** It is a good practice to always include a title attribute for the <iframe>. This is used by screen readers to read out what the content of the <iframe> is.


* **example "try it yourself":**
      <iframe 
        src="/default.asp" width="100%" height="300" style="border:1px solid black;">
         </iframe>

      <iframe src="/default.asp" width="100%" height="300"style="border:none;">
          </iframe>

