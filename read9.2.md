# HTML and CSS part IX
![HTML & CSS](https://media2.giphy.com/media/26tn33aiTi1jkl6H6/200.gif)

## Forms

Traditionally, the term 'form' has referred
to a printed document that contains
spaces for you to fill in information.

The notion of a form is used by HTML to refer to various components that allow you to collect information from visitors to your site.
HTML forms provide a collection of components to collect data from your visitors, whether you're putting a basic search box to your website or need to construct more sophisticated insurance applications. This chapter will teach you:

- What is the best way to make a form on your website?

- The many tools for data collection

- HTML5 form controls are now available.

### Why Forms?

The best known form on the web is probably
the search box that sits right in the middle of
Google's homepage.

Forms allow users to do more than just search. They also allow them to do various tasks online. You'll come across forms.

when signing up for newsletters or mailing lists, when registering as a member of a website, while buying online, and when signing up for newsletters or mailing lists

### Form Structure

< form>
Form controls live inside a
< form> element. This element
should always carry the action
attribute and will usually have a
method and id attribute too.

Action:
An action property is required for every form> element. Its value is the URL of the server page that will receive the data from the form after it is submitted.
___
## Lists, Tables and Forms

There are a number of CSS attributes designed to operate with certain HTML components, such as lists, tables, and forms.

This chapter will teach you how to:

- On lists, specify the type of bullet point or numbering.

- Table cells should have borders and backgrounds.

- Control the look of the form controls.

These variables work together to provide you more control over particular areas of your pages.

### Bullet Point Styles

list-style-type
You may alter the form or style of a bullet point (also known as a marker) with the list-style-type property.

It can be used on rules that
apply to the < ol>, < ul>, and < li>
elements.

### Table Properties

Several attributes that are often used with tables have previously been introduced to you. We'll use the following as an example to put them all together:

- width to set the width of the
table.
- padding to set the space
between the border of each table
cell and its content
- text-transform to convert the
content of the table headers to
uppercase
- letter-spacing, font-size
to add additional styling to the
content of the table headers
- text-align to align the writing
to the left of some table cells and
to the right of the others
- background-color to change
the background color of the
alternating table rows
____
# JS part IX
![JS](https://i.gifer.com/7S7L.gif)
## Events

W hen you browse the web, your browser registers different
types of events. It's the browser's way of saying, "Hey, this
just happened." Your script can then respond to these events. 

Scripts frequently react to these events by changing the web page's content (through the Document Object Model), making the page feel more dynamic. This chapter will teach you how to:

- EVENTS ARE CREATED BY INTERACTIONS. Users can trigger events by clicking or tapping on a link, hovering or swiping over an element, typing on the keyboard, resizing the window, or waiting for the requested page to load.
- TRIGGER CODE FOR EVENTS An event can be used to activate a specific function when it happens or fires.
- CODE RESPONDS TO USERS You saw how the DOM may be used to update a page in the last chapter. The events can cause the DOM to alter in a variety of ways.

### DIFFERENT EVENT TYPES 
Here's a rundown of what happens in your browser while you're surfing the web. You may utilize any of these events to call a function in your JavaScript code.

TERMINOLOGY

EVENTS EITHER FIRE OR RAISED
When something happens, it's commonly characterized as having "fired" or "raised." If the user taps on a link in the diagram on the right, the browser will trigger a click event.

SCRIPTS TO TRIGGER EVENTS

A function or script is said to be triggered by events. When a user clicks on an element in this diagram, a script that enlarges the selected object may be triggered.

### HOW EVENTS TRIGGER JAVASCRIPT CODE 

When a user interacts with HTML on a web page, there are three stages that must be followed in order for JavaScript code to be triggered.
The term "event handling" refers to the combination of these procedures.