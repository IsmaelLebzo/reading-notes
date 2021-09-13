# React: Component Lifecycle Events
![React: Component Lifecycle Events](https://miro.medium.com/max/2000/0*pqn5ljaOw4kWrUdF)
## What are component lifecycle events?
Components can be defined as classes or functions in React. The methods you can use on these are referred to as lifecycle events. These methods are available throughout a component's lifespan and allow you to alter the UI and application states.
![image](https://miro.medium.com/max/2000/0*0saPKFiTUk6W3FYp)

The three steps of the component lifetime are mounting, updating, and unmounting.

### Mounting
It is during the mounting step that an instance of a component is generated and put into the DOM. During mounting, the constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE componentWillMount are all called in this order.

### Updating
It is rerendered whenever a component is changed or its state changes. These lifecycle events occur in this order when updating.\
static getDerivedStateFromProps, shouldComponentUpdate, render,
getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps

### Unmounting
When a component is removed from the DOM, the last phase of the lifecycle is invoked. During this phase, componentWillUnmount is the single lifecycle event.

constructor()\
A React component's constructor is called before it is mounted.
If the component is a subclass, super(props) must be called else the props will be undefined. Constructors can be used to tie event handling methods to an instance or to assign state using this.state. Let's have a peek at some code in action.\

render()\
In a class component, only the render method is necessary. This will be looked into. When called, props and this.state are available. The render method should not change the component state because doing so every time it rerenders will result in a slew of problems. I should also avoid interacting with the browser directly. If shouldComponentUpdate() returns false, render will not be called. Here's an example of how to use render.

### UNSAFE Lifecycle Events

UNSAFE_componentWillMount()\
UNSAFE_componentWillUpdate()\
UNSAFE_componentWillReceiveProps()

Because these events have resulted in several problems and unexpected side effects, they will no longer be used without the UNSAFE tag in front of them in React 17. Use ComponentDidMount instead of componentWillMount.
Use static getDerivedStateFromProps instead of componentWillReceiveProps.
We'll use getSnapshotBeforeUpdate instead of componentWillUpdate.