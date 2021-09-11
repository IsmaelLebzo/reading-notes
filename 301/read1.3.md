# Introduction to React and Components
![Introduction to React and Components](https://www.innoraft.com/sites/default/files/styles/blog_original_size/public/2019-09/Screenshot%20from%202019-09-17%2014-05-24.png)
## Component-Based Architecture
The breakdown of the design into distinct functional or logical components that represent well-defined communication interfaces comprising methods, events, and attributes is the emphasis of component-based architecture. It gives the issue a higher degree of abstraction and separates it into sub-problems, each with its own set of component divisions.\
The fundamental goal of component-based architecture is to ensure that components may be reused. A component is a reusable and self-deployable binary unit that contains the functionality and behaviors of a software element. Component frameworks such as COM/DCOM, JavaBean, EJB, CORBA,.NET, web services, and grid services are all common. Graphic JavaBean components, MS ActiveX components, and COM components, all of which can be reused by simply dragging and dropping, are frequently utilized in local desktop GUI program design.\
The advantages of component-oriented software architecture over standard object-oriented techniques include:
- By reusing existing components, the time to market and development costs are reduced.

- Reusability of existing components improves dependability.
### What is a Component?
A component is a well-defined collection of modular, portable, replaceable, and reusable functionality that wraps and exports its implementation as a higher-level interface.\
A component is a software object that encapsulates specific functionality or a collection of functions and is designed to interact with other components. It has a well defined interface and follows a suggested behavior that other components in an architecture should follow.
### Characteristics of Components
- Components are often intended to be reused in a variety of scenarios across a variety of applications. Some components, on the other hand, may be tailored to a specific purpose.

- Components that are replaceable can be swapped out for others that are comparable.

- It is not context-specific. Components are made to work in a variety of settings and situations.

- Extensible: A component's behavior may be expanded by combining it with that of other components.

- An encapsulated an encapsulated an encapsulated A component shows the interfaces that allow the caller to access its functionality, but it does not reveal any underlying processes, variables, or state.

- Independent Components are created with the goal of having as little dependencies as possible on other components.

## What is Props?
React is a component-based framework that breaks down the user interface into smaller, reusable chunks. In some situations, those components may need to communicate (transfer data to one another), and the best method to do so is to use props.\
In React, “props” is a specific term that stands for properties and is used to transmit data from one component to another.\
The essential thing to note here is that data with props is passed in a one-way flow. Props data is also read-only, which implies that data from the parent should not be modified by child components.
### Using Props in React
Step-by-step instructions on how to utilize Props will be provided.\
1. To begin, specify an attribute and its value(data).
2.  Then, using Props, give it to the child component(s).
3. Last but not least, render the Props Data.

Props is a unique keyword in React that stands for properties.\
Components are given props, such as function arguments.\
Only one-way props can be passed to components (parent to child)
The data in the props is unchangeable (read-only).

Conclusion
It takes time to grasp React's approach to data manipulation.