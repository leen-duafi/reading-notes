## class 09

## Chapter 7: “Forms” (p.144-175)

* There are several types of form controls that you can use to collect information from visitors to your site.

* ADDING TEXT:
Text input (single-line)
Used for a single line of text such 
as email addresses and names.

Password input
Like a single line text box but it 
masks the characters entered.


Text area (multi-line)
For longer areas of text, such as 
messages and comments


* Making Choices:

Radio buttons
For use when a user must select 
one of a number of options.

Checkboxes
When a user can select and 
unselect one or more options.


Drop-down boxes 
When a user must pick one of a 
number of options from a list.

* Submitting Forms

Submit buttons
To submit data from your form 
to another web page

Image buttons
Similar to submit buttons but 
they allow you to use an image

* Uploading Files:

File upload
Allows users to upload files 
(e.g. images) to a website



**summarry**

* Whenever you want to collect information from 
visitors you will need a form, which lives inside a 
form element.


*  Information from a form is sent in name/value pairs.


* Each form control is given a name, and the text the 
user types in or the values of the options they select 
are sent to the server.


*  HTML5 introduces new form elements which make it 
easier for visitors to fill in forms




## Chapter 14: “Lists, Tables & Forms” (pp.330-357)




You can specify an image to act 
as a **bullet point** using the
list-style-image property.


The value starts with the letters 
url and is followed by a pair 
of parentheses. Inside the 
parentheses, the path to the 
image is given inside double 
quotes.


This property can be used on 
rules that apply to the ul and 
li elements.



**Lists** are indented into the page 
by default and the list-styleposition property indicates 
whether the marker should 
appear on the inside or the 
outside of the box containing the 
main points. 




This property can take one of 
two values:



**outside**
The marker sits to the left of the 
block of text. (This is the default 
behaviour if this property is not 
used.)




**inside**
The marker sits inside the box of 
text (which is indented).



**font-size** sets the size of the 
text entered by the user.
color sets the text color, and 
**background-color**sets the 
background color of the input.
**border** adds a border around 
the edge of the input box

The **:focus pseudo-class** is 
used to change the background 
color of the text input when it 
is being used, and the **:hover**
psuedo-class applies the same 
styles when the user hovers over 
them.

**background-image** adds a 
background image to the box. 
Because there is a different 
image for each input, we are 
using an attribute selector 
looking for the value of the id
attribute on each input.



**summary**

* In addition to the CSS properties covered in other 
chapters which work with the contents of all elements, 
there are several others that are specifically used to 
control the appearance of lists, tables, and forms.

* List markers can be given different appearances 
using the list-style-type and list-style image 
properties.

* Table cells can have different borders and spacing in 
different browsers, but there are properties you can 
use to control them and make them more consistent. 

* Forms are easier to use if the form controls are 
vertically aligned using CSS.

* Forms benefit from styles that make them feel more 
interactive


## Chapter 6: “Events” (pp.243-292)


* Select the element 
node(s) you want the 
script to respond to. 
For example, if you want to 
trigger a function when a user 
clicks on a specific link, you need 
to get the DOM node for that 
link element.
The UI events that relate to the 
browser window (rather than the 
HTML page loaded in it) work 
with the window object rather 
than an element node.


* Indicate which event on 
the selected node(s) will 
trigger the response. 
Programmers call this binding an 
event to a DOM node. 
The previous two pages showed 
a selection of the popular events 
that you can monitor for. 
Some events work with most 
element nodes, such as the 
mouseover event, which is 
triggered when the user rolls 
over any element. Other events 
only work with specific element 
nodes, such as the submit event, 
which only works with a form. 


* State the code you want 
to run when the event 
occurs. 
When the event occurs, on a 
specified element, it will trigger 
a function. This may be a named 
or an anonymous function. 


When the **c1ick** event fires on 
the close link the di smi ssNote() 
function is called. This function 
will remove the note that was 
added by the same script. 


**DETERMINING POSITION**

* as you move 
your mouse around the screen, 
the text inputs across the top of 
the page are updated with the 
current mouse position. 

* his demonstrates the three 
different positions you can 
retrieve when the mouse is 
moved or when one of the 
buttons is clicked. 

* Note how showPosition() is 
passed event as a parameter, 
which refers to the event object. 
The positions are all properties 
of this event object.

**summary**

* Events are the browser's way of indicating when 
something has happened (such as when a page has 
finished loading or a button has been clicked). 

* Binding is the process of stating which event you are 
waiting to happen, and which element you are waiting 
for that event to happen upon. 

* When an event occurs on an element, it can trigger a 
JavaScript function. When this function then changes 
the web page in some way, it feels interactive because 
it has responded to the user. 

* You can use event delegation to monitor for events 
that happen on all of the children of an element. 

* the most commonly used events are W3C DOM 
events, although there are others in the HTMLS 
specification as well as browser-specific events