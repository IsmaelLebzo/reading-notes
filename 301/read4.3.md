# React and Forms
![image](https://answerjs.com/wp-content/uploads/2021/06/react-forms.png)

# Forms

Because form elements inherently maintain some internal information, they behave differently in React than other DOM elements. In basic HTML, for example, this form takes only one name:\
< form>\
  < label>\
    Name:\
    < input type="text" name="name" />\
  </ label>\
  < input type="submit" value="Submit" />\
</ form>

When the user accepts the form, the normal HTML form action is for the user to be sent to a new page. It merely works with React if you desire this behavior. However, in most situations, it's more convenient to have a JavaScript function that handles form submission and has access to the data supplied by the user. The most common method is to use a technique known as "controlled components."

## Controlled Components

Form components like input, textarea, and select in HTML generally keep their own state and change it based on user input. In React, mutable state is generally stored in component state and only changed using setState ().

By making the React state the "one source of truth," we may integrate the two. The React component that renders a form then has control over what happens in that form when the user enters data. A "controlled component" is an input form element whose value is managed by React in this way.

The value of the input in a controlled component is always determined by the React state. While you'll have to enter a little more code as a result, you'll be able to send the value to other UI components and reset it from other event handlers.

## Handling Multiple Inputs

When dealing with numerous controlled input elements, you may give each one a name attribute and allow the handler function decide what to do based on the value of event.target.name.

## Controlled Input Null Value

If you specify the value prop on a controlled component, the user will not be able to change the input unless you want them to. If you specify a value yet the input remains editable, you may have set value to undefined or null by accident.

## Alternatives to Controlled Components

Because you must build an event handler for every method your data might change and route all of the input information via a React component, using controlled components can be laborious at times. When converting an old codebase to React or integrating a React application with a non-React library, this may be extremely aggravating. In these cases, you might want to consider using uncontrolled components, a different approach to designing input forms.

--------

# The Conditional (Ternary) Operator Explained

## Starting With the Basics — The if statement

When we use a conditional, such as an if statement, we may indicate that a certain block of code should be run if a specific condition is fulfilled.

Consider the following illustration:\
A person object is made up of a name, an age, and a driving attribute.

let person = {\
  name: 'tony',\
  age: 20,\
  driver: null\
};

We'd want to see if our person's age is more than or equal to 16. If this is correct, they are of legal driving age, and the driver should respond affirmatively. Driver should be set to 'No' if this is not the case.

We could use an if statement to accomplish this:\
if (person.age >= 16) {\
  person.driver = 'Yes';\
} else {\
  person.driver = 'No';\
}

## The Conditional (Ternary) Operator

We'll start by looking at the syntax of a standard if statement:

if ( condition ) {\
  value if true;\
} else {\
  value if false;\
}

Now, the ternary operator:\
condition ? value if true : value if false

## Here’s what you need to know:

1. The condition is what you're putting to the test. Your condition's outcome should be true or false, or at the very least coerce to either boolean value.
2. Our conditional value is separated from our real value by a? If the condition evaluates to true, anything between the? and the : is performed.
3. Finally, a colon (:). Any code following the colon is executed if your condition evaluates to false.

## Example — Multiple operations

Within a ternary, you may also perform several operations. To do so, we must use a comma to separate the procedures. Optionally, you may use parentheses to assist organize your code:

let isStudent = true;\
let price = 12;\
isStudent ? (\
  price = 8,\
  alert('Please check for student ID')\
) : (\
  alert('Enjoy the movie')\
);

Our movie's pricing is already set to $12 in the example above. If isStudent is true, we reduce the price to $8 and send an alert to the cashier, instructing them to check for student ID. The preceding code is bypassed if isStudent is false, and we just alert to watch the movie.