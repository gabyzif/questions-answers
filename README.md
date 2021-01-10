# questions-answers
Useful js / react /cheat sheet for interviews and life darling. :star_struck:	

## Javascript

+ **Difference let const var**

- var declarations are globally scoped or function scoped while let and const are block scoped.
- var variables can be updated and re-declared within its scope; let variables can be updated but not re-declared; const variables can neither be updated nor re-declared.
- They are all hoisted to the top of their scope. But while var variables are initialized with undefined, let and const variables are not initialized.
- While var and let can be declared without being initialized, const must be initialized during declaration.

+ **Prototype Inheritance**

All JavaScript objects inherit properties and methods from a prototype:

Date objects inherit from Date.prototype
Array objects inherit from Array.prototype
Person objects inherit from Person.prototype
The Object.prototype is on the top of the prototype inheritance chain:

Date objects, Array objects, and Person objects inherit from Object.prototype.


+ **Event Loop**

The Event Loop has one simple job — to monitor the Call Stack and the Callback Queue. If the Call Stack is empty, it will take the first event from the queue and will push it to the Call Stack, which effectively runs it.

More info: [https://www.educative.io/edpresso/what-is-an-event-loop-in-javascript](https://www.educative.io/edpresso/what-is-an-event-loop-in-javascript)


+ **Difference between map and foreach**


**Foreach**:

Executes a provided function once for each array element.
Simple iteration.
It does not returns anything.


**Map**

Creates an array and excecutes a provided function once for each element in the array.
Returns an array :sunglasses:	
