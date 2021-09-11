# EASILY CREATE STUNNING ANIMATED CHARTS WITH CHART.JS
![Charts](https://media0.giphy.com/media/l2JdTgYZ7VG4EeBVe/giphy.gif)

Charts are considerably better at graphically showing data than tables, and they have the extra virtue of never being forced into usage as a layout tool. They're more convenient to look at and transmit information fast, but they're not necessarily simple to make.

Chart.js, a JavaScript plugin that leverages HTML5's canvas element to create the graph onto the page, is a wonderful way to get started with charts. It's a well-documented plugin that makes creating bar charts, line charts, pie charts, and other graphs a breeze.

To demonstrate how to use chart.js, we'll make a set of three graphs: one will show the number of buyers a fictional product has over the course of 6 months using a line chart; the second will show which countries the customers come from using a pie chart; and the third will show profit over the period using a bar chart.

## Setting up

The first step is to get Chart.js installed. Remove the Chart.min.js file from the unzipped folder and place it in the working directory. Then import the script into a new HTML page.

## Drawing a line chart

To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page.

## Drawing a pie chart

Our line chart is complete, so let’s move on to our pie chart. First, we need the canvas element.

## Drawing a bar chart

Let's finish off by adding a bar chart to our page. Fortunately, the bar chart's syntax is fairly identical to the line chart we've just created. We begin by including the canvas element.

##  Conclusion
You can see an example of this in action here, and the whole script is available here if you want to copy & paste.
___________
# Drawing shapes with canvas
![Canvas](https://cdn.dribbble.com/users/882114/screenshots/2116878/final-canvas-animation-rev2.gif)

We can now dive into the intricacies of how to draw on the canvas now that we've set up our canvas environment. You will have learnt how to draw rectangles, triangles, lines, arcs, and curves by the conclusion of this tutorial, giving you a basic understanding of some of the fundamental forms. When drawing things onto the canvas, working with paths is crucial, and we'll show how to accomplish that.

## The grid

Before we begin drawing, we must first discuss the canvas grid, often known as coordinate space. A canvas element was 150 pixels wide and 150 pixels high in our HTML skeleton from the previous page.


In most cases, 1 unit in the grid equals 1 pixel on the canvas. The origin of this grid is at coordinates in the upper left corner (0,0). All components are positioned in relation to this starting point. As a result, the blue square's top left corner moves x pixels to the left and y pixels to the right, at coordinates x, y. (x,y). We'll learn how to transfer the origin to a new location, rotate the grid, and even scale it later in this lesson, but for now we'll keep with the default.

## Drawing rectangles

Canvas only supports two primitive shapes: rectangles and pathways, unlike SVG (lists of points connected by lines). All additional forms must be made by joining two or more pathways together. Fortunately, we have a variety of route drawing methods that allow us to create extremely complicated forms.

Let's start with the rectangle. On the canvas, there are three functions for drawing rectangles:

Draws a filled rectangle using fillRect(x, y, width, height).
Draws a rectangle shape with strokeRect(x, y, width, height).
clearRect(x, y, width, height) completely transparently clears the provided rectangular region.

## Drawing paths
Let's have a look at pathways now. A route is a collection of points connected by segments of lines of various forms, curved or not, varying widths, and colors. It is possible to shut a path or even a subpath. We take a few more steps to build forms using paths:

1. To begin, you must first build the route.
2. The route is then drawn into using drawing instructions.
3. After you've constructed the route, you may stroke or fill it to render it.

