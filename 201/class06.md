# read06

## Understanding the problem domain is the hardest part of programming

Writing code is a lot like putting together a jigsaw puzzle.  We put together code with the purpose of building components that we have taken out of the “bigger picture” of the problem domain.

The big issue is that many problem domains are like a puzzle with a blurry picture or no picture at all.

As programmers, we also are often not given complete information about the problem domain, so we don’t even have the information we need to understand it.

**Programming is easy if you understand the problem domain**

* Make the problem domain easier

You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.

What I mean by this is that it is often beneficial to take a part of the problem and fully understand that part before expanding the problem domain.



* Get better at understanding the problem domain

make sure you understand a problem inside and out before you try and solve it with code. 



## Chapter 3: “Object Literals” (pp.100-105)

**function declaration** creates a function that you 
can call later in your code. It is the type of function 
you have seen so far in this book. 
In order to call the function later in your code, you 
must give it a name, so these are known as **named functions**  B

If you put a function where the interpreter would 
expect to see an expression, then it is treated as an 
expression, and it is known as a **function expression.**

**In function expressions,**  the name is usually omitted. 
A function with no name is called an **anonymous function.**


When a variable is created inside a function using the 
var keyword, it can only be used in that function. 
It is called a **local variable or function-level variable.**
It is said to have local scope or function-level scope. 
It cannot be accessed outside of the function in 
which it was declared. 


If you create a variable outside of a function, then it 
can be used anywhere within the script. It is called a 
**global variable and has global scope.** 


## Chapter 5: “Document Object Model” (pp.183-242)

The key difference between 
a **whi 1 e loop** and a **do whi 1 e loop** is that the statements in 
the code block come before the 
condition. This means that those 
statements are run once whether 
or not the condition is met. 


**ACCESS THE ELEMENTS**

Here is an overview of the methods and properties that access elements 

* Here are three common ways to 

* select an individual element: 

Uses the value of an element's 
id attribute (which should be 
unique within the page). 


* Uses a CSS selector, and returns 
the first matching element. 

* You can also select individual 
elements by traversing from one 
element to another within the 
DOM tree (see third column). 

* There are three common ways to 
select multiple elements. 

* getElementsByClassName() 
Selects all elements that have 
a specific value for their cl ass 
attribute. 

* getElementsByTagName() 
Selects all elements that have the 
specified tag name .. 

* querySelectorAll() 
Uses a CSS selector to select all 
matching elements. 

**get El ementByi d ()** allows you 
to select a single element node 
by specifying the value of its 
id attribute. 


This method has **one parameter:**
the value of the id attribute on 
the element you want to select. 
This value is placed inside quote 
marks because it is a string. The 
quotes can be single or double 
quotes, but they must match. 

The code then uses a property 
called **cl assName**  to update the 
value of the cl ass attribute 
of the element stored in this 
variable. Its value is coo 1, and 
this triggers a new rule in the 
CSS that sets the background 
color of the element to aqua. 
Note how the c 1 assName 
property is used on the variable 
that stores the reference to the 
element. 



* This property finds the element 
node for the containing (or 
parent) element in the HTML. 
(1) If you started with the 
first <l i >element, then its 
parent node would be the one 
representing the <ul >element. 


* These properties find the 
previous or next sibling of a node 
if there are siblings. 
If you started with the first <1 i > 
element, it would not have a 
previous sibling. However, its next 
sibling (2) would be the node 
representing the second <l i >. 


* lastChild 
These properties find the first or 
last child of the current element. 
If you started with the <u 1 > 
element, the first child would be 
the node representing the first 
<l i> element, and (3) the last 
child would be the last <1 i >.


**STORE THE ELEMENT**

TO BE REMOVED IN A 
VARIABLE 
You start by selecting the 
element that is going to be 
removed and store that element 
node in a variable. 

When you remove an element 
from the DOM, it will also 
remove any child elements. 

**STORE THE PARENT OF THAT ELEMENT IN A VARIABLE**

 you find the parent element 
that contains the element you 
want to remove and store that 
element node in a variable. 
The simplest way to get this 
element is to use the parentNode 
property of this element. 


**REMOVE THE ELEMENT FROM ITS CONTA INING ELEMENT**

The removeChi ld() method is 
used on the containing element 
that you selected in step 2. 
The removeChi ld() method 
takes one parameter: the 
reference to the element that 
you no longer want.