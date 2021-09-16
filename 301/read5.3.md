# Putting it all together
![image](https://hashrouter.in/wp-content/uploads/2020/05/think-in-react.png)

## Thinking in React
React is, in our opinion, the best method to use JavaScript to create large, fast Web apps. For us at Facebook and Instagram, it has scaled really effectively.

React's ability to make you think about apps as you develop them is one of its many strengths. We'll guide you through the thinking process of creating a searchable product data table using React in this paper.

## Step 1: Break The UI Into A Component Hierarchy
The first step is to create boxes around each component (and subcomponent) in the mockup and give them their names. If you're working with a designer, it's possible that they've already done this, so ask them! It's possible that the names of their Photoshop layers will wind up becoming the names of your React components!

But how can you determine which components should be on their own? Use the same methods to determine whether or not to construct a new function or object. The single responsibility concept, which states that a component should ideally only do one thing, is one such method. It should be split into smaller subcomponents if it grows.

Because you'll be showing a JSON data model to a user frequently, your UI (and hence your component structure) will translate neatly if your model was created appropriately. Because UI and data models tend to follow the same information architecture, this is the case. Separate your UI into components, each of which corresponds to a different part of your data model.

## Step 2: Build A Static Version in React

You'll want to construct components that reuse other components and pass data using props to create a static version of your app that renders your data model. Props are a means for data to be sent from a parent to a child. If you're familiar with the idea of state, you shouldn't utilize it to create this static version. Only interactivity, or data that varies over time, is allowed to use state. You don't need it because this is a static version of the program.

## Step 3: Identify The Minimal (but complete) Representation Of UI State

You must be able to make modifications to your underlying data model in order to make your UI interactive. With state, React does this.

To properly construct an app, you must first consider the bare minimum of mutable state that it requires. DRY is the important word here: Don't make the same mistake twice. Calculate anything else you need on-demand after determining the absolute minimum representation of the state your application requires. Retain an array of TODO items around if you're making a TODO list; don't keep a distinct state variable for the count. Instead, take the length of the TODO items array when rendering the TODO count.

## Step 4: Identify Where Your State Should Live

Keep in mind that React is based on one-way data flow along the component hierarchy. It's not always apparent which component should be in charge of particular state. This is typically the most difficult element for newbies to grasp, so follow these steps to figure it out:

For each state in your application, write:

- Determine which components render something depending on that state.
- Look for a component with a common owner (a single component above all the components that need the state in the hierarchy).
- The state should be owned by either the common owner or another component further up in the hierarchy.
- If you can't find a component that makes sense to own the state, develop a new component dedicated to keeping the state and place it above the common owner component in the hierarchy.

Let's have a look at our application's strategy:

- ProductTable must filter the product list by state, and SearchBar must show the search phrase as well as the checked state.
- FilterableProductTable is the common owner component.
- FilterableProductTable is a natural place for the filter text and checked value to live.

## Step 5: Add Inverse Data Flow

So far, we've created an app that renders properly as props and state move down the hierarchy. Now it's time to allow data flow in the opposite direction: deep in the hierarchy, form components must change the state of FilterableProductTable.

This data flow is made explicit in React to help you understand how your application works, but it does need a bit more typing than typical two-way data binding.

Let's consider what we'd want to happen. We want to ensure that anytime the user makes a modification to the form, the state is updated to reflect the changes. FilterableProductTable will pass callbacks to SearchBar that will trigger anytime the state should be modified, because components should only update their own state. To be alerted of it, we may utilize the onChange event on the inputs. FilterableProductTable's callbacks will call setState(), and the app will be updated.

# Higher-order functions
![image](https://res.cloudinary.com/practicaldev/image/fetch/s--ubo7JUyn--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/i/uuhsczcbn8gdbpewmoe6.jpeg)

Higher-order functions are functions that operate on other functions by accepting them as arguments or returning them. Because we've previously shown that functions are regular values, the fact that they exist isn't especially noteworthy. The word is derived from mathematics, where the difference between functions and other values is more carefully considered.

Higher-order functions are functions that operate on other functions by accepting them as arguments or returning them. Because we've previously shown that functions are regular values, the fact that they exist isn't especially noteworthy. The word is derived from mathematics, where the difference between functions and other values is more carefully considered.

## Script data set

Despite the fact that I can only read Latin letters fluently, I enjoy the fact that individuals are producing texts in at least 80 different writing systems, many of which I am unfamiliar with.

The sample data collection includes some details about the 140 scripts specified by Unicode. The SCRIPTS binding is accessible in the coding sandbox for this chapter. The binding is made up of an array of objects, each of which is a script.

## Filtering arrays

The following function may be useful for locating scripts that are still in use in the data collection. It removes elements from an array that fail to pass a test.\
function filter(array, test) {\
  let passed = [];\
  for (let element of array) {\
    if (test(element)) {\
      passed.push(element);\
    }\
  }\
  return passed;\
}\

console.log(filter(SCRIPTS, script => script.living));\
// → [{name: "Adlam", …}, …]
The function fills a "gap" in the computation—the process of choosing which elements to collect—with the parameter test, a function value.

Rather of removing entries from the existing array, the filter method creates a new array with just the elements that pass the test. This is a pure function. It makes no changes to the array it is given.

## Summary
The ability to transfer function values to other functions is one of JavaScript's most valuable features. It enables us to build functions that simulate computations with "gaps." The code that invokes these functions can provide function values to fill in the gaps.

A variety of interesting higher-order techniques are available in arrays. You may use forEach to cycle over an array's elements. Only the elements that pass the predicate function are returned by the filter method, which creates a new array. Map is used to transform an array by passing each element through a function. Reduce can be used to condense an array's items into a single value. The some method examines each element to see whether it fits a specified predicate function. The location of the first element that meets a predicate is determined by findIndex.