# HTML and CSS part VIII
![HTML & CSS](https://media2.giphy.com/media/26tn33aiTi1jkl6H6/200.gif)

## Layout
In this chapter we are going to look at
how to control where each element sits
on a page and how to create attractive
page layouts.

This entails understanding how creating for a screen differs from designing for other mediums (such as print). This chapter will cover the following topics:

- Using normal flow, relative positioning, absolute positioning, and floats, experiment with different approaches to place components.

- Learn how screen sizes and resolution change between devices and how this influences the design process.

- Find out what the differences are between fixed width and liquid layouts, as well as how they're made.

- Learn how to utilize grids in your page designs to make them appear more professional.

## Key Concepts in Positioning Elements

Building Blocks
CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.

Inline boxes flow between surrounding text, but block-level boxes start on a new line and function as the fundamental building elements of any arrangement. By adjusting the width of the boxes, you can determine how much space each one takes up (and sometimes the height, too). Borders, margins, padding, and background colors can all be used to divide boxes.

- Block-level elements
start on a new line
Examples include:
< h1> < p> < ul> < li>

- Inline elements
flow in between
surrounding text
Examples include:
<img> <b> <i>

## Controlling the Position of Elements

Normal flow, relative positioning, and absolute positioning are the three CSS positioning techniques that allow you to manage the layout of a page. The position property in CSS is used to describe the positioning strategy. The float property may also be used to float items.

- Flow that is normal
Every element at the block level appears on a new line, making each item to look lower on the page than the one before it.
Even if the box widths are specified and there is enough room for two components to sit next to each other, they will not display next to each other. This is the browser's default behavior (until you tell it otherwise).

- Positioning in Relation to Others
This shifts an element from its regular location to the top, right, bottom, or left of where it would have been placed in normal flow. The location of surrounding elements is unaffected; they remain in the same place as they would be in regular flow.

- Positioning that is absolute
This specifies the element's position in respect to its parent element. It is removed from the usual flow, which means it has no effect on the location of any nearby components (since they just disregard the space it would have taken up).
As visitors scroll up and down the page, items that are absolutely positioned move.

