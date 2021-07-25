# Functions

![image](https://scriptverse.academy/img/tutorials/js-nested-functions.png)

***Functions*** are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.
_________
### Defining functions

A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:

- The name of the function.
- A list of parameters to the function, enclosed in parentheses and separated by commas.
- The JavaScript statements that define the function, enclosed in curly brackets, {...}.

For example, the following code defines a simple function named square:

function square(number) {

  return number * number;

}

_________
### Function expressions

While the function declaration above is syntactically a statement, functions can also be
 created by a function expression.

Such a function can be anonymous; it does not have to have a name. For example, the 
function square could have been defined as:

const square = function(number) { return number * number }

var x = square(4) // x gets the value 16

However, a name can be provided with a function expression. Providing a name allows the function to refer to itself, and also makes it easier to identify the function in a debugger's stack traces:

const factorial = function fac(n) { return n < 2 ? 1 : n * fac(n - 1) }

console.log(factorial(3))
_________
## Predefined functions
JavaScript has several top-level, built-in functions:

Here is some of them

- eval()

The eval() method evaluates JavaScript code represented as a string.

- uneval()

The uneval() method creates a string representation of the source code of an Object.

- isFinite()

The global isFinite() function determines whether the passed value is a finite number. If needed, the parameter is first converted to a number.

- isNaN()

The isNaN() function determines whether a value is NaN or not. Note: coercion inside the isNaN function has interesting rules; you may alternatively want to use Number.isNaN(), as defined in ECMAScript 2015, or you can use typeof to determine if the value is Not-A-Number.

- parseFloat()

The parseFloat() function parses a string argument and returns a floating point number.

- parseInt()

The parseInt() function parses a string argument and returns an integer of the specified radix (the base in mathematical numeral systems).

- decodeURI()

The decodeURI() function decodes a Uniform Resource Identifier (URI) previously created by encodeURI or by a similar routine.