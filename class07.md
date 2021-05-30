# class 07 
## Domain Modeling

Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as  **an object-oriented model**


* To define the same properties between many objects, you'll want to use a constructor function.

* Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

*Here's some tips to follow when building your own domain models.

* When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
* Model its attributes with a constructor function that defines and initializes properties.
* Model its behaviors with small methods that focus on doing one job well.
* Create instances using the new keyword followed by a call to a constructor function.
* Store the newly created object in a variable so you can access its properties and methods from outside.
* Use the this variable within methods so you can access the object's properties and methods from inside.


## Chapter 6: “Tables” (pp.126-145)

**The <img> element is used to add images to a web page**

* You must always specify a src attribute to indicate the 
source of an image and an alt attribute to describe the 
content of an image.
* You should save images at the size you will be using 
them on the web page and in the appropriate format.
* Photographs are best saved as JPEGs; illustrations or 
logos that use flat colors are better saved as GIFs


**The <table> element is used to add tables to a web page.**

*  A table is drawn out row by row. Each row is created 
with the <tr> element.
* Inside each row there are a number of cells 
represented by the <td> element (or <th> if it is a 
header).
* You can make cells of a table span more than one row 
or column using the rowspan and colspan attributes.
* For long tables you can split the table into a <thead>, 
<tbody>, and <tfoot>


## Chapter 3: “Functions, Methods, and Objects” (pp.106-144)

* BROWSER OBJECT MODEL 
The Browser Object Model contains 
objects that represent the current 
browser window or tab. It contains 
objects that model things like 
browser history and the 
device's screen.  
 
* GLOBAL JAVASCRIPT OBJECTS 
The global JavaScript objects 
represent things that the JavaScript 
language needs to create a model 
of. 

* DOCUMENT OBJECT MODEL 
The Document Object Model uses 
objects to create a representation of 
the current page. It creates a new 
object for each element (and each 
individual section of text) 
within the page.


* 1. Two of the window object's 
properties, i nnerWi dth and 
i nnerHei ght, show width and 
height of the browser window. 


* 2. Child objects are stored as 
properties of t heir parent object. 
So dot notation is used to access 
them, just like you would access 
any other property of that object. 
In turn, to access the properties 
of the child object, another dot is 
used between the child object's 
name and its properties, 


* 3. The element whose id 
attribute has a value of info is 
selected, and the message that 
has been built up to this point is 
written into the page. 


1. String 
2. Number 
3. Boolean 
4. Undefined (a variable that has been declared, but 
no value has been assigned to it yet) 
5. Null (a variable with no value - it may have had 
one at some point, but no longer has a value) 
As you have seen, both the web browser and the 
current document can be modeled using objects 
(and objects can have methods and properties)
6. 0bject 
Under the hood, arrays and functions are considered 
types of objects. 