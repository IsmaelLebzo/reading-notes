# FUNCTIONAL PROGRAMMING

![image](https://miro.medium.com/max/1400/1*3wp2A9xFW7LbCKFA_X2-sw.png)

## Concepts of Functional Programming in Javascript

Functional Programming is a style of programming. It follows the declarative pattern, which means it concentrates on what the program intends to do rather than how it will accomplish it. JavaScript, in particular, cannot be compared to functional languages such as Haskell, Erlang, Elm, and others, but it does a good job of supporting the functional paradigm. We design the application architecture and create code using just functions when we use functional programming. For data processing, concurrent, high-critical, and serverless systems, functional programming is ideal.

With the use of basic code examples, we'll go through the following functional programming principles in JavaScript:

- Immutability
- Referential Transparency
- Pure Functions
- Higher-order functions;
- First-class functions

## Why functional programming matters?

- Readable
- Concise
- Testable
- Enables Concurrency
- Robust

Small modules may be coded fast and simply using Functional Programming. It is one of the paradigm's key advantages. Furthermore, Functional Programming is far more succinct than Object-Oriented Programming. It encourages programmers to write code in the sequence of operations, which is more logical. Pure functions are more predictable in Functional Programming than impure functions. Pure functions in functional programming are predictable since their input is the only thing they depend on, and all they do is return their result. It's therefore safer, and it's more difficult to add flaws into your code. It also makes it easy to test programs and discover issues if they arise.

## Pure functions

Given the same parameters, the pure function gives the same result. From the outside, it doesn't look at anything else. It just returns the results of its operation. It has no other impact on the rest of the globe. Additional than returning their return value, pure functions make no other modifications.\
In Functional Programming, there is a concept known as side-effects. A side-effect occurs when a function not only returns a value but also alters something in the background. When a function executes, it has the potential to alter anything. You must prevent side effects to the greatest extent feasible. Sometimes it's necessary to have side effects.

Always attempt to keep the scope of each variable as little as possible. It means that every variable you create should have the lowest feasible scope and that you should localize your variables as much as possible.

## Immutability

The idea of immutability has its origins in Functional Programming. Instead of altering the existing object, we should receive a new one with the updated data whenever we wish to make changes to it. Immutability is similar to "save as" in that it yields a new object, but typical in-place mutation is similar to "save" in that it updates the original while discarding the previous state. It provides you more control over your data, making your code safer and more predictable right away.

## Higher-order functions

Higher-order functions are functions that take or return arguments from other functions.

In Functional Programming, a higher-order function is a key notion. These methods enable you to construct code that is both simpler and more elegant. We can eliminate errors and make our code easier to read and comprehend by using higher-order functions.

## Conclusion

Functional Programming is quickly becoming the industry standard for developing and maintaining JavaScript applications. The concepts presented in this post will enable you to use Functional Programming and produce cleaner code. Recursion, monads, functors, lambda, monoid, curry, and other Functional Programming topics are not covered in this article. Because they are fairly sophisticated, they were left out of this article. Understanding these functional programming ideas will give you a significant advantage.
