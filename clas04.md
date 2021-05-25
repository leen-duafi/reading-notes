# clas04

## Chapter 4: Ch.4 “Links” (pp.74-93)

* **The definition list** is created with 
the <dl> element and usually 
consists of a series of terms and 
their definitions.
Inside the <dl> element you will 
usually see pairs of <dt> and 
<dd> elements.

**<dt>**
This is used to contain the term 
being defined (the definition 
term).

**<dd>**
This is used to contain the 
definition.
Sometimes you might see a list 
where there are two terms used 
for the same definition or two 
different definitions for the same 
term


* Ordered lists use numbers.
* Unordered lists use bullets.
* Definition lists are used to define terminology.

 **<a>**
Links are created using the <a>
element which has an attribute 
called href. The value of the 
href attribute is the page that 
you want people to go to when 
they click on the link.

**mailto**
To create a link that starts up 
the user's email program and 
addresses an email to a specified 
email address, you use the <a>
element.

## Chapter 15: “Layout” (pp.358-404)

**Block-level boxes** start on a new line and act as the main building blocks 
of any layout, while inline boxes flow between surrounding text. You can 
control how much space each box takes up by setting the width of the 
boxes (and sometimes the height, too). To separate boxes, you can use 
borders, margins, padding, and background colors.

If one block-level element sits inside another 
block-level element then the outer box is 
known as **the containing or parent element**


**Normal flow**
Every block-level element 
appears on a new line, causing 
each item to appear lower down 
the page than the previous one. 
Even if you specify the width 
of the boxes and there is space 
for two elements to sit side-byside, they will not appear next 
to each other. 

**Relative Positioning**
This moves an element from the 
position it would be in normal 
flow, shifting it to the top, right, 
bottom, or left of where it 
would have been placed. This 
does not affect the position of 
surrounding elements

**Absolute positioning**
This positions the element 
in relation to its containing 
element. It is taken out of 
normal flow, meaning that it 
does not affect the position 
of any surrounding elements 

**Fixed Positioning** 
Elements with fixed positioning 
do not affect the position of 
surrounding elements and they 
do not move when the user 
scrolls up or down the page.

**Floating Elements**
Floating an element allows 
you to take that element out 
of normal flow and position 
it to the far left or right of a 
containing box.

## Chapter 3 (first part): “Functions, Methods, and Objects” 

* Variables are used to temporarily store pieces of 
information used in the script. 

* Arrays are special types of variables that store more 
than one piece of related information.

* JavaScript distinguishes between numbers (0-9), 
strings (text), and Boolean values (true or false).


**Functions** let you group a series of statements together to perform a 
specific task. If different parts of a script repeat the same task, you can 
reuse the function (rather than repeating the same set of statements). 



If you are going to ask the function to perform its task 
later, you need to give your **function a name** . They do not have a 
should describe the task it is When you write a function and name, so they cannot be called. 
performing

When you write a function and you expect it to provide you with an answer, the response is known as a **return value.**


##  “6 Reasons for Pair Programming”

**pair programming** commonly involves **two roles: the Driver and the Navigator.** The **Driver** is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. **The Navigator** uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. 

**Pair programming touches on all four skills:** developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.

* Greater efficiency

 So, in the long-run, it’s often actually more efficient than two people working on separate features. When coming up with ideas and discussing solutions out loud, two programmers may come to a solution faster than one programmer on their own. Also, when the pair is stuck, both programmers can research the problem and reach a solution faster


* Engaged collaboration

 When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone. It is harder to procrastinate or get off track when someone else is relying on you to complete the work.

* Learning from fellow students

 he developers in a pairing have different skill sets. If one programmer is more experienced in a certain skill, they can teach a student who is less familiar with that area. The less experienced developer benefits from the experienced developer’s knowledge and guidance, and the latter benefits from explaining the topic in their own words

* Social skills

 Pair programming not only improves programming skills, but can also help programmers develop their interpersonal skills. 

* Job interview readiness
  
  For most roles, the ability to work with and learn from others and stellar communication skills are as (or more!) important to a company than specific technical skills. Pair programming strengthens all of those skills.

* Work environment readiness

 Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. 