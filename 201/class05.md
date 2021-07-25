# class05 

## Chapter 5: “Images” (pp.94-125)


**Linking to a Specific Part of the Same Page**

* To link to an element that uses 
an id attribute you use the <a>
element again, but the value of 
the href attribute starts with 
the # symbol, followed by the 
value of the id attribute of the 
element you want to link to. In 
this example, <a href="#top">
links to the <h1> element at 
the top of the page whose id
attribute has a value of top.

**Linking to a Specific Part of Another Page**

* Therefore, the href attribute 
will contain the address for the 
page (either an absolute URL or 
a relative URL), followed by the 
# symbol, followed by the value 
of the id attribute that is used on 
the element you are linking to.

**Adding Images**
To add an image into the page 
you need to use an <img>
element. This is an empty 
element (which means there is 
no closing tag). 

**height**
This specifies the height of the 
image in pixels.
**width**
This specifies the width of the 
image in pixels

**align**
commonly used to indicate how 
the other parts of a page should 
flow around an image

 * Save images in 
the right format
Websites mainly use images in 
jpeg, gif, or png format. If you 
choose the wrong image 
format then your image might 
not look as sharp as it should 
and can make the web page 
slower to load.

* Save images at 
the right size
You should save the image at 
the same width and height it will 
appear on the website. 

* Use the correct

Computer screens are made up 
of dots known as pixels. Images 
used on the web are also made 
up of tiny dots


## Chapter 11: “Color” (pp.246-263)

* CSS treats each HTML element as if it appears inside 
its own box and uses rules to indicate how that 
element should look.
*  Rules are made up of selectors (that specify the 
elements the rule applies to) and declarations (that 
indicate what these elements should look like).
* Different types of selectors allow you to target your 
rules at different elements.
* Declarations are made up of two parts: the properties 
of the element that you want to change, and the values 
of those properties.
*  CSS rules usually appear in a separate document, 
although they may appear within an HTML page


**rgb values**
These express colors in terms 
of how much red, green and 
blue are used to make it up. For 
example: rgb(100,100,90)
 **hex codes**
These are six-digit codes that 
represent the amount of red, 
green and blue in a color, 
preceded by a pound or hash # 
sign. For example: #ee3e80
**color names**
There are 147 predefined color 
names that are recognized 
by browsers. For example: 
DarkCyan


**hue**
Hue is the colloquial idea of 
color. In HSL colors, hue is often 
represented as a color circle 
where the angle represents the 
color, although it may also be 
shown as a slider with values 
from 0 to 360.
**saturation**
Saturation is the amount of 
gray in a color. Saturation is 
represented as a percentage. 
100% is full saturation and 0% 
is a shade of gray.
**lightness**
Lightness is the amount of 
white (lightness) or black 
(darkness) in a color. Lightness 
is represented as a percentage. 
0% lightness is black, 100% 
lightness is white, and 50% 
lightness is normal. Lightness 
is sometimes referred to as 
luminosity


## Chapter 12: “Text” (pp.264-299)

**Monospace**
Every letter in a monospace 
typeface is the same width. 
(Non-monospace fonts have 
different widths.)

**Cursive**
Cursive fonts either have 
joining strokes or other cursive 
characteristics, such as 
handwriting styles.

**Fantasy**
Fantasy fonts are usually 
decorative fonts and are often 
used for titles. They're not 
designed for long bodies of text.

* There are properties to control the choice of font, size, 
weight, style, and spacing.
X There is a limited choice of fonts that you can assume 
most people will have installed.
* If you want to use a wider range of typefaces there are 
several options, but you need to have the right license 
to use them.
* You can control the space between lines of text, 
individual letters, and words. Text can also be aligned 
to the left, right, center, or justified. It can also be 
indented.
* You can use pseudo-classes to change the style of an 
element when a user hovers over or clicks on text, or 
when they have visited a link

## JPEG vs PNG vs GIF — which image format to use and when?

Use **JPEG format** for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use **PNG format** for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use **GIF format** for images that contain animations.

* Compression can be of two types — lossless and lossy. **In lossless compression**, it is possible to reconstruct the original image from the compressed image because there is no information loss during compression. This is not the case in lossy compression . **Lossy compression** algorithms always have a superior compression ratio (the ratio of size of compressed image to original image) as compared to lossless compression. However, this compression ratio comes at a cost of reduced quality that becomes more evident after zooming in on the image. This noticeable reduction in quality or distortion of the image is called compression artefact.


**pNG** is a lossless image format using DEFLATE compression. No data is lost during compression and no compression artefacts are introduced in the image. For this reason, a PNG image would retain higher quality than an image than JPEG and would look a lot sharper


**GIF** is also a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics in websites in its early days because the support of PNG was still growing. Given that PNG is now supported across all major devices and that PNG compression is about 5–25% better than GIF compression, GIF images are now mainly used only if the image contains animations.


 * **transparency** indicates something that is completely invisible. Logos and icons often need to be placed on backgrounds with variable colours.

**JPEG** images don’t support transparency and are hence not usable for such cases.

**GIF** images support transparency by declaring a single colour in the colour palette 