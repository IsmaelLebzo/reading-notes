# Passing Functions as Props
![Passing Functions as Props](https://i.ytimg.com/vi/yH5Z-lSeV9Y/maxresdefault.jpg)

## Lists and Keys

Let's go through how to convert lists in JavaScript first.

In the code below, we use the map() method to double the values of an array of integers. We report the new array provided by map() by assigning it to the variable doubled:

const numbers = [1, 2, 3, 4, 5];\
const doubled = numbers.map((number) => number * 2);\
console.log(doubled);\
This code logs [2, 4, 6, 8, 10] to the console.

In React, transforming arrays into lists of elements is nearly identical.
## Rendering Multiple Components

Curly braces can be used to create collections of items and include them in JSX.

Using the JavaScript map() method, we cycle through the numbers array below. For each item, we return a li> element. Finally, we assign listItems to the resultant array of elements:

const numbers = [1, 2, 3, 4, 5];\
const listItems = numbers.map((number) =>\
  < li>{number}</ li>
);\
We include the entire listItems array inside a < ul> element, and render it to the DOM:

ReactDOM.render(\
  < ul>{listItems}< /ul>,\
  document.getElementById('root')\
);

## Basic List Component

Normally, lists would be shown within a component.

The preceding example may be refactored into a component that takes an array of integers and returns a list of items.

function NumberList(props) {\
  const numbers = props.numbers;\
  const listItems = numbers.map((number) =>\
    < li>{number}</ li>\
  );\
  return (\
    < ul>{listItems}</ ul>\
  );\
}

const numbers = [1, 2, 3, 4, 5];\
ReactDOM.render(\
  < NumberList numbers={numbers} />,\
  document.getElementById('root')\
);

When you execute this code, you'll get a warning that a key for list items is required. When constructing lists of items, a "key" is a specific string property that must be included. In the following part, we'll go through why it's crucial.

Let's give our list elements within numbers a key.

Fix the missing key problem with map().

function NumberList(props) {\
  const numbers = props.numbers;\
  const listItems = numbers.map((number) =>\
    < li key={number.toString()}>\
      {number}\
    </ li>\
  );\
  return (\
    < ul>{listItems}</ ul>\
  );\
}

const numbers = [1, 2, 3, 4, 5];\
ReactDOM.render(\
  < NumberList numbers={numbers} />,\
  document.getElementById('root')\
);

# How to Use the Spread Operator (…) in JavaScript
![image](https://livecodestream.dev/post/how-to-use-the-spread-operator-in-javascript/featured_hu552373e3dd9cfa7192fd6d6eeac47a64_53660_680x0_resize_q75_box.jpg)

The spread operator is a convenient and fast way to add items to arrays, combine arrays or objects, and spread an array over a function's parameters.

## What is the spread operator?

Spread syntax in JavaScript refers to the usage of a three-dot ellipsis (...) to extend an iterable object into a list of parameters.

## What is ... used for?

Consider the following example of using Math.max() to determine the biggest number in an array:

Math.max(1,3,5) // 5\
Math.max([ 1,3,5]) // NaN

It is not possible to send an array to a JavaScript function that expects distinct parameters. It returns a NaN value in this situation. Enter...:


Math.max(...[ 1,3,5]) // 5

The array is “spread” into distinct arguments using the spread idiom.

## What else can … do?

In JavaScript, the... spread operator is helpful for a variety of purposes, including the following:

- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Using an array as arguments
- Adding an item to a list
- Adding to state in React
- Combining objects
- Converting NodeList to an array