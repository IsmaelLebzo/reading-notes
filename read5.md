# Operators
**JavaScript** has the following types of operators. This section describes the operators and contains information about operator precedence.

- Assignment operators
- Comparison operators
- Arithmetic operators
- Bitwise operators
- Logical operators
- String operators
- Conditional (ternary) operator
- Comma operator
- Unary operators
- Relational operators

***JavaScript*** has both binary and unary operators, and one special ternary operator, the conditional operator. A binary operator requires two operands, one before the operator and one after the operator:

For example, 3+4 or x*y.

-----------
## Assignment operators
----
An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = y assigns the value of y to x.

There are also compound assignment operators that are shorthand for the operations listed in the following table:

![operators](oparator.PNG)

and much more!

-----
# Loops 
Loops offer a quick and easy way to do something repeatedly. This chapter of the JavaScript Guide introduces the different iteration statements available to JavaScript.

You can think of a loop as a computerized version of the game where you tell someone to take X steps in one direction, then Y steps in another. For example, the idea "Go five steps to the east" could be expressed this way as a loop:

for (let step = 0; step < 5; step++) {

  // Runs 5 times, with values of step 0 through 4.

  console.log('Walking east one step');
}

-----
## For statement
A for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop.

A for statement looks as follows:

for ([initialExpression]; [conditionExpression]; [incrementExpression])

  statement

--------
## While statement
A while statement executes its statements as long as a specified condition evaluates to true.

 A while statement looks as follows:

while (condition)

  statement

If the *condition *becomes false, statement within the loop stops executing and control passes to the statement following the loop.