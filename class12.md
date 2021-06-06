# class 12 

##  Chart.js API

![image](https://www.ft.com/__origami/service/image/v2/images/raw/ftcms%3A347ece48-0f69-11e9-a3aa-118c761d2745?source=ig)

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.


To see how to use chart.js we’re going to create a set of 3 graphs; one will show the number of buyers a fictional product has over the course of 6 months, this will be a line chart; the second will show which countries the customers come from, this will be the pie chart; finally we’ll use a bar chart to show profit over the period.


It's easy to get started with Chart.js. All that's required is the script included in your page along with a single canvas node to render the chart

## Basic usage


The **canvas element differs from an img tag** in that, like for video, audio, or picture elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.

Providing fallback content is very straightforward: just insert the alternate content inside the canvas element. Browsers that don't support canvas will ignore the container and render the fallback content inside it. Browsers that do support canvas will ignore the content inside the container, and just render the canvas normally.


**The canvas element** creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. In this tutorial, we focus on the 2D rendering context. Other contexts may provide different types of rendering; for example, WebGL uses a 3D context based on OpenGL ES.

The canvas is initially blank. To display something, a script first needs to access the rendering context and draw on it. The canvas element has a method called **getContext()**, used to obtain the rendering context and its drawing functions. getContext() takes one parameter, the type of context. For 2D graphics, such as those covered by this tutorial, you specify "2d" to get a CanvasRenderingContext2D.


The first line in the script retrieves the node in the DOM representing the canvas element by calling the document.getElementById() method. **Once you have the element node,** you can access the drawing context using its getContext() method.


## Applying styles and colors

Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

* fillStyle = color
Sets the style used when filling shapes.


* strokeStyle = color
Sets the style for shapes' outlines.


color is a string representing a CSS color, a gradient object, or a pattern object. We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000).


In addition to drawing opaque shapes to the canvas, we can also draw **semi-transparent (or translucent) shapes**  This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.

* globalAlpha = transparencyValue
Applies the specified transparency value to all future shapes drawn on the canvas. The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). This value is 1.0 (fully opaque) by default.

The globalAlpha property can be useful if you want to draw a lot of shapes on the canvas with similar transparency, but otherwise it's generally more useful to set the transparency on individual shapes when setting their colors.


**Line styles**

There are several properties which allow us to style lines.

lineWidth = value
Sets the width of lines drawn in the future.


lineCap = type
Sets the appearance of the ends of lines.

lineJoin = type
Sets the appearance of the "corners" where lines meet.


miterLimit = value
Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.


getLineDash()
Returns the current line dash pattern array containing an even number of non-negative numbers.


setLineDash(segments)
Sets the current line dash pattern.


lineDashOffset = value
Specifies where to start a dash array on a line.


## Drawing text


![image](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text/baselines.png)


The canvas rendering context provides two methods to render text:



* fillText(text, x, y [, maxWidth])
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.




* strokeText(text, x, y [, maxWidth])
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.



**styling text**


font = value
The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif



textAlign = value
Text alignment setting. Possible values: start, end, left, right or center. The default value is start.



textBaseline = value
Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.



direction = value
Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.