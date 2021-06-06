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