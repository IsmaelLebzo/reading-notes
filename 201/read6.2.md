# Understanding The Problem Domain Is The Hardest Part Of Programming
![HTML & CSS](https://media2.giphy.com/media/26tn33aiTi1jkl6H6/200.gif)

There are many common answers to this question:

- Learning a new technology
- Naming things
- Testing your code
- Debugging
- Fixing bugs
- Making software maintainable

The list goes on and on.
But as I reflect back on my programming career, and I’ve conversed with many new programmers that are learning the craft, I’ve found the single hardest thing about programming is learning the problem domain.

## A familiar problem
In several of my Pluralsight classes, I demonstrate how to create the “Protein Tracker” application.

I'm frequently asked why I spend so much time in each of my classes explaining how to develop the same simple application.

“Familiarity” is the answer.

The Protein Tracker app's concept is that it allows a user to establish a daily protein intake target. The user can enter protein quantities, which are then added to the user's overall protein count.

### Why problem domains are hard

The difficulty of puzzles like this one stems from the fact that you can't see what you're trying to create very well. When putting together a jigsaw puzzle, you often follow steps that look like this:

1. Figure out what the major components of the picture are
2. Sort the pieces by color or component
3. Put together all the border pieces
4. Put together each component of the picture from the piles you created

### Programming is easy if you understand the problem domain

I used to work at Hewlett-Packard, where I wrote software for multi-function printers.

At the time, the majority of the job included simple waterfall development. There wasn't much Agile going on there while I was there, at least not when I was there.

____
# JPEG vs PNG vs GIF Part VI

![JPEG vs PNG vs GIF](https://media0.giphy.com/media/xT9IgzoKnwFNmISR8I/giphy.gif)

## WHAT IS AN OBJECT? 

Objects bring together a collection of variables and functions to build a model of anything you'd see in real life. Variables and functions in an object are given new names.

VARIABLES ARE REFERRED TO AS PROPERTIES IN AN OBJECT.
A property is a variable that is a component of an object. The name of a hotel or the number of rooms it has are examples of properties that tell us about the item.
Each hotel may have a different name and number of rooms than the others.

IN AN OBJECT, FUNCTIONS ARE CALLED METHODS.
A method is a function that is a component of an object.
Methods are connected with the object and represent tasks. By subtracting the number of booked rooms from the total number of rooms, you can determine how many rooms are available.

This object represents a hotel. It has five properties and one method.
The object is in curly braces. It is stored in a variable called hotel.

Like variables and named functions,
properties and methods have a
name and a value. In an object,
that name is called a key. 

An object cannot have two keys
with the same name. This is
because keys are used to access
their corresponding values. 

The value of a property can be a
string, number, Boolean, array, or
even another object. The value of a
method is always a function. 

## Document Object Model
The Document Object Model (DOM) describes how browsers should construct an HTML page model and how JavaScript may access and alter a web page's contents while it is in the browser window.

The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules.
It is implemented by all major browser makers, and covers two primary areas: 

MAKING A MODEL OF THE HTML PAGE 

ACCESSING AND CHANGING THE HTML PAGE 

### THE DOM TREE IS A MODEL OF A WEB PAGE 

A browser builds a model of a web page as it loads it.
The model is known as a DOM tree, and it is kept in the memory of browsers.
It is made up of four different sorts of nodes.BODY OF HTML PAGE
< html>

< body>

< di v id="page">

< hl id="header">List< /hl>

< h2>Buy groceries< /h2>

< ul >

< li id="one" class="hot">< em>fresh</em> figs< /li>

< li id="two" class="hot">pine nuts< /l i>

< l i id="three" class="hot">honey< /l i >

< l i id="four">balsamic vinegar< /l i>

</ ul >

< script src="js/l i st.js ">< /script>

</ div>

</ body>

</ html > 

- THE DOCUMENT NODE 

- ELEMENT NODES 
