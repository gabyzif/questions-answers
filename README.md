# questions-answers
Useful js / react /cheat sheet for interviews and life darling. :star_struck:	

## Javascript

**Difference let const var**

- var declarations are globally scoped or function scoped while let and const are block scoped.
- var variables can be updated and re-declared within its scope; let variables can be updated but not re-declared; const variables can neither be updated nor re-declared.
- They are all hoisted to the top of their scope. But while var variables are initialized with undefined, let and const variables are not initialized.
- While var and let can be declared without being initialized, const must be initialized during declaration.


**Prototype Inheritance**

All JavaScript objects inherit properties and methods from a prototype:

Date objects inherit from Date.prototype
Array objects inherit from Array.prototype
Person objects inherit from Person.prototype
The Object.prototype is on the top of the prototype inheritance chain:

Date objects, Array objects, and Person objects inherit from Object.prototype.


**Event Loop**

The Event Loop has one simple job — to monitor the Call Stack and the Callback Queue. If the Call Stack is empty, it will take the first event from the queue and will push it to the Call Stack, which effectively runs it.

More info: [https://www.educative.io/edpresso/what-is-an-event-loop-in-javascript](https://www.educative.io/edpresso/what-is-an-event-loop-in-javascript)

**Event Delegation**

JavaScript event delegation is a simple technique by which you add a single event handler to a parent element in order to avoid having to add event handlers to multiple child elements.

**Event Bubbling**

When an event happens on an element, it first runs the handlers on it, then on its parent, then all the way up on other ancestors.


**Difference between map and foreach**


**Foreach**:

Executes a provided function once for each array element.
Simple iteration.
It does not returns anything.


**Map**

Creates an array and excecutes a provided function once for each element in the array.
Returns an array :sunglasses:	


## React

JSX stands for JavaScript XML. JSX allows us to write HTML in React. JSX makes it easier to write and add HTML in React.
Instead of artificially separating technologies by putting markup and logic in separate files, it creates components that have both.


**Props vs state**
Props are inmutable vs state that suffers from mutations in time (mostly generated from user events).

**Context**
Context provides a way to pass data through the component tree without having to pass props down manually at every level.

**Bundling**
Most React apps will have their files “bundled” using tools like Webpack, Rollup or Browserify. Bundling is the process of following imported files and merging them into a single file: a “bundle”. This bundle can then be included on a webpage to load an entire app at once.

**Code splitting**
To avoid winding up with a large bundle, it’s good to get ahead of the problem and start “splitting” your bundle. Code-Splitting is a feature supported by bundlers like Webpack, Rollup and Browserify (via factor-bundle) which can create multiple bundles that can be dynamically loaded at runtime.

The React.lazy function lets you render a dynamic import as a regular component.

**Virtual dom vs real dom**
The Virtual DOM is an abstraction of the HTML DOM. ... It allows React to do its computations within this abstract world and skip the “real” DOM operations, often slow and browser-specific. There's no big difference between the “regular” DOM and the virtual DOM

Most JavaScript frameworks update the entire DOM even when a small part of the DOM changes.
To address the problem of inefficient updating, the react team introduced the concept of virtual DOM.

For every DOM object, there is a corresponding virtual DOM object(copy), which has the same properties.
The main difference between the real DOM object and the virtual DOM object is that any changes in the virtual DOM object will not reflect on the screen directly. Consider a virtual DOM object as a blueprint of the real DOM object.
Whenever a JSX element gets rendered, every virtual DOM object gets updated.


**Keys**
Keys in React are used to identify unique VDOM Elements with their corresponding data driving the UI; having them helps React optimize rendering by recycling existing DOM elements. Let’s look at an example to portray this.

**Refs**

Similarly to keys, refs are added as an attribute to a React.createElement() call, such as <li ref="someName"/>. The ref serves a different purpose, it provides us quick and simple access to the DOM Element represented by a React Element.

**Hooks**
React Hooks are functions that let us hook into the React state and lifecycle features from function components.
By this, we mean that hooks allow us to easily manipulate the state of our functional component without needing to convert them into class components.

Hooks rules: Don’t call Hooks inside loops, conditions, or nested functions — Only call Hooks at the top level.
Don’t call Hooks from regular JavaScript functions — Only call Hooks from React function components.


**What are the differences between functional and class components?**
Before the introduction of Hooks in React, functional components were called stateless components and were behind class components on feature basis. After the introduction of Hooks, functional components are equivalent to class components.


**What are the different lifecycle methods in React?**
Every component in React has lifecycle methods that we can tap into, to trigger changes at a particular phase of the life cycle.
Each component in react goes through three phases: Mounting, Updating, and Unmounting.
There are corresponding lifecycle methods for each of the three phases

**Strickt mode**

StrictMode is a tool added in the version 16.3 of React to highlight potential problems in an application. It performs additional checks on the application.

**How to prevent re rendering ? **

React.memo(component)


**React State**
Every component in react has a built-in state object, which contains all the property values that belong to that component.
In other words, the state object controls the behaviour of a component. Any change in the property values of the state object leads to re-rendering of the component.



