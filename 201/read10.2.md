# JavaScript Part X
![javascript!](https://tutorialzine.com/media/2017/08/titanic.gif)

JavaScript is a difficult language to master, and everyone makes mistakes when programming it. This chapter will teach you how to identify and correct problems in your code. It will also show you how to create scripts that gracefully handle potential problems.

If you're writing JavaScript for the first time, don't expect to get it right the first time. Programming is similar to problem solving in that you are given a puzzle and must not only solve it but also generate the instructions that will allow the machine to solve it. too.

Nobody gets everything perfect the first time they write a big script. At first glance, browser error messages appear obscure, but they may help you figure out what went wrong with your JavaScript and how to repair it. This chapter will teach you about:

- THE CONSOLE & DEVELOPMENT TOOLS Error-hunting tools included into the browser.
- COMMON \sPROBLEMS Errors that people make and how to fix them.
- HANDLING \sERRORS How code may gracefully handle possible failures.

## ORDER OF EXECUTION 

Knowing how scripts are handled can aid in locating the cause of an issue.
The sequence in which statements are performed can be complicated; certain activities need the execution of another statement or function before they can be completed.

1. The greetUser() method provides the value for the greeting variable.
2. greetUser() constructs the message by combining the string 'He 11 o'with the getName() result ().
3. greetUser's name is returned by getName (). ().
2. Now that greetUser() is aware of the user's name, it mixes it with the string. The message is then returned to the statement that called it in step one.
1. The significance of the greeting is remembered.
4. An alert box receives this greeting variable.

## EXECUT.ION CONTEXTS 
Execution contexts are used by the JavaScript interpreter.
There is a single global execution context, as well as a fresh execution context for each function. They are the same as variable scope.

EXECUTION CONTEXT
JavaScript
Hello Molly
Every statement in a script lives in one of three
execution contexts:
Q GLOBAL CONTEXT
Code that is in the script, but not in a function.
There is only one global context in any page.
FUNCTION CONTEXT
Code that is being run within a function.
Each function has its own function context.
Q EVAL CONTEXT (NOT SHOWN)
Text is executed like code in an internal function
called eva l {) (which is not covered in this book). 

