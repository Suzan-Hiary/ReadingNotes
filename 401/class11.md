# NumPy :
 #### Data Analysis with Python





## What is NumPy ?
NumPy is a commonly used Python data analysis package. 

_ By using NumPy, you can speed up your workflow, and interface with other packages in the Python ecosystem, like scikit-learn, that use NumPy under the hood. NumPy was originally developed in the mid 2000s, and arose from an even older package called Numeric. This longevity means that almost every data analysis or machine learning package for Python leverages NumPy in some way.


### Lists Of Lists for CSV Data:

Before using NumPy, we’ll first try to work with the data using Python and the csv package. We can read in the file using the csv.reader object, which will allow us to read in and split up all the content from the ssv file.

In the below code, we:

* Import the csv library.
* Open the winequality-red.csv file.
* With the file open, create a new csv.reader object.
* Pass in the keyword argument delimiter=";" to make sure that the * * records are split up on the semicolon character instead of the default comma character.
* Call the list type to get all the rows from the file.
* Assign the result to wines.



                    import csv

                    with open('winequality-red.csv', 'r') as f:

                        wines = list(csv.reader(f, delimiter=';'))





## Numpy 2-Dimensional Arrays :

With NumPy, we work with multidimensional arrays. We’ll dive into all of the possible types of multidimensional arrays later on, but for now, we’ll focus on 2-dimensional arrays. A 2-dimensional array is also known as a matrix, and is something you should be familiar with. In fact, it’s just a different way of thinking about a list of lists. A matrix has rows and columns. By specifying a row number and a column number, we’re able to extract an element from a matrix.


![](https://www.w3resource.com/w3r_images/python-numpy-image-exercise-58.png)



## How Creating A NumPy Array ?

###  using the numpy.array function 
   If we pass in a list of lists, it will automatically create a NumPy array with the same number of rows and columns. Because we want all of the elements in the array to be float elements for easy computation


  * Import the numpy package. 

  * Pass the list of lists wines into the array function, which converts it into a NumPy array.
      * Exclude the header row with list slicing.
      * Specify the keyword argument dtype to make sure each element    is converted to a float. We’ll dive more into what the dtype      is later on.





                    import csv

                    with open("winequality-red.csv", 'r') as f:

                        wines = list(csv.reader(f, delimiter=";"))

                    import numpy as np

                    wines = np.array(wines[1:], dtype=np.float)





[referance](https://www.dataquest.io/blog/numpy-tutorial-python/)                    