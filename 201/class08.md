# class 08

* CSS has the following positioning schemes that allow you to control 
the layout of a page **:** normal flow, relative positioning, and absolute 
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.


**Normal flow**

Every block-level element 
appears on a new line, causing 
each item to appear lower down 
the page than the previous one. 
Even if you specify the width 
of the boxes and there is space 
for two elements to sit side-byside, they will not appear next 
to each other. This is the default 
behavior 


**Relative Positioning**
This moves an element from the 
position it would be in normal 
flow, shifting it to the top, right, 
bottom, or left of where it 
would have been placed. This 
does not affect the position of 
surrounding elements; they stay 
in the position they would be in 
in normal flow.


**Absolute positioning**
This positions the element 
in relation to its containing 
element. It is taken out of 
normal flow, meaning that it 
does not affect the position 
of any surrounding elements 
(as they simply ignore the 
space it would have taken up). 
Absolutely positioned elements 
move as users scroll up and 
down the page


**Fixed Positioning**
This is a form of absolute 
positioning that positions 
the element in relation to the 
browser window, as opposed 
to the containing element. 
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
containing box. The floated 
element becomes a block-level 
element around which other 
content can flow

## Screen Sizes

* Different visitors to your site will have different sized screens that show 
different amounts of information, so your design needs to be able to 
work on a range of different sized screens

**Screen Resolution**



Resolution refers to the number of dots a screen shows per inch. Some 
devices have a higher resolution than desktop computers and most 
operating systems allow users to adjust the resolution of their screens



**Page Sizes**



Because screen sizes and display resolutions vary so much, web 
designers often try to create pages of around 960-1000 pixels wide 
(since most users will be able to see designs this wide on their screens).


**Fixed Width Layouts**


**Advantages**



* Pixel values are accurate 
at controlling size and 
positioning of elements.


* The designer has far greater 
control over the appearance 
and position of items on the 
page than with liquid layouts.


* You can control the lengths 
of lines of text regardless of 
the size of the user's window.


* The size of an image will 
always remain the same 
relative to the rest of the 
page.


**Disadvantages**



* You can end up with big gaps 
around the edge of a page.


* If the user's screen is a much 
higher resolution than the 
designer's screen, the page 
can look smaller and text can 
be harder to read.


* If a user increases font sizes, 
text might not fit into the 
allotted spaces.


* The design works best on 
devices that have a site or 
resolution similar to that of 
desktop or laptop computers.


* The page will often take up 
more vertical space than a 
liquid layout with the same 
content


**Liquid Layouts**

**Advantages**


* Pages expand to fill the entire browser window so there are no spaces around the page on a large screen.

* If the user has a small 
window, the page can 
contract to fit it without the 
user having to scroll to the 
side.


* The design is tolerant of 
users setting font sizes larger 
than the designer intended 
(because the page can 
stretch).


**Disadvantages**


* If you do not control the 
width of sections of the page 
then the design can look very 
different than you intended, 
with unexpected gaps around 
certain elements or items 
squashed together.


* If the user has a wide 
window, lines of text can 
become very long, which 
makes them harder to read.


* If the user has a very narrow 
window, words may be 
squashed and you can end up 
with few words on each line.


* If a fixed width item (such as 
an image) is in a box that is 
too small to hold it (because 
the user has made the 
window smaller) the image 
can overflow over the text


CSS **frameworks** aim to make your life easier by providing the code for 
common tasks, such as creating layout grids, styling forms, creating 
printer-friendly versions of pages and so on. You can include the CSS 
framework code in your projects rather than writing the CSS from scratch


**ADVANTAGES**


*  They save you from 
repeatedly writing code for 
the same tasks.


*  They will have been tested 
across different browser 
versions (which helps avoid 
browser bugs)


**DISADVANTAGES**


*  They often require that you 
use class names in your 
HTML code that only control 
the presentation of the page 
(rather than describe its 
content).


*  In order to satisfy a wide 
variety of needs, they often 
contain more code than you 
need for your particular web 
page (commonly referred to 
as code ???bloat???)


## summary 

* div elements are often used as containing elements 
to group together sections of a page.


*  Browsers display pages in normal flow unless you 
specify relative, absolute, or fixed positioning.


* The float property moves content to the left or right 
of the page and can be used to create multi-column 
layouts. (Floated items require a defined width.)


* Pages can be fixed width or liquid (stretchy) layouts.


*  Designers keep pages within 960-1000 pixels wide, 
and indicate what the site is about within the top 600 
pixels (to demonstrate its relevance without scrolling).


* Grids help create professional and flexible designs.


* CSS Frameworks provide rules for common tasks.


* You can include multiple CSS files in one page