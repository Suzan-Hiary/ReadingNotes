# USING HTML5 STORAGE :

## What is HTML Web Storage?
With web storage, web applications can store data locally within the user's browser.

Before HTML5, application data had to be stored in cookies, included in every server request. Web storage is more secure, and large amounts of data can be stored locally, without affecting website performance.

Unlike cookies, the storage limit is far larger (at least 5MB) and information is never transferred to the server.

Web storage is per origin (per domain and protocol). All pages, from one origin, can store and access the same data.
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype. 

    interface Storage {
    getter any getItem(in DOMString key);
    setter creator void setItem(in DOMString key, in any data);
    };

![](https://theburningmonk.com/wp-content/uploads/2010/12/image42.png)
Calling setItem() with a named key that already exists will silently overwrite the previous value. Calling getItem() with a non-existent key will return null rather than throw an exception.

Like other JavaScript objects, you can treat the localStorage object as an associative array. Instead of using the getItem() and setItem() methods, you can simply use square brackets. For example, this snippet of code:

## The localStorage Object
The localStorage object stores the data with no expiration date. The data will not be deleted when the browser is closed, and will be available the next day, week, or year.

      // Store
        localStorage.setItem("lastname", "Smith");

      // Retrieve
           document.getElementById("result").innerHTML = localStorage.getItem("lastname");


           Example explained:

Create a localStorage name/value pair with name="lastname" and value="Smith"
Retrieve the value of "lastname" and insert it into the element with id="result"


The example above could also be written like this:

          // Store
               localStorage.lastname = "Smith";
          // Retrieve
               document.getElementById("result").innerHTML = localStorage.lastname;

![](https://academy.hsoub.com/uploads/monthly_2016_07/html5-local-storage.png.6cd0e4e6aedf627d353a5bd3cf9795bf.png)


  ## TRACKING CHANGES TO THE HTML5 STORAGE AREA
If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. For example, if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.

The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8. IE 8 does not support the W3C standard addEventListener (although that will finally be added in IE 9). Therefore, to hook the storage event, you’ll need to check which event mechanism the browser supports. (If you’ve done this before with other events, you can skip to the end of this section. Trapping the storage event works the same as every other event you’ve ever trapped. If you prefer to use jQuery or some other JavaScript library to register your event handlers, you can do that with the storage event, too.)

[referance](https://www.w3schools.com/html/html5_webstorage.asp)