## Random Module in Python :

The random module provides access to functions that support many operations. Perhaps the most important thing is that it allows you to generate random numbers. 


### When to use it? 

We want the computer to pick a random number in a given range Pick a random element from a list, pick a random card from a deck, flip a coin etc. When making your password database more secure or powering a random page feature of your website.


### Random functions
The Random module contains some very useful functions.
Randint
If we wanted a random integer, we can use the randint function Randint accepts two parameters: a lowest and a highest number. Generate integers between 1,5. The first value should be less than the second.

import random
print random.randint(0, 5)
This will output either 1, 2, 3, 4 or 

# Risk Analysis :

In any software, using risk analysis at the beginning of a project highlights the potential problem areas. After knowing about the risk areas, it helps the developers and managers to mitigate the risks. When a test plan has been created, risks involved in testing the product are to be taken into consideration along with the possibility of the damage they may cause to your software along with solutions.

### risks that are unavoidable 

* The time that you allocated for testing

* A defect leakage due to the complexity or size of the application

* Urgency from the clients to deliver the project

* Incomplete requirements

### Risk Identification
There are different sets of risks included in the risk identification process. Those are as follows:

* Business Risks: This risk is the most common risk associated with our topic. It is the risk that may come from your company or your customer, not from your project.

* Testing Risks: You should be well acquainted with the platform you are working on, along with the software testing tools being used.

* Preature Release Risk: a fair amount of knowledge to analyze the risk associated with releasing unsatisfactory or untested software is required

* Software Risks: You should be well versed with the risks associated with the software development process.


### Risk Assessment
In the risk analysis process, these steps prove to be the most important one. It is said that this step is way too complex and should be tackled with the utmost care. After risk identification, assessment has to be dealt programmatically. There are a few perspectives on risk assessment. Read on!

The perspective of Risk Assessment
There are three perspectives of Risk Assessment:

Effect

Cause

Likelihood


## TestCoverage 

Test coverage is a useful tool for finding untested parts of a codebase. Test coverage is of little use as a numeric statement of how good your tests are.

Like most aspects of programming, testing requires thoughtfulness. TDD is a very useful, but certainly not sufficient, tool to help you get good tests. If you are testing thoughtfully and well, I would expect a coverage percentage in the upper 80s or 90s. I would be suspicious of anything like 100% - it would smell of someone writing tests to make the coverage numbers happy, but not thinking about what they are doing.


[refeerance](https://martinfowler.com/bliki/TestCoverage.html)