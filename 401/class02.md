# TDD with Python

Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.
But Test-Driven Development is a strategy to think (and write!) tests first.

** The Cycle ** 

 this is an example of an important thing about TDD: the cycle.
The cycle is made by three steps:

* 🆘 Write a unit test and make it fail (it needs to fail because the feature isn’t there, right? If this test passes, call the Ghostbusters, really)
* ✅ Write the feature and make the test pass! (you can dance after that)
* 🔵 Refactor the code — the first version doesn’t need to be the beautiful one (don’t be shy)


# if __name__ == “__main__”:

Before executing code, Python interpreter reads source file and define few special variables/global variables.  

if the executing file is the main the variable name will set as main value and the code of if statment will be executing .

but if the moudle was secondary and imported by onther moudle ,
the if statment will get false and the code will not implemnt  .

the code which is written outside any scope will implemnt at the two cases .


# Recursion :


The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. 

<br>

### What is the difference between direct and indirect recursion? 
A function fun is called direct recursive if it calls the same function fun. A function fun is called indirect recursive if it calls another function say fun_new and fun_new calls fun directly or indirectly. Difference between direct and indirect recursion has been illustrated in Table 1. 

**  //  An example of direct recursion** 

         void directRecFun()
          {
            // Some code....

            directRecFun();

           // Some code...
          }



  
  ** // An example of indirect recursion **

            void indirectRecFun1()
            {
            // Some code...

            indirectRecFun2();

            // Some code...
            }
            void indirectRecFun2()
            {
            // Some code...

            indirectRecFun1();

            // Some code...
            }


  ### What is difference between tailed and non-tailed recursion? 
A recursive function is tail recursive when recursive call is the last thing executed by the function.


[referance](https://www.geeksforgeeks.org/recursion/)