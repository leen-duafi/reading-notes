# class 11 

## Chapter 16: “Images” (pp.406-427)


* Centering images Using C


By default, images are inline 
elements. This means that they 
flow within the surrounding text. 
In order to center an image, it 
should be turned into a blocklevel element using the display
property with a value of block. 
Once it has been made into a 
block-level element, there are 
two common ways in which you 
can horizontally center an image:


*  On the containing element, 
you can use the text-align
property with a value of center.


*  On the image itself, you can 
use the use the margin property 
and set the values of the left and 
right margins to auto.
You can specify class names 
that allow any element to be 
centered, in the same way that 
you can for the dimensions or 
alignment of images


* Repeating images

**repeat**
The background image is 
repeated both horizontally and 
vertically (the default way it 
is shown if the backgroundrepeat property isn't used).


**repeat-x**
The image is repeated 
horizontally only (as shown in 
the first example on the left).
repeat-y
The image is repeated vertically 
only.


**no-repeat**
The image is only shown once.
The background-attachment 
property specifies whether a 
background image should stay in 
one position or move as the user 
scrolls up and down the page. It 
can have one of two values:


**fixed**
The background image stays in 
the same position on the page.


**scroll**
The background image moves 
up and down as the user scrolls 
up and down the page.


* summary

You can specify the dimensions of images using CSS. 
This is very helpful when you use the same sized 
images on several pages of your site.

* Images can be aligned both horizontally and vertically 
using CSS.

* You can use a background image behind the box 
created by any element on a page. 

* Background images can appear just once or be 
repeated across the background of the box.

* You can create image rollover effects by moving the 
background position of an image.

* To reduce the number of images your browser has to 
load, you can create image sprites


## Chapter 19: “Practical Information” (476-492)



* How to Identify Keywords and Phrases


**1: Brainstorm**
List down the words that 
someone might type into 
Google to find your site. Be sure 
to include the various topics, 
products or services your site is 
about.
It often helps to ask other people 
what words they would use to 
find your site because people 
less familiar with a topic might 
use different terms than you. (In 
particular, they are less likely to 
use industry-specific jargon.)
Your list may include some 
keyword phrases (not just 
individual words) if you have 
topics which are described by 
more than one word.


**2: Organize**
Group the keywords into 
separate lists for the different 
sections or categories of your 
website.


**3: Research**
There are several tools that let 
you enter your keywords and 
then they will suggest additional 
keywords you might like to 
consider, such as:
adwords.google.co.uk/
select/KeywordToolExternal
(When using this tool, select the 
"exact match" option rather than 
"broad match.")
www.wordtracker.com
www.keyworddiscovery.com
Once these tools have suggested 
additional keywords, add the 
relevant options to your lists. 
(Keyword tools will most likely 
suggest some terms that are 
irrelevant so do omit any that do 
not seem appropriate)



**4: Compare**

It is very unlikely that your 
site will appear at the top of 
the search results for every 
keyword. This is especially true 
for topics where there is a lot 
of competition. The more sites 
out there that have already been 
optimized for a given keyword, 
the harder it will be for you to 
rise up the search results when 
people search on that term.
Some of the keyword research 
sites can tell you how many 
people have searched for a 
specific keyword to help you 
know how much competition 
those terms have.
You can also use Google's 
advanced search feature to 
just search the titles of web 
pages. This will help you to 
determine how many sites have 
that keyword in the title of their 
pages. (The more pages with 
the term in the title, the more 
competition there is.)


**5: Refine**
Now you need to pick which 
keywords you will focus on. 
These should always be the ones 
that are most relevant to each 
section of your site.
If there is a phrase that is very 
relevant but you find there is a 
lot of competition, you should 
still use it. To improve the 
chances of your site being found 
you can look at whether there 
are other words that could be 
incorporated into a phrase. For 
example, if the information or 
service you offer on your website 
is location specific, then you will 
often find that incorporating 
your location into your keyword 
list will help people find you.
If your site is promoting a slate 
roofing company in Australia 
then it is better to get 100 
people from Australia who are 
looking for a slate roof than 
10,000 from the USA who are 
looking for other kinds of rooves.


**6: Map**
Now that you have a refined list 
of keywords, you know which 
have the most competition, and 
which ones are most relevant, 
it is time to start picking which 
keywords you will use for each 
page.

Pick 3-5 keywords or phrases 
that map to each page of your 
website and use these as the 
keywords for each page.
You should not need to repeat 
the same keywords on all of 
the pages. It is also likely that, 
as you move further away from 
the homepage into the sections 
of the site, the keywords will 
become more specific to the 
individual topic dealt with on 
each page


* summary

* Search engine optimization helps visitors find your 
sites when using search engines.

* Analytics tools such as Google Analytics allow you to 
see how many people visit your site, how they find it, 
and what they do when they get there.

* To put your site on the web, you will need to obtain a 
domain name and web hosting.

* FTP programs allow you to transfer files from your 
local computer to your web server.

* Many companies provide platforms for blogging, email 
newsletters, e-commerce and other popular website 
tools (to save you writing them from scratch


## This MDN article on audio and video elements


HTML5 comes with elements for embedding rich media in documents — video and audio — which in turn come with their own APIs for controlling playback, seeking, etc. This article shows you how to do common tasks such as creating custom playback controls.



The whole player is wrapped in a div element, so it can all be styled as one unit if needed.
The video element contains two source elements so that different formats can be loaded depending on the browser viewing the site.


**Exploring the HTML**

The controls HTML is probably the most interesting:
We have four buttons — play/pause, stop, rewind, and fast forward.
Each button has a class name, a data-icon attribute for defining what icon should be shown on each button (we'll show how this works in the below section), and an aria-label attribute to provide an understandable description of each button, since we're not providing a human-readable label inside the tags. The contents of aria-label attributes are read out by screenreaders when their users focus on the elements that contain them.


There is also a timer div, which will report the elapsed time when the video is playing. Just for fun, we are providing two reporting mechanisms — a span containing the elapsed time in minutes and seconds, and an extra div that we will use to create a horizontal indicator bar that gets longer as the time elapses. To get an idea of what the finished product will look like

**Exploring the CSS** 

We start off with the visibility of the custom controls set to hidden. In our JavaScript later on, we will set the controls to visible, and remove the controls attribute from the video element. This is so that, if the JavaScript doesn't load for some reason, users can still use the video with the native controls.


We give the controls an opacity of 0.5 by default, so that they are less distracting when you are trying to watch the video. Only when you are hovering/focusing over the player do the controls appear at full opacity.


We lay out the buttons inside the control bar using Flexbox (display: flex), to make things easier.


**Summary**

* The time display currently breaks if the video is an hour long or more (well, it won't display hours; just minutes and seconds). Can you figure out how to change the example to make it display hours?

* Because audio elements have the same HTMLMediaElement functionality available to them, you could easily get this player to work for an audio element too. Try doing so.

* Can you work out a way to turn the timer inner div element into a true seek bar/scrobbler — i.e., when you click somewhere on the bar, it jumps to that relative position in the video playback? As a hint, you can find out the X and Y values of the element's left/right and top/bottom sides via the getBoundingClientRect() method, and you can find the coordinates of a mouse click via the event object of the click event, called on the Document object.



## Chapter 9: pages 201-206

The most popular way of 
adding Flash into a web page 
is using JavaScript. There are 
several scripts that allow you 
to do this without an in-depth 
understanding of the JavaScript 
language.


The script we will be looking at 
here is called SWFObject. You 
can obtain a copy of it for free 
from Google, and you can see 
how we use it on the next page.
One advantage to using this 
technique is that it allows 
browsers to show alternative 
content for users whose 
browsers are not capable of 
showing Flash.


This technique uses a div
element to create a space where 
the Flash movie should sit. 
The div element has an id
attribute whose value is used 
by the SWFObject script. In this 
example, the value of the id
attribute is bird.


Inside the div element you 
can place the alternative content 
for users who are not able to 
play Flash.
Adding a Flash Movie 
to Your Web Page
The SWFObject script will check 
to see if the user's browser can 
play the Flash movie. If it can, the 
script will replace the content of 
the div with the .swf file.
For users who cannot see the 
Flash movie, you could show a 
still from the movie instead. You 
might also like to consider using 
a text description of the Flash 
file.


If you use a text description as 
alternative content, then you can 
achieve two further benefits:
* The text can be accessed by 
those with visual and/or physical 
impairments who are not able to 
interact with the Flash file. 


* The text can be indexed by 
search engines (which are not as 
effective at indexing SWF files), 
increasing the chance that your 
content will be found