# 📚 59 Must-Know JavaScript Interview Questions and Answers

This repository contains detailed and organized answers to the 59 most important JavaScript interview questions.  
Designed to help you prepare confidently for your next interview!

---

# 📖 Table of Contents

## 🟢 Basics
- [What are the different data types in JavaScript?](#what-are-the-different-data-types-in-javascript)
- [Difference between var, let, and const](#difference-between-var-let-and-const)
- [How does type coercion work?](#how-does-type-coercion-work)
- [What are truthy and falsy values?](#what-are-truthy-and-falsy-values)
- [Difference between == and ===](#difference-between--and-)
- [How do functions work in JavaScript?](#how-do-functions-work-in-javascript)
- [Function declarations vs. expressions](#function-declarations-vs-expressions)
- [Arrow functions vs. regular functions](#arrow-functions-vs-regular-functions)
- [What is the value of `this` in different contexts?](#what-is-the-value-of-this-in-different-contexts)
- [What is hoisting?](#what-is-hoisting)
- [What is lexical scope?](#what-is-lexical-scope)
- [Arrays vs. objects](#arrays-vs-objects)
- [Template literals](#template-literals)
- [Destructuring](#destructuring)
- [Default parameters in functions](#default-parameters-in-functions)

## ⚙️ Functions & Scope
- [What is a higher-order function?](#what-is-a-higher-order-function)
- [What is a closure?](#what-is-a-closure)
- [What is currying?](#what-is-currying)
- [What is a callback function?](#what-is-a-callback-function)
- [What is callback hell and how to avoid it?](#what-is-callback-hell-and-how-to-avoid-it)
- [call(), apply(), and bind() differences](#call-apply-and-bind-differences)
- [Arrow functions vs. bind() for this](#arrow-functions-vs-bind-for-this)
- [What is an IIFE?](#what-is-an-iife)
- [Scope vs. lexical scope](#scope-vs-lexical-scope)

## 🧩 Control Flow & Iteration
- [for, for...in, vs. for...of](#for-forin-vs-forof)
- [map(), forEach(), filter() differences](#map-foreach-filter-differences)
- [Use cases of map(), filter(), reduce()](#use-cases-of-map-filter-reduce)

## 🌐 DOM & Events
- [What is the DOM and how to manipulate it?](#what-is-the-dom-and-how-to-manipulate-it)
- [Event bubbling vs. capturing](#event-bubbling-vs-capturing)
- [Event delegation](#event-delegation)

## 🔁 Async & Execution Model
- [Synchronous vs. asynchronous code](#synchronous-vs-asynchronous-code)
- [What is the Event Loop?](#what-is-the-event-loop)
- [Microtasks vs. macrotasks](#microtasks-vs-macrotasks)
- [What is a Promise?](#what-is-a-promise)
- [How async/await works?](#how-asyncawait-works)
- [How setTimeout() and setInterval() work?](#how-settimeout-and-setinterval-work)
- [Purpose of Promise.all(), Promise.any(), and Promise.race()](#purpose-of-promiseall-promiseany-and-promiserace)

## 🧠 Concepts & Patterns
- [What is immutability?](#what-is-immutability)
- [What is a pure function?](#what-is-a-pure-function)
- [What is optional chaining (?.)?](#what-is-optional-chaining-)
- [What is nullish coalescing (??)?](#what-is-nullish-coalescing-)
- [Shallow copy vs. deep copy](#shallow-copy-vs-deep-copy)
- [Truthy and falsy values (with examples)](#truthy-and-falsy-values-with-examples)
- [JavaScript modules: import/export](#javascript-modules-importexport)
- [Error handling with try/catch/finally](#error-handling-with-trycatchfinally)
- [What is the typeof operator?](#what-is-the-typeof-operator)

## 💡 Advanced JavaScript
- [What is the prototype chain?](#what-is-the-prototype-chain)
- [Memory management & garbage collection](#memory-management--garbage-collection)
- [Object.freeze() vs. Object.seal()](#objectfreeze-vs-objectseal)
- [Object.keys(), values(), entries()](#objectkeys-values-entries)
- [What is a memory leak and how to avoid it?](#what-is-a-memory-leak-and-how-to-avoid-it)
- [What are WeakMap and WeakSet?](#what-are-weakmap-and-weakset)
- [Stack vs. heap memory](#stack-vs-heap-memory)
- [Debouncing vs. throttling](#debouncing-vs-throttling)
- [How the new keyword works](#how-the-new-keyword-works)
- [Common JS design patterns](#common-js-design-patterns)
- [Deep equality vs. strict equality](#deep-equality-vs-strict-equality)
- [How the JS engine works internally?](#how-the-js-engine-works-internally)
- [Generators vs. iterators](#generators-vs-iterators)

---

# 🧑‍💻 Maintainer

Maintained by [Maksuda Akter Suborno].

---

## 🟢 Basics

### 1. What are the different data types in JavaScript?
<a id="what-are-the-different-data-types-in-javascript"></a>
JavaScript provides different data types including:
- Primitive types: String, Number, Boolean, Null, Undefined, Symbol, BigInt
- Non-primitive types: Objects (including Arrays, Functions, etc.)

---

### 2. Difference between var, let, and const
<a id="difference-between-var-let-and-const"></a>
- `var` is function-scoped, can be re-declared and updated.
- `let` is block-scoped, can be updated but not re-declared in the same scope.
- `const` is block-scoped, cannot be updated or re-declared after initialization.

---

### 3. How does type coercion work?
<a id="how-does-type-coercion-work"></a>
- Type coercion in JavaScript refers to the automatic or implicit conversion of one data type to another. This occurs when JavaScript expects a value of a certain type but encounters a different one, and the language tries to convert it to the expected type.

There are two types of type coercion:

- Implicit Coercion: Automatically done by JavaScript when an operation involves different types.

- Explicit Coercion: When you manually convert one type to another using functions like String(), Number(), Boolean(), etc.

---

### 4. What are truthy and falsy values?
<a id="what-are-truthy-and-falsy-values"></a>
- Falsy Values:
These are the values that are considered false when coerced into a Boolean. There are only 6 falsy values in JavaScript:

-false (the Boolean false), 0 (zero), "" (empty string), null, undefined, NaN (Not-a-Number)

- Truthy Values:
All values except the falsy ones are considered truthy. This means that any value that is not falsy will be treated as true in a Boolean context.

-For example: Non-empty strings (e.g., "Hello"), Non-zero numbers (e.g., 1, -1, 3.14), Objects (including arrays, functions, etc.), true (the Boolean true), Infinity (positive and negative infinity), Dates (e.g., new Date())

---

### 5. Difference between == and ===
<a id="difference-between--and-"></a>
In JavaScript, == and === are comparison operators used to compare values, but they behave differently:

- == (Equality/Loose Comparison):
The == operator compares two values for equality after performing type coercion (i.e., it converts the values to a common type before making the comparison).
- === (Strict Equality/Strict Comparison):
The === operator compares both value and type. It does not perform type coercion, meaning both the values and their types must be the same for the comparison to return true.

---

### 6. How do functions work in JavaScript?
<a id="how-do-functions-work-in-javascript"></a>

In JavaScript, functions are blocks of code designed to perform a particular task. You define a function once, and then you can execute (call) it whenever you want. 
- Defining a Function: 
You can define a function in JavaScript using the function keyword followed by the function name, parameters (optional), and a block of code.
```javascript
function greet(name) {
  console.log('Hello, ' + name + '!');
}
```
In this example, the function is named 'greet', and it takes one parameter (name). Inside the function body, it prints a greeting message to the console.

- Calling a Function: 
To call a function, you use its name followed by parentheses, passing any required arguments inside the parentheses.

```javascript
greet('Alice');  // Output: Hello, Alice!
greet('Bob');    // Output: Hello, Bob!
```

- Return Values:
Functions can return values using the 'return' keyword. When a function returns a value, it can be used in other expressions.
```javascript
function add(a, b) {
  return a + b;
}

let sum = add(3, 4);  // sum = 7
console.log(sum);      // Output: 7
```

- Function Expressions: 
You can also define functions as expressions. This is common for passing functions as arguments or returning them from other functions. Here’s an example:
```javascript
const multiply = function(a, b) {
  return a * b;
};

console.log(multiply(2, 5));  // Output: 10
```

- Arrow Functions:
ES6 introduced arrow functions, which are a shorter syntax for writing functions. Arrow functions are particularly useful for short functions and when you want to avoid issues with the 'this' keyword.
```javascript
const square = (x) => x * x;
console.log(square(5));  // Output: 25
```

Parameters and Arguments: 
- Parameters are the names used in the function definition (like name in the greet function).

- Arguments are the values passed into the function when calling it (like 'Alice' or 'Bob' in the example above).

You can have default parameters, rest parameters, and even handle arguments using the arguments object for non-named parameters.

---

### 7. Function declarations vs. expressions
<a id="function-declarations-vs-expressions"></a>

Function Declarations:

- Defined using the function keyword followed by the function name.

- Hoisted, meaning they can be called before they are defined in the code.

```javascript
function greet() {
  console.log('Hello!');
}
```

Function Expressions:

- Defined as part of an expression (can be anonymous or named).

- Not hoisted; they must be defined before being called.

```javascript
const greet = function() {
  console.log('Hello!');
};
```

---

### 8. Arrow functions vs. regular functions
<a id="arrow-functions-vs-regular-functions"></a>

Arrow Functions:

- Shorter syntax: () => {}.

- Do not have their own 'this'; they inherit this from the surrounding context (lexical scoping).

- Cannot be used as constructors (i.e., they don’t support new keyword).

- Cannot have the arguments object.

```javascript
const greet = (name) => console.log('Hello, ' + name);
```

Regular Functions:

- Use the function keyword and have their own 'this'.

- Can be used as constructors (with new keyword).

- Have their own arguments object.

```javascript
function greet(name) {
  console.log('Hello, ' + name);
}
```

---

### 9. What is the value of `this` in different contexts?
<a id="what-is-the-value-of-this-in-different-contexts"></a>
The value of this in JavaScript varies depending on the context in which it is used.

Global Context (Outside any function or object):
- In non-strict mode, 'this' refers to the global object (window in browsers or global in Node.js).

- In strict mode, this is undefined.

```javascript
console.log(this); // In non-strict mode: window (browser)
```

Function Context:
- In a regular function, 'this' refers to the global object in non-strict mode and undefined in strict mode.

```javascript
function example() {
  console.log(this); // Non-strict: global object, strict: undefined
}
example();

```

Method Context (Inside an object):
- Inside a method of an object, this refers to the object that the method is called on.

```javascript
const person = {
  name: 'Alice',
  greet: function() {
    console.log(this.name); // 'this' refers to 'person'
  }
};
person.greet(); // Output: Alice
```

Arrow Functions:
- Arrow functions do not have their own 'this'. Instead, they inherit 'this' from their enclosing lexical context (the scope in which they were defined).

```javascript
const person = {
  name: 'Alice',
  greet: () => {
    console.log(this.name); // 'this' refers to the outer context, not 'person'
  }
};
person.greet(); // Output: undefined (if in global scope)
```

Constructor Functions:
- When using a constructor function (called with new), this refers to the newly created object.

```javascript
function Person(name) {
  this.name = name;
}
const person1 = new Person('Alice');
console.log(person1.name); // Output: Alice
```

Event Handlers:
- In event handlers, 'this' refers to the DOM element that the event is triggered on.

```javascript
const button = document.querySelector('button');
button.addEventListener('click', function() {
  console.log(this); // 'this' refers to the button element
});

```

Explicit Binding (call(), apply(), bind()):
- You can explicitly bind this to any value using call(), apply(), or bind().

```javascript
function greet() {
  console.log(this.name);
}

const person = { name: 'Alice' };
greet.call(person); // Output: Alice
```

---

### 10. What is hoisting?
<a id="what-is-hoisting"></a>

Hoisting in JavaScript refers to the behavior where declarations (but not initializations) of variables and functions are moved to the top of their containing scope during the execution phase, before any code is actually run. This allows you to reference variables or call functions before they are defined in the code.

- <b>Variables</b>: var declarations are hoisted (initialized as undefined), while let and const are hoisted but not initialized.
- Functions: Function declarations are hoisted with their implementation, but function expressions are hoisted only with the variable declaration, causing errors if called before assignment.

---

### 11. What is lexical scope?
<a id="what-is-lexical-scope"></a>

-Lexical scope in JavaScript means that a function's ability to access variables is determined by where it was physically written in the code.

- In other words, when you write a function, it "remembers" the environment where it was created, and it can access variables from that environment.

```javascript
function outer() {
  let outerVar = "I am from outer!";

  function inner() {
    console.log(outerVar); // ✅ inner can access outerVar
  }

  inner();
}

outer();
```
- inner() can access outerVar because it was written inside outer().

- That's lexical scope — based on the position of code, not on how or where the function is called later.

Key point:
- JavaScript looks at where a function was defined, not where it was called.

---

### 12. Arrays vs. objects
<a id="arrays-vs-objects"></a>

Arrays
- Used to store ordered collections of items.

- Items are accessed using numeric indexes (starting from 0).

- Best for lists, queues, stacks, or sequences.

- Comes with many built-in methods like push(), pop(), map(), filter(), etc.

Example:

```javascript
let colors = ["red", "green", "blue"];
console.log(colors[1]); // green
```

Objects

- Used to store key-value pairs.

- Keys are strings (or symbols), not numbers.

- Best for representing entities with properties (like a user, product, or settings).

- Comes with methods like Object.keys(), Object.values(), and Object.entries().

- Example:

```javascript
let car = { brand: "Toyota", color: "white" };
console.log(car.brand); // Toyota
```

---

### 13. What is Template literals?
<a id="template-literals"></a>

- Template literals are a way to create strings in JavaScript.

- They are written using backticks ` instead of single ' ' or double quotes " ".

- They allow:

Multiline strings easily (no need for \n).

Embedding variables directly into the string using ${}.

More readable and flexible string building.

- Normal String:
```javascript
let name = "John";
let greeting = "Hello, " + name + "!";
console.log(greeting); // Hello, John!
```

- Template literal:
```javascript
let name = "John";
let greeting = `Hello, ${name}!`;
console.log(greeting); // Hello, John!
```

- Multiline with template literals:
```javascript
let text = `This is line one
This is line two
This is line three`;
console.log(text);
```
- Template literals make it easier and cleaner to work with strings, especially when you need to mix variables or write multiple lines.

---

### 14. What is Destructuring?
<a id="destructuring"></a>

- Destructuring is a convenient way to extract values from arrays or properties from objects and assign them to variables in a more readable and concise way.
- Array destructuring lets you pull values from arrays based on position.
- Object destructuring lets you pull properties from objects based on property names.
- It makes your code more concise and easier to read.

---

### 15. Default parameters in functions
<a id="default-parameters-in-functions"></a>
Default parameters allow you to set default values for function parameters if the caller does not provide them.

- If the caller does not pass an argument for a parameter, the default value is used.

- This helps to avoid undefined values and makes the function more robust.

```javascript
function greet(name = "Guest") {
  console.log(`Hello, ${name}!`);
}

greet();          // Hello, Guest!
greet("Alice");   // Hello, Alice!
```
In this example, if <b>greet()</b> is called without an argument, <b>name</b> will default to <b>"Guest"</b>.

---

## ⚙️ Functions & Scope

### 16. What is a higher-order function?
<a id="what-is-a-higher-order-function"></a>

A higher-order function in JavaScript is a function that either:

- Takes one or more functions as arguments, or

- Returns a function as a result.

In other words, a higher-order function can either accept a function as an input or output a function.
Higher-order functions are common in JavaScript, especially in functions like <b>map</b>, <b>filter</b>, and <b>reduce</b>, which take a function as an argument to operate on arrays.

---

### 17. What is a closure?
<a id="what-is-a-closure"></a>

- A closure in JavaScript refers to a function that retains access to variables from its lexical scope (the scope in which it was defined), even after that scope has finished executing.

- In simpler terms, a closure allows a function to "remember" the environment in which it was created, even if it is called outside that environment.

Example of Closure
```javascript
function outerFunction(outerVariable) {
  return function innerFunction(innerVariable) {
    console.log("Outer variable: " + outerVariable); // Can access outerVariable
    console.log("Inner variable: " + innerVariable);
  };
}

const closureExample = outerFunction('I am outside!');
closureExample('I am inside!');
// Output:
// Outer variable: I am outside!
// Inner variable: I am inside!
```

In this example:

<b>outerFunction</b> defines a variable <b>outerVariable</b> and returns <b>innerFunction</b>.

Even though <b>outerFunction</b> finishes executing when <b>closureExample</b> is called, the <b>innerFunction</b> still has access to <b>outerVariable</b> because of the closure.

Why Closures are Useful:

- Data encapsulation: Closures allow you to create private variables, which cannot be accessed directly from outside the closure but can still be manipulated through the returned function.

- Maintaining state: Closures are often used in situations like event handlers, callbacks, or managing states in asynchronous operations.

Key Points of Closures:
1. Function inside a function: Closures typically occur when a function is defined inside another function.

2. Access to outer function variables: The inner function has access to variables from its outer function, even after the outer function has executed and returned.

---

### 18. What is currying?
<a id="what-is-currying"></a>

Currying is a technique in JavaScript (and other programming languages) where a function that takes multiple arguments is transformed into a sequence of functions, each taking one argument. Instead of calling the function with all its arguments at once, you call it with one argument, and it returns a new function that takes the next argument, and so on, until all arguments are provided.

- How Currying Works:
A curried function breaks down a function that takes multiple arguments into a series of unary (one-argument) functions.

- Example of Currying:
Let's look at a simple example of a curried function:
```javascript

function add(a) {
  return function(b) {
    return a + b;
  };
}

const addFive = add(5); // Returns a function that adds 5 to its argument
console.log(addFive(3)); // Output: 8
console.log(addFive(10)); // Output: 15
```
Currying with Multiple Arguments:
You can also curry a function with multiple arguments. Here's a more general approach using currying:

```javascript
function multiply(a) {
  return function(b) {
    return function(c) {
      return a * b * c;
    };
  };
}

const result = multiply(2)(3)(4); // Output: 24
console.log(result);
```
Here, the multiply function is curried so that:

- multiply(2) returns a function that takes b.

- That returned function then returns another function that takes c.

- Finally, the result of a * b * c is computed when all arguments are provided.

Why Use Currying?
- Reusability: You can create more specialized functions by fixing some of the arguments.

- Partial application: Currying allows you to provide arguments incrementally, which can be useful when you want to apply certain arguments in advance and provide the rest later.

- Cleaner code: Currying makes code more modular and can be used for better code composition in functional programming styles.

---

### 19. What is a callback function?
<a id="what-is-a-callback-function"></a>

A callback function is simply a function that you pass as an argument to another function, and then the other function calls (executes) it later.

It’s called a “callback” because the main function calls it back at the right time.

```javascript
function greet(name) {
  console.log('Hello, ' + name + '!');
}

function processUserInput(callback) {
  const name = 'Alice';
  callback(name);  // calling the function passed as argument
}

processUserInput(greet);
```
- Here, 'greet' is a callback.

- 'processUserInput' takes a function (callback) and calls it.

- In short:

A callback is a function passed into another function so that it can be called later.

---

### 20. What is callback hell and how to avoid it?
<a id="what-is-callback-hell-and-how-to-avoid-it"></a>

Callback hell happens when you have many nested callbacks — callbacks inside callbacks inside callbacks — and your code becomes very messy, hard to read, and hard to maintain.

It looks something like this:

```javascript
doTask1(function(result1) {
  doTask2(result1, function(result2) {
    doTask3(result2, function(result3) {
      doTask4(result3, function(result4) {
        console.log('All tasks done!');
      });
    });
  });
});
```
It's hard to understand what's happening because it's so deeply nested (often called the "Pyramid of Doom").

How to avoid callback hell?
Here are 3 common ways:

1. Modularize:

- Break your callbacks into separate named functions instead of writing everything inline.

Example:
```javascript
function task1Done(result1) { doTask2(result1, task2Done); }
function task2Done(result2) { doTask3(result2, task3Done); }
function task3Done(result3) { doTask4(result3, task4Done); }
function task4Done(result4) { console.log('All tasks done!'); }

doTask1(task1Done);
```

2. Use Promises:

- Promises let you chain asynchronous operations in a cleaner way.

Example:
```javascript
doTask1()
  .then(result1 => doTask2(result1))
  .then(result2 => doTask3(result2))
  .then(result3 => doTask4(result3))
  .then(result4 => console.log('All tasks done!'))
  .catch(error => console.error(error));
```

3. Use async/await:

- This is the cleanest and most modern way (built on top of promises).
```javascript
async function doAllTasks() {
  try {
    const result1 = await doTask1();
    const result2 = await doTask2(result1);
    const result3 = await doTask3(result2);
    const result4 = await doTask4(result3);
    console.log('All tasks done!');
  } catch (error) {
    console.error(error);
  }
}

doAllTasks();
```

---

### 21. Differences between call(), apply(), and bind()
<a id="call-apply-and-bind-differences"></a>

1. call() → calls now, arguments one by one.
```javascript
function greet(greeting, name) {
  console.log(greeting + ', ' + name);
}

greet.call(null, 'Hello', 'Alice'); 
// Output: Hello, Alice
```
- 'this' is 'null' here (not important for this example).

- Arguments passed individually.

2. apply() → calls now, arguments in an array.
```javascript
greet.apply(null, ['Hello', 'Alice']); 
// Output: Hello, Alice
```
- Same as 'call()', but arguments passed as an array.

3. bind() → creates a new function, call later.
```javascript
const greetHello = greet.bind(null, 'Hello');
greetHello('Alice');
// Output: Hello, Alice
```
'bind()' returns a new function that can be called later.

It locks the 'this' value and the first argument (greeting = 'Hello').

---

### 21. Arrow functions vs. bind() for this
<a id="arrow-functions-vs-bind-for-this"></a>

Features: 
- 'this' behavior : Arrow Function Inherits 'this' from the surrounding (parent) scope on the other hand 'bind()' manually sets 'this' to a specific value
- When 'this' is determined: Arrow Function-> At function definition time.  bind() -> At function creation/bind time
- Syntax: Arrow Function -> Short and Clean. bind() -> Slightly longer (needs .bind(this))
- Common Use: Arrow Function -> Best for callbacks, event handlers, methods in classes. bind()-> Useful when you want to reuse or delay a function with a fixed 'this'

Example to make it clear:

- Without arrow functions or bind:
```javascript
function Person() {
  this.name = 'Alice';

  setTimeout(function() {
    console.log(this.name); // undefined 😵 (because 'this' points to global/window)
  }, 1000);
}

new Person();
```

- Using 'bind(this)':
```javascript
function Person() {
  this.name = 'Alice';

  setTimeout(function() {
    console.log(this.name); // Alice 😎
  }.bind(this), 1000);
}

new Person();
```

- Using arrow function (easier!):
```javascript
function Person() {
  this.name = 'Alice';

  setTimeout(() => {
    console.log(this.name); // Alice 😎
  }, 1000);
}

new Person();
```
Arrow function automatically picks up this from Person, no need for .bind().

If you're writing modern JavaScript (especially ES6+), prefer arrow functions for simplicity unless you specifically need '.bind()' for flexibility (like when you want to reuse a function with different 'this' values).

---



