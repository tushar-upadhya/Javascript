# Javascript

Q1. What are the primitive data types in JS?

Ans. In JavaScript, a primitive (primitive value, primitive data type) is data that is not an object and has no methods or properties. these are predefined data types. There are 7 primitive data types: 1.string. 2.number. 3.bigint. 4.boolean. 5.undefined. 6.symbol. 7.null.

Q2. What's the difference between a variable that is: null, undefined or undeclared?

Ans. Undeclared: It occurs when we try to access any variable that is not initialized or declared earlier using var or const keyword. Undefined: It occurs when a variable has been declared but has not been assigned with any value. Null: The null value represents the intentional absence of any object value. It is one of JavaScript's primitive values and is treated as falsy for boolean operations.

Q3. What is the difference between while and do-while loops in JavaScript?

Ans. The while loop in java executes one or more statements after testing the loop continuation condition at the start of each iteration. The do-while loop, however, tests the loop continuation condition after the first iteration has completed.

Q4. What language constructions do you use for iterating over object properties and array items?

Ans. for loop, for..in, for each..in, map, reduce etc.

Q5. What are the promises and how do they work?

Ans. The Promise object represents the eventual completion (or failure) of an asynchronous operation and its resulting value.They are easy to manage when dealing with multiple asynchronous operations where callbacks can create callback hell leading to unmanageable code. A Promise is in one of these states: 1.pending: initial state, neither fulfilled nor rejected. 2.fulfilled: meaning that the operation was completed successfully. 3.rejected: meaning that the operation failed.

Q6. What are IIFEs and explain with an example where they can be used?

Ans. An IIFE (Immediately Invoked Function Expression) is a JavaScript function that runs as soon as it is defined. The name IIFE is promoted by Ben Alman in his blog. (function () { // … })();

            (() => {
            // …
            })();

            (async () => {
            // …
            })();
It is a design pattern which is also known as a Self-Executing Anonymous Function and contains two major parts:

1.The first is the anonymous function with lexical scope enclosed within the Grouping Operator (). This prevents accessing variables within the IIFE idiom as well as polluting the global scope. 2.The second part creates the immediately invoked function expression () through which the JavaScript engine will directly interpret the function. Use cases-- 1.Avoid polluting the global namespace 2.Execute an async function 3.The module pattern

Q7. Explain event delegation.

Ans. Event Delegation is a pattern based upon the concept of Event Bubbling. It is an event-handling pattern that allows you to handle events at a higher level in the DOM tree other than the level where the event was first received.

Q8. Explain how this works in JavaScript. a.Can you give an example of one of the ways that working with this has changed in ES6?

Ans. 'This' keyword in javascript always holds the reference to a single object, that defines the current line of code’s execution context. Functions, in JavaScript, are essentially objects. Like objects, they can be assigned to variables, passed to other functions, and returned from functions. And much like objects, they have their own properties. One of these properties is this.
ES6 allows you to use arrow functions which uses the enclosing lexical scope. This is usually convenient, but does prevent the caller from controlling context via .call or .apply—the consequences being that a library such as jQuery will not properly bind this in your event handler functions. Thus, it's important to keep this in mind when refactoring large legacy applications.

Q9. Explain how prototypal inheritance works.?

Ans. Every object with its methods and properties contains an internal and hidden property known as "Prototype". The Prototypal Inheritance is a feature in javascript used to add methods and properties in objects. It is a method by which an object can inherit the properties and methods of another object. Traditionally, in order to get and set the "Prototype" of an object, we use Object.getPrototypeOf and Object.

Q10. What is a closure, and how/why would you use one?

Ans. A closure is the combination of a function bundled together (enclosed) with references to its surrounding state (the lexical environment). In other words, a closure gives you access to an outer function's scope from an inner function. Why would we use... 1.Data privacy / emulating private methods with closures. Commonly used in the module pattern. 2.Partial applications or currying.

Q11. Can you describe the main difference between the Array.forEach() loop and Array.map() methods and why you would pick one versus the other?

Ans.
