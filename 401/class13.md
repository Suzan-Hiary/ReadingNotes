## How to run Linear regression in Python scikit-Learn

You know that linear regression is a popular technique and you might as well seen the mathematical equation of linear regression. But do you know how to implement a linear regression in Python?? If so don’t read this post because this post is all about implementing linear regression in Python. There are several ways in which you can do that, you can do linear regression using numpy, scipy, stats model and sckit learn. But in this post I am going to use scikit learn to perform linear regression.

![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Prices.png)


## Linear Regression in Python
We’re living in the era of large amounts of data, powerful computers, and artificial intelligence. This is just the beginning. Data science and machine learning are driving image recognition, autonomous vehicles development, decisions in the financial and energy sectors, advances in medicine, the rise of social networks, and more. Linear regression is an important part of this.

Linear regression is one of the fundamental statistical and machine learning techniques. Whether you want to do statistics, machine learning, or scientific computing, there are good chances that you’ll need it. It’s advisable to learn it first and then proceed towards more complex methods.

 you’ll have learned:

* What linear regression is
* What linear regression is used for
* How linear regression works
* How to implement linear regression in Python, step by step


## Exploring Boston Housing Data Set

![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Explore-1.png)


This data set is available in sklearn Python module, so I will access it using scikitlearn. I am going to import Boston data set into Ipython notebook and store it in a variable called boston.
![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/sklearn.png)


The object boston is a dictionary, so you can explore the keys of this dictionary.

![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/boston-keys.png)

![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/boston-data-shape1.png)

I am going to print the feature names of boston data set.

![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/boston-features.png)

I will see the description of this data set to know more about it. In this data set I have 506 instances(rows) and 13 attributes or parameters(columns). The goal of this exercise is to predict the housing prices in boston region using the features given.
![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/boston-description.png)

![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Attribution.png)


## Scikit Learn
In this section I am going to fit a linear regression model and predict the Boston housing prices. I will use the least squares method as the way to estimate the coefficients.

Y = boston housing price(also called “target” data in Python)

and

X = all the other features (or independent variables)

First, I am going to import linear regression from sci-kit learn module. Then I am going to drop the price column as I want only the parameters as my X values. I am going to store linear regression object in a variable called lm.

![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Skitlearn-linear-model1.png)

![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/linear-regression.png)

[referance](https://bigdata-madesimple.com/how-to-run-linear-regression-in-python-scikit-learn/)
