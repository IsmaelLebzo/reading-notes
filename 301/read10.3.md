# In memory storage

![image](https://thumbs.gfycat.com/AshamedDapperEasteuropeanshepherd-size_restricted.gif)

## The JavaScript Call Stack - What It Is and Why It's Necessary

The JavaScript engine (which may be found in a hosting environment such as a browser) is a single-threaded interpreter with a single call stack and heap. Web APIs such as the DOM, AJAX, and Timers are available in the browser.

The purpose of this article is to explain what the call stack is and why it is necessary. Understanding the call stack can help you understand how the JavaScript engine handles "function hierarchy and execution order."

The call stack is mostly utilized for invoking functions (call). Because the call stack is single, functions are executed one by one, from top to bottom. It denotes a synchronous call stack.

When a function is called, the function, its parameters, and variables are placed onto the call stack, forming a stack frame. This is a memory region in the stack called a stack frame. When the function returns and pops out of the stack, the memory is cleaned.

## How does the call stack handle function calls?

1. When secondFunction() gets executed, an empty stack frame is created. It is the main (anonymous) entry point of the program.
2. secondFunction() then calls firstFunction()which is pushed into the stack.
3. firstFunction() returns and prints “Hello from firstFunction” to the console.
4. firstFunction() is pop off the stack.
5. The execution order then move to secondFunction().
6. secondFunction() returns and print “The end from secondFunction” to the console.
7. secondFunction() is pop off the stack, clearing the memory.

## What causes a stack overflow?

When a recursive function (one that calls itself) does not have an exit point, a stack overflow occurs. The browser (hosting environment) can only handle a certain number of stack calls before throwing a stack error.

## In summary

The following are the important takeaways from the call stack:

1. It is single-threaded. Meaning it can only do one thing at a time.
2. Code execution is synchronous.
3. A function invocation creates a stack frame that occupies a temporary memory.
4. It works as a LIFO — Last In, First Out data structure.

We've utilized the call stack article to build the groundwork for a series of articles on Asynchronous JavaScript (which we will be looking at in another article).

# JavaScript error messages && debugging

As a developer, you spend the majority of your time reading code and then debugging it, most likely to be able to understand it or solve a "unexpected feature" (which, kidding aside, is more properly called as a "bug").

## Types of error messages

The (in)famous error message, like the one we saw only moments ago, is the first sign that anything is amiss with your code. It generally shows on your console (being developer tools of the browser, terminal or whatever else you are using).\
Reading an error message is second nature to programmers; for everyone else, it's something you learn whether you like it or not, so let's take a closer look at each of them.

- Reference errors
- Syntax errors
- Range errors
- Type errors

## Debugging

The simplest and maybe most frequent approach to debug your JS code is to use the console. log() the variables you want to check or, by using chrome developer tools, open your page with your JS code (press cmd+o in macOS or Ctrl+o in Windows) and choose your file to debug, click the line you wanna debug and refresh your page again (F5).

If the line you picked was executed, you'll be able to examine what happened before that point and try evaluating the following lines to verify if everything is working as it should.
You may also set a breakpoint in your code by including a debugger statement in the line you wish to break.

## Conclusion

One of your most powerful weapons is the ability to understand error messages and practice troubleshooting. has a developer, do it regularly, and you'll see a significant reduction in the amount of time you spend on each error you uncover along the road. Remember to remove any debugging items from your code before committing/pushing; we don't want the customer or another developer to get trapped on a debugger, do we?
