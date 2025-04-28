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

### 23. What is an IIFE?
<a id="what-is-an-iife"></a>

An IIFE in JavaScript stands for Immediately Invoked Function Expression.

It’s a function that runs immediately after it's defined.

Here’s the basic syntax:

```javascript
(function() {
  console.log("I run immediately!");
})();
```
```javascript
(() => {
  console.log("I also run immediately, and I'm an arrow function!");
})();
```
- The function is wrapped in parentheses to turn it into an expression.

- Then it’s immediately invoked by the second pair of parentheses () right after it.

- It’s often used to create a private scope — variables inside the IIFE don’t leak outside.

---

### 24. Difference between scope and lexical scope
<a id="scope-vs-lexical-scope"></a>

<b>Scope</b>
- Scope means: "Where can I access a variable?"

- It's about visibility — where a variable exists and where it doesn’t.

```javascript
function myFunction() {
  const a = 10; // 'a' exists only inside this function
  console.log(a); // ✅
}
console.log(a); // ❌ Error: 'a' is not defined
```
- Here, a has function scope — it’s only accessible inside myFunction.

<b>Lexical Scope</b>
- Lexical scope means: "Where a variable is available depends on where it was written in the code."

- It’s determined at the time you write your code, not at runtime.

- Inner functions can access variables of their parent functions because of lexical scoping.

```javascript
function outer() {
  const b = 20;

  function inner() {
    console.log(b); //  inner can access b
  }

  inner();
}

outer();
```
- 'inner()' can access b because of lexical scope: it was written inside outer(), so it remembers the environment where it was created.

---

## 🧩 Control Flow & Iteration

### 25. Explain for, for...in, for...of loop
<a id="for-forin-vs-forof"></a>

🔵 for loop (classic loop)
- Used to loop a fixed number of times (usually over numbers or arrays by index).

```javascript
const fruits = ['apple', 'banana', 'cherry'];

for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}
// Output: apple, banana, cherry
```
Great when you need the <b>index(i)</b>

🔵 for...in loop
- Used to loop over object properties (keys).

- Works on objects or arrays (but mainly used for objects).

```javascript
const person = { name: 'Alice', age: 25 };

for (let key in person) {
  console.log(key, person[key]);
}
// Output:
// name Alice
// age 25
```
- Loops keys of an object.
-  If you use for...in on an array, it loops indexes (not values), which is not usually recommended.

🔵 for...of loop

- Used to loop over values directly in iterables (like arrays, strings, maps, sets).

```javascript
const fruits = ['apple', 'banana', 'cherry'];

for (let fruit of fruits) {
  console.log(fruit);
}
// Output: apple, banana, cherry
```

```javascript
for (let char of 'hello') {
  console.log(char);
}
// Output: h, e, l, l, o
```
- Loops values directly, much cleaner for arrays or strings!

<b>When to use for, for...in, and for...of?</b>

1. for loop

Use when:

- You need to loop over arrays or sequences where you know the number of iterations or want to access both index and value.

- Classic for loop: when you need more control over loop counters and iteration conditions.

2. for...in loop

Use when:

- You need to loop over object properties (keys), not values.

- Best for objects or cases where you want to get all the keys of an object, including inherited ones.

- Warning: Avoid using for...in on arrays because it loops over indexes as strings, and can also loop through additional properties added to the array.

3. for...of loop

Use when:

- You need to loop over values in arrays, strings, or iterables (like Sets, Maps).

- It’s cleaner than for...in for arrays because it doesn’t care about indexes, just the values.

---

### 26. Differences map(), forEach(), filter()
<a id="map-foreach-filter-differences"></a>

1. map()
- Purpose: Creates a new array by transforming each element of the original array based on a function you provide.

- Returns: A new array with the transformed values.

- Use case: When you need to modify every item in the array and get a new array of the same length.
```javascript
const numbers = [1, 2, 3];
const doubled = numbers.map(num => num * 2);

console.log(doubled); // Output: [2, 4, 6]
```

2. forEach()
- Purpose: Executes a function on each element of the array but does not return anything (i.e., returns undefined).

- Returns: undefined (side effects only).

- Use case: When you want to perform actions on each item in an array (e.g., logging, updating external variables, etc.) but don’t need a new array.

```javascript
const numbers = [1, 2, 3];
numbers.forEach(num => console.log(num * 2));

// Output: 
// 2
// 4
// 6
```

3. filter()
- Purpose: Creates a new array that only includes elements that satisfy a condition (the function returns true or false).

-Returns: A new array with elements that meet the condition (may be a smaller array or empty).

- Use case: When you need to select elements from an array that meet a specific condition.

```javascript

const numbers = [1, 2, 3, 4];
const evenNumbers = numbers.filter(num => num % 2 === 0);

console.log(evenNumbers); // Output: [2, 4]

```

---

### 27. Use cases of map(), filter(), reduce()
<a id="use-cases-of-map-filter-reduce"></a>

1. map()

<b>Use Case: Transforming Data</b>

- When to use it:
Use map() when you want to transform each item in an array and return a new array with the modified values.

- Examples:

Doubling Numbers: Transform an array of numbers by doubling each number.

```javascript
const numbers = [1, 2, 3, 4];
const doubled = numbers.map(num => num * 2);
console.log(doubled); // Output: [2, 4, 6, 8]
```
Extracting Data: When working with an array of objects, map() is often used to extract certain properties.

```javascript
const users = [
  { name: 'Alice', age: 25 },
  { name: 'Bob', age: 30 }
];
const names = users.map(user => user.name);
console.log(names); // Output: ['Alice', 'Bob']
```

2. filter()

<b>Use Case: Filtering Data</b>

- When to use it:
Use filter() when you want to select certain elements in an array based on a condition. It returns a new array containing only the elements that pass the condition.

- Examples:

Filtering Even Numbers: Select only the even numbers from an array.

```
const numbers = [1, 2, 3, 4, 5, 6];
const evenNumbers = numbers.filter(num => num % 2 === 0);
console.log(evenNumbers); // Output: [2, 4, 6]
```
Filtering Active Users: Filter out inactive users from a list.
```javascript

const users = [
  { name: 'Alice', isActive: true },
  { name: 'Bob', isActive: false }
];
const activeUsers = users.filter(user => user.isActive);
console.log(activeUsers); // Output: [{ name: 'Alice', isActive: true }]
```
3. reduce()

<b>Use Case: Accumulating or Combining Data</b>

- When to use it:
Use reduce() when you want to accumulate or combine all the elements of an array into a single value (like sum, product, or concatenation).

- Examples:

Summing Numbers: Calculate the sum of all numbers in an array.

```javascript
const numbers = [1, 2, 3, 4];
const sum = numbers.reduce((accumulator, currentValue) => accumulator + currentValue, 0);
console.log(sum); // Output: 10
```

Counting Occurrences: Count how many times each item appears in an array.
```javascript
const fruits = ['apple', 'banana', 'orange', 'apple', 'banana'];
const fruitCount = fruits.reduce((acc, fruit) => {
  acc[fruit] = (acc[fruit] || 0) + 1;
  return acc;
}, {});
console.log(fruitCount); // Output: { apple: 2, banana: 2, orange: 1 }

```
Flattening an Array of Arrays: Flatten a nested array into a single array.

```javascript

const nestedArray = [[1, 2], [3, 4], [5, 6]];
const flatArray = nestedArray.reduce((acc, current) => acc.concat(current), []);
console.log(flatArray); // Output: [1, 2, 3, 4, 5, 6]
```

In Conclusion:
- map(): Use when you need to transform the array.

- filter(): Use when you need to select elements based on a condition.

- reduce(): Use when you need to combine or accumulate values into one result.

---


## 🌐 DOM & Events

### 28. What is the DOM and how to manipulate it?
<a id="what-is-the-dom-and-how-to-manipulate-it"></a>


- The DOM (Document Object Model) is a programming interface for web documents. It represents the structure of an HTML or XML document as a tree of objects, where each object corresponds to a part of the document (e.g., an element, attribute, or piece of text). The DOM allows programs to interact with the content, structure, and style of web pages dynamically.

- DOM Tree: The DOM organizes HTML elements in a hierarchical tree structure. Each element, attribute, and piece of text in the document becomes a node in the DOM tree.


<b>Manipulating the DOM with JavaScript</b>
You can use JavaScript to manipulate the DOM and change the content, structure, and style of a webpage dynamically. This allows you to create interactive websites. Here's how to do it:

1. Accessing DOM Elements
You need to first select the DOM element(s) you want to manipulate. There are several methods to select elements:

1.1. getElementById()
Selects an element by its ID.

```javascript
const element = document.getElementById('myElement');
```

1.2. getElementsByClassName()
Selects elements by their class name. This returns a live HTMLCollection.

```javascript
const elements = document.getElementsByClassName('myClass');
```

1.3. getElementsByTagName()
Selects elements by their tag name.

```javascript
const paragraphs = document.getElementsByTagName('p');
```

1.4. querySelector()
Selects the first matching element based on a CSS selector.

```javascript
const firstParagraph = document.querySelector('p');
```

1.5. querySelectorAll()
Selects all matching elements based on a CSS selector.

```javascript
const allParagraphs = document.querySelectorAll('p');
```

<b>2. Manipulating DOM Elements</b><br>
Once you've selected an element, you can manipulate it in various ways. Here are some common methods:

2.1. Changing Content
- innerText: Get or set the visible text content inside an element.

```javascript
document.getElementById('myElement').innerText = 'New content!';
```
- innerHTML: Get or set the HTML content inside an element (allows you to include HTML tags).
```javascript
document.getElementById('myElement').innerHTML = '<strong>Bold content</strong>';
```

2.2. Changing Attributes
You can change attributes of an element like src, href, class, etc.

- setAttribute(): Set an attribute.

```javascript
document.getElementById('myImage').setAttribute('src', 'newImage.jpg');
```

- getAttribute(): Get an attribute.

```javascript
const srcValue = document.getElementById('myImage').getAttribute('src');
```

2.3. Adding and Removing Classes
- classList.add(): Add a class to an element.

```javascript
document.getElementById('myElement').classList.add('newClass');
```

-classList.remove(): Remove a class from an element.

```javascript
document.getElementById('myElement').classList.remove('oldClass');
```

- classList.toggle(): Add the class if it doesn't exist, or remove it if it does.

```javascript
document.getElementById('myElement').classList.toggle('active');
```

2.4. Changing Styles
- style: Directly manipulate the inline CSS styles of an element.

```javascript
document.getElementById('myElement').style.backgroundColor = 'blue';
```

<b>3. Adding/Removing Elements</b>
You can also create new elements, add them to the document, or remove existing ones.

3.1. Creating Elements
- createElement(): Creates a new element.

```javascript
const newDiv = document.createElement('div');
newDiv.innerText = 'Hello, world!';
```

3.2. Adding Elements to the DOM
- appendChild(): Adds a new child to an element.

```javascript
document.body.appendChild(newDiv);
```

3.3. Removing Elements
- removeChild(): Removes a child from an element.

```javascript
const parent = document.getElementById('parentElement');
const child = document.getElementById('childElement');
parent.removeChild(child);
```

<b>4. Handling Events</b>
You can listen to user actions (clicks, key presses, etc.) and respond to them with JavaScript.

4.1. Adding Event Listeners
- addEventListener(): Registers an event listener on an element.

```javascript
document.getElementById('myButton').addEventListener('click', function() {
  alert('Button clicked!');
});
```

4.2. Removing Event Listeners
- removeEventListener(): Removes an event listener.

```javascript
const button = document.getElementById('myButton');
const handleClick = function() {
  alert('Button clicked!');
};
button.addEventListener('click', handleClick);

// To remove the listener
button.removeEventListener('click', handleClick);
```

---

### 29. Difference between Event bubbling and Capturing
<a id="event-bubbling-vs-capturing"></a>

Event bubbling and capturing are two phases in the event propagation mechanism in JavaScript when an event is triggered on an element. Here's the difference between the two:

1. Event Bubbling (Default Behavior)
- Order: The event starts from the innermost element (the target element) and propagates outward to the root element (typically the document or window).

- How it works: When an event occurs, it triggers on the target element first and then "bubbles up" through its parent elements, all the way up to the root element.

- Use case: This is useful for event delegation, where a single event listener can be placed on a parent element to handle events for its child elements.

Example:

```javascript
document.getElementById("child").addEventListener("click", () => {
  alert("Child clicked");
});

document.getElementById("parent").addEventListener("click", () => {
  alert("Parent clicked");
});
```
In this case, if the child is clicked, the "Child clicked" alert will appear first, and then the "Parent clicked" alert will show up as the event bubbles up.


2. Event Capturing (also called "Trickling")
- Order: The event starts from the root element and propagates inward to the target element.

- How it works: The event is captured by the outermost elements first and then travels inward towards the target element.

- Use case: This is less commonly used, but it can be useful when you want to handle the event before any inner elements can process it.

Example:
```javascript
document.getElementById("parent").addEventListener("click", () => {
  alert("Parent clicked");
}, true); // "true" makes it capture the event during the capturing phase

document.getElementById("child").addEventListener("click", () => {
  alert("Child clicked");
});
```
In this case, if the child is clicked, the "Parent clicked" alert will appear first because the event is captured before it reaches the child.

---

### 30. What is Event delegation?
<a id="event-delegation"></a>

Event delegation is a technique in JavaScript where you attach a single event listener to a parent element instead of attaching individual listeners to each child element. This approach takes advantage of event propagation (bubbling) to handle events for dynamically added or multiple child elements efficiently.

How Event Delegation Works:
- Attach a single event listener: Instead of adding separate event listeners to every child element, you add an event listener to a common parent element.

- Event propagation: When an event is triggered on a child element, it bubbles up through its ancestors (parent elements) until it reaches the parent element with the event listener.

- Check the target: Inside the event handler, you can check the event.target property to determine which child element was clicked or interacted with.

Benefits of Event Delegation:

- Improves performance: Instead of adding event listeners to multiple child elements, you add only one to their common parent. This is especially useful for a large number of child elements.

- Handles dynamically added elements: If new child elements are added after the event listener is set up, the parent element still handles events for them, without needing to attach new listeners to each new element.

- Reduces memory usage: Fewer event listeners are needed, saving memory.

Example of Event Delegation:
- Let's say you have a list of items, and you want to detect clicks on individual list items:

```html
<ul id="itemList">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

<script>
  // Parent element
  const list = document.getElementById("itemList");

  // Event listener on the parent element
  list.addEventListener("click", function(event) {
    // Check if the clicked target is an <li> element
    if (event.target.tagName === "LI") {
      alert("You clicked on " + event.target.textContent);
    }
  });
</script>
```
In this example:

- The 'click' event listener is attached to the 'ul' element (the parent).

- When a list item ('li') is clicked, the event bubbles up to the 'ul' element, where the handler checks if the target element is a 'li' element using 'event.target'.

- Even if new items are added to the list later, the event listener on the parent ('ul') will still work for them.

Use Case:

Event delegation is especially useful when:

- You have a large number of elements (e.g., list items, table rows, etc.) and want to avoid adding event listeners to each one.

- Your elements are dynamically created, so you can't predict all of them ahead of time.

---

## 🔁 Async & Execution Model

### 31. Difference between Synchronous and Asynchronous code
<a id="synchronous-vs-asynchronous-code"></a>

<b>1. Synchronous Code:</b>

- Execution Order: In synchronous code, tasks are executed one after another, in a sequential manner. Each operation must complete before the next one starts.

- Blocking: Synchronous operations block the execution of subsequent code. If a task takes time (like reading a file or fetching data), it will block the entire program until it's done.

- Use case: Synchronous code is suitable for tasks that are quick and don't need to interact with external resources or don't involve heavy computations.

Example:
```javascript
console.log('Start');
console.log('Middle');
console.log('End');
```
Output:
```sql
Start
Middle
End
```
Each statement is executed in the order it's written, blocking the next one until the current task completes.

<b>2. Asynchronous Code:</b>

- Execution Order: In asynchronous code, tasks are executed independently of the main program flow. When an asynchronous task is called, it is handed off to the system (or an event loop) to be executed later, while the program continues with the next line of code.

- Non-blocking: Asynchronous operations do not block the execution of subsequent code. This allows for more efficient handling of tasks that take time (like I/O operations or network requests).

- Use case: Asynchronous code is used when tasks need to run in parallel, such as making HTTP requests, interacting with databases, or waiting for user input.

Example using 'setTimeout' (asynchronous function):

```javascript
console.log('Start');
setTimeout(() => {
  console.log('Middle');
}, 1000);
console.log('End');
```

Output:
```sql
Start
End
Middle
```
- "Start" is printed first, followed by "End", and then after 1 second, "Middle" is printed. This happens because 'setTimeout' is asynchronous and does not block the rest of the code.

<b>Synchronous</b> code runs sequentially and blocks the program until each task is completed.

<b>Asynchronous</b> code allows the program to continue running while certain tasks are being handled in the background, enabling more efficient execution for tasks like I/O or network calls.


---

### 32. What is the Event Loop?
<a id="what-is-the-event-loop"></a>

The <b>event loop</b> allows JavaScript to run asynchronously, ensuring non-blocking behavior. It manages the execution of synchronous code, handles asynchronous operations, and processes the callback queue, making JavaScript efficient in handling tasks like I/O, animations, and network requests without freezing the main thread.

---

### 33. Difference between Microtasks and Macrotasks.
<a id="microtasks-vs-macrotasks"></a>

<b>Microtasks:</b>
Microtasks are smaller tasks that have higher priority than macrotasks. They typically include tasks like resolved promises (.then(), catch(), and finally()), 'MutationObserver' callbacks, and 'async' functions. Microtasks are always executed <b>before</b> the event loop moves to the next macrotask, even if a macrotask is already waiting.

- Execution Timing: After the synchronous code is executed and before any macrotask is processed, the event loop will first clear all the microtasks that have been queued. This ensures that any microtasks get completed before the browser does any other task, including rendering or handling macrotasks.

- Examples:

A promise '.then()' callback.

An 'async' function's '.then()'.

<b>Macrotasks:</b>
Macrotasks are typically larger tasks that are placed in the <b>callback queue</b>. These include tasks such as 'setTimeout()', 'setInterval()', I/O operations, and events like user input or network responses. Macrotasks represent chunks of work that can be processed by the event loop after microtasks are completed.

- Execution Timing: The event loop processes macrotasks one by one in the order they appear in the queue. It waits until all microtasks have been processed before moving to the next macrotask. If there are multiple macrotasks, the event loop will handle them one after the other, only interrupting with microtasks if any are pending.

- Examples:

setTimeout()

setInterval()

I/O operations (e.g., file reading, network requests)

<b>Execution Order:</b>

The event loop prioritizes microtasks over macrotasks. This means that if there are microtasks pending after the synchronous code execution, they will be executed before the event loop processes the next macrotask. Only after all microtasks are completed will the event loop begin handling the next macrotask.

---

### 34. What is a Promise?
<a id="what-is-a-promise"></a>

A Promise in JavaScript is an object that allows you to handle asynchronous operations in a more manageable and structured way. It has three states: pending, fulfilled, and rejected, and provides methods (then(), catch(), finally()) to handle the results of the operation or errors. By using promises, you can avoid callback hell and write more readable and maintainable asynchronous code.

---

### 35. How async/await works?
<a id="how-asyncawait-works"></a>

<b>What is async/await?</b>
- 'async/await' is a modern way to handle asynchronous operations (like fetching data from a server) in JavaScript.

- It makes asynchronous code look and behave like synchronous (normal step-by-step) code — making it much easier to read and manage.

<b>How does it work?</b>

1. async keyword:

- You put async before a function to make it return a promise automatically.

- Even if you return a simple value, it wraps it in a promise.

Example: 
```javascript
async function sayHello() {
  return "Hello";
}

sayHello().then(alert);  // Alerts "Hello"
```

2. await keyword:

- You use await inside an async function.

- await pauses the function until the promise is settled (either fulfilled or rejected).

- After the promise is settled, it resumes the function and gives you the result.

Example: 
```javascript
async function getData() {
  let response = await fetch('https://api.example.com/data');
  let data = await response.json();
  console.log(data);
}
```
Here:

- It waits for fetch() to complete.

- Then it waits for response.json() to complete.

- Then it prints the data.

In short:
- async = Marks a function that will work with promises.

- await = Waits for a promise to resolve inside that async function.

---

### 36. How setTimeout() and setInterval() work?
<a id="how-settimeout-and-setinterval-work"></a>

<b>1. How setTimeout() works</b>

- setTimeout() runs a function once after a delay.
- It waits for the given time once, then executes the function.

example:
```javascript
setTimeout(() => {
  console.log("Hello after 2 seconds");
}, 2000);
```

- After 2 seconds, it prints: Hello after 2 seconds.
- It runs only once after the timer.


<b>2. How setInterval() works</b>
- setInterval() runs a function repeatedly, again and again at regular intervals.
- It keeps running the function every given time until you stop it.

```javascript
setInterval(() => {
  console.log("Hello every 2 seconds");
}, 2000);
```
- Every 2 seconds, it prints: Hello every 2 seconds, forever until you stop it.

<b>Stopping setTimeout() or setInterval()</b>

- setTimeout can be canceled by clearTimeout(timerID).

- setInterval can be canceled by clearInterval(timerID).

Example with canceling interval:

```javascript
const intervalId = setInterval(() => {
  console.log("Repeating...");
}, 1000);

// Stop after 5 seconds
setTimeout(() => {
  clearInterval(intervalId);
  console.log("Stopped the interval!");
}, 5000);
```

Prints "Repeating..." every second.

After 5 seconds, it stops.


<b>How they work behind the scenes</b>
- JavaScript has an event loop and callback queue.

- setTimeout and setInterval don't pause JavaScript.

- They schedule the callback to run later.

- JavaScript continues running the rest of the code meanwhile.

- When the time is up, the callback function is put into the queue and executed when JavaScript is free.

---

### 37. Purpose of Promise.all(), Promise.any(), and Promise.race()
<a id="purpose-of-promiseall-promiseany-and-promiserace"></a>

👉 Promise.all()

Purpose:

- Wait for all promises to succeed (or fail if any one fails).

- If all promises are successful, you get an array of their results.

- If any promise fails, it immediately rejects.

Example:
```javascript
Promise.all([
  Promise.resolve(1),
  Promise.resolve(2),
  Promise.resolve(3)
])
.then(results => console.log(results))
.catch(error => console.error(error));
```
Output:
```csharp
[1, 2, 3]
```

👉 Promise.any()

Purpose:

- Wait for any one promise to succeed.

- It ignores failures unless all promises fail.

- If at least one succeeds, you get its result.

```javascript
Promise.any([
  Promise.reject("Error 1"),
  Promise.resolve(2),
  Promise.resolve(3)
])
.then(result => console.log(result))
.catch(error => console.error(error));
```
Output:
```
2
```
✅ First successful promise gives the result.

👉 Promise.race()

Purpose:

- Return the first settled promise (whether fulfilled or rejected).

- Whichever promise settles first, that becomes the result.

Example:
```javascript
Promise.race([
  new Promise(resolve => setTimeout(resolve, 1000, "One")),
  new Promise(resolve => setTimeout(resolve, 500, "Two"))
])
.then(result => console.log(result))
.catch(error => console.error(error));
```

Output:
```ngnix
Two
```
✅ Two wins because it finished faster (after 500ms).

---

## 🧠 Concepts & Patterns

### 38. What is immutability?
<a id="what-is-immutability"></a>

- In JavaScript, immutability means not changing the original value — instead, you create and work with new copies when you want to make changes.

In simple words:

- Immutable data cannot be changed once created.

Why is immutability important?

- Makes code predictable and easier to debug.

- Helps in undo/redo functionality (like in apps).

- Crucial in React.js and modern frontend frameworks.

Common ways to achieve immutability in JS:

- Use 'const' for variables.

- Use methods like 'map(), filter(), slice()' that return new arrays.

- Avoid methods like 'push(), splice(), sort()' that mutate the original array.

---

### 39. What is a pure function?
<a id="what-is-a-pure-function"></a>

A pure function in JavaScript (or in any programming language) is a function that:

- Always gives the same output for the same input.

- Does not change anything outside itself (no side effects).

Example of a pure function:

```javascript
function add(a, b) {
  return a + b;
}

console.log(add(2, 3)); // 5
console.log(add(2, 3)); // 5 (always the same result)
```
Why Pure Functions are Important:
- Easier to test and debug.

- Make code predictable and safe.

- Important for functional programming and libraries like React.

---

### 40. What is optional chaining (?.)?
<a id="what-is-optional-chaining-"></a>

<b>Optional chaining (?.)</b> is a feature in JavaScript that lets you safely access deeply nested properties without worrying if something in the chain is null or undefined.

In simple words:

It checks each step — if something is missing (null or undefined), it stops and returns undefined instead of throwing an error.

Example without optional chaining:

```javascript
const user = {
  name: "Alice",
  address: {
    city: "Wonderland"
  }
};

console.log(user.address.city); // "Wonderland"
console.log(user.profile.bio);  // ❌ Error! Cannot read property 'bio' of undefined
```
Same example using optional chaining:

```javascript
console.log(user.address?.city);   // "Wonderland"
console.log(user.profile?.bio);    // undefined (no error, safely handled)
```
- user.profile is undefined, so user.profile?.bio becomes undefined automatically.

- No crash! ✅

Where you can use ?.
- Access properties: obj?.prop

- Call functions: obj.method?.()

- Access array elements: arr?.[index]

---

### 41. What is nullish coalescing (??)?
<a id="what-is-nullish-coalescing-"></a>

- Nullish coalescing (??) is a feature in JavaScript that provides a default value when the left side is null or undefined.
- If the value is null or undefined, ?? gives you something else (a backup/default value).

Example:

```javascript
const username = null;
const displayName = username ?? "Guest";

console.log(displayName); // "Guest"
```
- Since username is null, it falls back to "Guest".

<b>How it's different from || (OR operator):</b>

'||' treats falsy values like 0, "" (empty string), false as well,
but ?? only cares about null or undefined.

---

### 42. Difference between Shallow copy and Deep copy 
<a id="shallow-copy-vs-deep-copy"></a>

📚 Shallow Copy

- Copies only the top-level of the object/array.

- If the object contains other objects (nested), the inner objects are still shared (not copied).

Example of Shallow Copy:

```javascript
Copy code
const person = {
  name: "Alice",
  address: {
    city: "Wonderland"
  }
};

const shallowCopy = { ...person };

shallowCopy.name = "Bob";           // ✅ Only changes shallowCopy
shallowCopy.address.city = "Paris"; // ❗ Changes both shallowCopy AND person!

console.log(person.address.city); // "Paris" (affected!)
```

- 'name' change is safe (copied value).

- But 'address.city' change affects the original too!
- because only the reference to 'address' was copied, not the inner object itself.

📚 Deep Copy

- Copies everything, including nested objects.

- The original and the copy are completely independent.

Example of Deep Copy:

```javascript
Copy code
const person = {
  name: "Alice",
  address: {
    city: "Wonderland"
  }
};

// Deep Copy (one simple way using JSON)
const deepCopy = JSON.parse(JSON.stringify(person));

deepCopy.name = "Bob";           // ✅ Changes deepCopy only
deepCopy.address.city = "Paris"; // ✅ Changes deepCopy only

console.log(person.address.city); // "Wonderland" (original untouched!)
```

- Now, changes inside address don't affect person.

- Full separation ✅

🔵 In one sentence:

Shallow copy = surface copy only;
Deep copy = full independent copy.

---

### 43. JavaScript modules: import/export
<a id="javascript-modules-importexport"></a>

🧩 What are JavaScript Modules?
In JavaScript, modules mean splitting your code into separate files (each handling a specific task) and sharing code between them.

This keeps your code:

- Organized

- Reusable

- Easier to maintain

<b>1. export — Sending something out</b>

You use export when you want to make something available outside the current file.

There are two types of export:

- Named Export — export multiple things by name

- Default Export — export one main thing

<b>2. import — Bringing something in</b>
You use 'import' when you want to use exported stuff from another file.

<b>Importing Named Exports</b>
```javascript
import { add, subtract } from './math.js';

console.log(add(2, 3));      // 5
console.log(subtract(5, 2)); // 3
```
- Use {} to import named exports.

- Names must match exactly.

<b>Importing Default Export</b>

```javascript
import greet from './greet.js';

console.log(greet("Alice")); // "Hello, Alice!"
```
- No {} needed.

- You can give any name to the default import.

<b>Important points:</b>
- File extension should be .js or .mjs (for modules).
- In HTML, when linking the JS file, use:
```html
<script type="module" src="app.js"></script>
```
- Relative paths (./ or ../) are important when importing.

---

### 44. Error handling with try/catch/finally
<a id="error-handling-with-trycatchfinally"></a>

🧠 Why handle errors?
When something unexpected happens (like a wrong input, missing data, etc.), you don't want your app to crash 🚨.
You want to catch the error and handle it gracefully (like showing a nice message).

That’s where try/catch/finally comes in.

🔥 Basic Syntax
```javascript
try {
  // code that might throw an error
} catch (error) {
  // code to handle the error
} finally {
  // (optional) code that runs no matter what
}
```

📦 Example:
```javascript
try {
  let result = 10 / 0;
  console.log("Result:", result);

  throw new Error("Something went wrong!"); // Manually throwing an error
} catch (error) {
  console.log("Caught an error:", error.message);
} finally {
  console.log("This block always runs.");
}
```
🧩 Output:

```vbnet

Result: Infinity
Caught an error: Something went wrong!
This block always runs.
```
✨ What each part does:

try -> Try to run the risky code
catch -> If an error happens, catch it and handle it
finally -> Always runs, whether there was an error or not (cleanup etc.)

🧨 A Real-world Example:
Imagine you are trying to parse some JSON:

```javascript

const jsonString = '{"name": "Alice"}'; // Correct JSON

try {
  const user = JSON.parse(jsonString);
  console.log(user.name); // "Alice"
} catch (error) {
  console.log("Invalid JSON format!");
} finally {
  console.log("Parsing attempt finished.");
}
```

If the 'jsonString' was broken (like missing a quote), the 'catch' would grab the error without crashing your app.

🛠 Important points:

- catch(error) → the error object gives information about what went wrong.

- finally block always runs:

whether there is an error

or no error

- You can even throw your own custom errors using throw.

Example:

```javascript
throw new Error("Custom error message");
```
🔵 In one sentence:

try to do something risky ➔ catch the problem if it happens ➔ finally always clean up afterward.

---

### 45. What is the typeof operator?
<a id="what-is-the-typeof-operator"></a>

The typeof operator is used to check the data type of a value. It returns a string describing the type.

Basic Syntax:
```javascript
typeof value
```
```javascript
console.log(typeof "Hello"); // "string"
console.log(typeof 123);     // "number"
console.log(typeof true);    // "boolean"
console.log(typeof {});      // "object"
console.log(typeof []);      // "object"  ❗ (Arrays are technically objects)
console.log(typeof undefined); // "undefined"
console.log(typeof null);      // "object" ❗ (strange historical bug)
console.log(typeof function() {}); // "function"
```
🛠 Important things to remember:
- typeof null returns "object" — this is a bug in JavaScript from the very beginning!

- Arrays are also objects → use Array.isArray() if you want to specifically detect an array.

- typeof NaN (Not-a-Number) is "number", because NaN is still a number type internally.

---

## 💡 Advanced JavaScript


### 46. What is the prototype chain?
<a id="what-is-the-prototype-chain"></a>

🧠 What is the Prototype Chain in JavaScript?
The prototype chain is a system in JavaScript where objects inherit properties and methods from other objects.

✅ In simple words:
If you try to access a property on an object and it doesn’t exist there, JavaScript will look up the chain (on its prototype) to find it.

Basic Example:
```javascript

const person = {
  greet() {
    console.log("Hello!");
  }
};

const student = Object.create(person);

student.study = function() {
  console.log("Studying...");
};
student.greet();  // "Hello!" (inherited from person)
student.study();  // "Studying..." (own method)
```
✅ student didn't have a greet() method directly,
so JavaScript looked at student's prototype → found greet() on person.

How the Chain Works:
Imagine it like a ladder:

```plaintext

student → person → Object.prototype → null
```
- student looks for greet.

- If not found, it checks its prototype (person).

- If still not found, it checks Object.prototype.

- If nowhere found, it returns undefined.

✨ A Real-world Analogy:
Imagine you are looking for a book 📚:

- First, you check your own bookshelf (your own properties).

- If it's not there, you check your parent's bookshelf (prototype).

- If still not found, you check the town library (Object.prototype).

- If nowhere, then you give up (null).

Quick Summary:
- Every object has an internal link to another object called its prototype.

- This prototype chain is what enables inheritance in JavaScript.

- The search for properties/methods moves up the chain until found or it hits null.

---

### 47. Memory management & garbage collection
<a id="memory-management--garbage-collection"></a>

🧠 Memory Management in JavaScript
In simple words:
✅ Memory management = controlling how your program allocates and frees up memory.

Your code creates variables, objects, functions, etc., and they all consume memory.
At some point, when you're done with them, that memory needs to be reclaimed to avoid memory leaks (bad for performance).

Good news:

👉 In JavaScript, memory management is automatic.
👉 The JavaScript Engine (like V8 in Chrome, Node.js) handles it for you using Garbage Collection.

🗑️ What is Garbage Collection?
Garbage collection (GC) is the process where JavaScript automatically finds and removes values from memory that are no longer needed.

✅ When an object is no longer reachable, it is removed by the garbage collector.

📚 How JavaScript decides what to delete?

✅ JavaScript uses a simple concept called Reachability:

- A value is considered reachable if it can be accessed somehow.

- If a value becomes unreachable, it becomes "garbage" → ready to be cleaned up.

🔥 Example:

```javascript

let user = {
  name: "Alice"
};

user = null; // The object { name: "Alice" } becomes unreachable.
```

- Initially, { name: "Alice" } is reachable through user.

- When we set user = null, there's no reference to that object anymore.

- Now it's garbage collected automatically!

🧩 In short:

Reachable -> Still accessible → stays in memory.
Unreachable -> No references → removed from memory.
Garbage Collector -> The tool that finds unreachable data and deletes it.

🧠 Some Common Reachable Values

- Local variables and parameters in a function currently running

- Global variables

- Any value that is still referenced from those

Quick Summary:

JavaScript automatically manages memory by allocating it when objects are created and reclaiming it when they become unreachable through garbage collection.
You don’t have to manually free memory — but you do have to code carefully to avoid leaks!

---

### 48. Difference between Object.freeze() and Object.seal()
<a id="memory-management--garbage-collection"></a>

Both are methods used to restrict changes to an object, but they have different levels of strictness.

🔥 Object.freeze()
✅ Makes an object completely immutable.

- You cannot add new properties.

- You cannot remove existing properties.

- You cannot change (modify) existing property values.

- You cannot reconfigure property attributes (like making writable: false, etc.).

The object becomes totally locked.

Example:
```javascript
const user = {
  name: "Alice"
};

Object.freeze(user);

user.name = "Bob"; //  Can't modify
user.age = 30;     //  Can't add new property
delete user.name;  //  Can't delete

console.log(user); 
// { name: "Alice" }
```

🔥 Object.seal()
✅ Allows modifications to existing properties, but no adding or removing.

- You can change (modify) existing property values.

- You cannot add new properties.

- You cannot delete properties.

- You cannot reconfigure properties (make them writable: false, etc.).

The object is sealed — structure can't change, but contents can update.

Example: 
```javascript
const user = {
  name: "Alice"
};

Object.seal(user);

user.name = "Bob"; // Can modify existing
user.age = 30;     // Can't add new property
delete user.name;  // Can't delete property

console.log(user); 
// { name: "Bob" }
```

- Freeze = Frozen solid ❄️ (can't change anything!)

- Seal = Sealed container 📦 (can't add/remove, but you can edit inside)

Object.freeze() locks everything; Object.seal() locks the object's structure but allows changes to values.

---

### 49. Explain Object.keys(), values(), entries()
<a id="objectkeys-values-entries"></a>

1. Object.keys(obj)
✅ Returns an array of the object’s property names (keys).

Example:
```javascript
const user = {
  name: "Alice",
  age: 25,
  city: "Paris"
};
console.log(Object.keys(user));
// Output: ["name", "age", "city"]
```

2. Object.values(obj)
✅ Returns an array of the object’s property values.

Example:
```javascript

console.log(Object.values(user));
// Output: ["Alice", 25, "Paris"]
```

3. Object.entries(obj)

✅ Returns an array of [key, value] pairs.

Each pair is itself a small array: [key, value].

Example:
```javascript

console.log(Object.entries(user));
/*
Output:
[
  ["name", "Alice"],
  ["age", 25],
  ["city", "Paris"]
]
*/
```
✨ Use Cases:
- Object.keys() → loop through property names.

- Object.values() → loop through values.

- Object.entries() → loop through both keys and values easily.

---

### 50. What is a memory leak and how to avoid it?
<a id="what-is-a-memory-leak-and-how-to-avoid-it"></a>

✅ Memory leak = when your program keeps holding on to memory that it no longer needs.

Even though the data is useless, the JavaScript engine cannot free that memory because something (like a variable or reference) is still pointing to it.

Over time, memory usage grows → performance slows down  → maybe even crashes!

-  Example of a memory leak:

```javascript

let user = {
  name: "Alice"
};

let unused = user; // Another reference

user = null; // But 'unused' still holds the object!

// The { name: "Alice" } object is STILL in memory because 'unused' points to it.
```

<b>Common Causes of Memory Leaks:</b>

- Global variables -> Unnecessary variables on window/global
- Forgotten timers/listeners -> setInterval, event listeners not cleared
- Detached DOM elements	-> DOM elements removed visually but still referenced in JS
- Closures holding too much data -> Functions unintentionally keeping old data alive

<b>How to Avoid Memory Leaks?</b>

Best practices:

- Avoid unnecessary global variables.

- Clear timers and intervals when no longer needed.

- Remove event listeners when elements are deleted.

- Nullify references manually if needed (someVar = null).

- Be careful with closures (don't keep huge objects inside closures if not needed).

- Use modern tools like React, Vue, etc. carefully — they have built-in cleaning mechanisms (e.g., useEffect cleanup functions in React).

---

### 51. What are WeakMap and WeakSet?
<a id="what-are-weakmap-and-weakset"></a>

1. WeakMap
✅ A WeakMap is like a Map, but:

- Keys must be objects (not primitives like strings or numbers).

- Keys are held weakly (they don’t prevent garbage collection).

- No .size, no .keys(), no iteration — for safety.

Example:

```javascript
const weakMap = new WeakMap();

let user = { name: "Alice" };

weakMap.set(user, "User Data");

console.log(weakMap.get(user)); // "User Data"

user = null; // Now the { name: "Alice" } object can be garbage collected!

// weakMap will automatically remove the entry behind the scenes!
```

-user's object gets garbage collected automatically because WeakMap doesn't stop it.

2. WeakSet:

✅ A WeakSet is like a Set, but:

- Only stores objects, not primitive values.

- Objects are held weakly.

- No .size, no iteration methods — again for safety.

Example:

```javascript
const weakSet = new WeakSet();

let car = { brand: "Tesla" };

weakSet.add(car);

console.log(weakSet.has(car)); // true

car = null; // Now the { brand: "Tesla" } object can be garbage collected!
```
- After car = null, the object disappears from WeakSet automatically.

✨ Why use WeakMap/WeakSet?
- Private Data: Attach hidden info to objects (without preventing GC).

- Memory-efficient Caching: Cache based on objects without risking memory leaks.

- DOM Node Tracking: Manage DOM elements without holding them if they are removed.

<b>Important points:</b>

- You cannot loop (forEach, for..of) over WeakMaps/WeakSets.

- They are mostly used internally in libraries and frameworks — but knowing them is important for understanding efficient memory use!

---

### 52. Difference between Stack and Heap memory
<a id="stack-vs-heap-memory"></a>

<b>Stack:</b>
- Think of it like a pile of plates.

- When a function is called, its local variables are pushed onto the stack.

- When the function ends, it pops off and frees memory automatically.

- Fast, but limited in size.

✅ Example (stack memory):

```javascript
function add(a, b) {
  let result = a + b; // 'result' is stored in the stack
  return result;
}
```
Numbers (a, b, result) are primitives → go into stack.

<b>Heap:</b>
- Think of it like a big messy warehouse.

- Objects, arrays, and functions are stored in the heap.

- You access them via references (pointers).

- Slower, but can handle big data.

✅ Example (heap memory):

```javascript
let user = { name: "Alice", age: 25 };
```

- The object { name: "Alice", age: 25 } lives in the heap, and user holds a reference (address) to it in the stack.

<b>How Stack and Heap work together:</b>
- Primitive types → stored directly in the stack.

- Reference types → the reference (address) is stored in the stack, but the actual object/array is stored in the heap.

---

### 53. Difference between Debouncing and Throttling
<a id="debouncing-vs-throttling"></a>

<b>What is Debouncing?</b>

Debouncing means waiting until the user stops doing something for a certain amount of time, and then taking action.

- Suppose you are typing in a search bar.

- Every time you press a key, the website could search — but that would be very wasteful!

- Instead, debouncing says:
👉 "Wait until the user has stopped typing for 500ms, and then perform the search."

If the user keeps typing fast, the timer keeps resetting, and the action doesn’t happen yet.

Example:

```javascript
function debounce(func, delay) {
  let timer;
  return function() {
    clearTimeout(timer);
    timer = setTimeout(func, delay);
  };
}

const search = debounce(() => console.log('Searching...'), 500);
```
Every time you type, it resets the clock.

<b>What is Throttling?</b>
Throttling means limiting how often an action can happen, even if the user keeps triggering it.

- Imagine a user is scrolling the page really fast.

- Without throttling, the scroll event could fire hundreds of times per second, which is very heavy!

- Throttling says:
👉 "Only run the scroll function once every 100ms, no matter how many times scrolling happens."
Example:

```javascript
function throttle(func, limit) {
  let inThrottle;
  return function() {
    if (!inThrottle) {
      func();
      inThrottle = true;
      setTimeout(() => inThrottle = false, limit);
    }
  };
}

const handleScroll = throttle(() => console.log('Scrolling...'), 100);
```
Even if the user scrolls madly, the function runs only once every 100ms.

<b>Quick way to remember:<b>
- Debounce = “Wait until the action stops, then fire once.”

- Throttle = “Keep firing, but not too often.”

---

### 54. How the new keyword works?
<a id="how-the-new-keyword-works"></a>

When you use the 'new' keyword with a function, it creates a new object and sets it up based on that function.

It does 4 important things automatically behind the scenes:

<b>Step-by-Step</b>
- Create a new empty object {}.

- Set the prototype of that object to be the prototype of the constructor function.

→ (This connects the new object to methods defined on the constructor's .prototype.)

- Call the constructor function with this set to the new object.

→ (It allows the function to add properties/methods onto the new object.)

- Return the new object unless the constructor returns its own object.

<b>Simple Example:</b>

```javascript
function Person(name, age) {
  this.name = name;
  this.age = age;
}

const user = new Person('Alice', 25);

console.log(user); // { name: 'Alice', age: 25 }
```

So,The 'new' keyword automates the creation of a new object, sets up inheritance, runs the constructor function, and returns the new object. 

---

### 55. Common JS design patterns
<a id="common-js-design-patterns"></a>

<b>1. Module Pattern</b>
- Purpose: Organize related code together, hide internal details, and expose only what’s needed.

Used a lot to create private variables and methods.

```javascript

const Counter = (function() {
  let count = 0;

  return {
    increment() { count++; console.log(count); },
    decrement() { count--; console.log(count); }
  };
})();

Counter.increment(); // 1
Counter.increment(); // 2
Counter.decrement(); // 1
```
👉 count is private. Only increment and decrement can modify it.

<b>2. Singleton Pattern</b>
Purpose: Make sure only one instance of something exists.

Useful for managing global states (e.g., app settings, user session).

```javascript

const AppSettings = (function() {
  let instance;

  function createInstance() {
    return { theme: 'dark', version: '1.0' };
  }

  return {
    getInstance() {
      if (!instance) {
        instance = createInstance();
      }
      return instance;
    }
  };
})();

const settings1 = AppSettings.getInstance();
const settings2 = AppSettings.getInstance();

console.log(settings1 === settings2); // true
```
👉 Only one settings object is created.

<b>3. Factory Pattern</b>
Purpose: Create different types of objects using the same interface.

You don't have to manually use new everywhere — useful when object creation is complex.

```javascript

function Car(type) {
  if (type === 'electric') {
    return { type: 'Electric Car', battery: '100%' };
  } else {
    return { type: 'Gas Car', fuel: 'Full' };
  }
}

const car1 = Car('electric');
const car2 = Car('gas');

console.log(car1, car2);
```
👉 The factory decides what type of object to return.

<b>4. Observer Pattern</b>
Purpose: When one object changes, automatically notify others.

Used in event systems, real-time apps, chat apps, etc.

```javascript

class Subject {
  constructor() {
    this.observers = [];
  }

  subscribe(fn) {
    this.observers.push(fn);
  }

  unsubscribe(fn) {
    this.observers = this.observers.filter(observer => observer !== fn);
  }

  notify(data) {
    this.observers.forEach(observer => observer(data));
  }
}

const subject = new Subject();

function logger(data) {
  console.log('Logger:', data);
}

subject.subscribe(logger);
subject.notify('Hello Observers!'); // Logger: Hello Observers!
```
👉 Subject notifies all subscribed observers when something happens.

<b>5. Prototype Pattern</b>
Purpose: Share common methods across instances to save memory.

Used heavily in OOP (Object-Oriented Programming) in JavaScript.

```javascript

function Dog(name) {
  this.name = name;
}

Dog.prototype.bark = function() {
  console.log(this.name + ' says woof!');
};

const dog1 = new Dog('Buddy');
dog1.bark(); // Buddy says woof!
```
👉 bark is not copied to every dog — it's shared through prototype.

<b>Summary in One Line:</b>
- Module → Organize and hide details.

- Singleton → Only one instance allowed.

- Factory → Create objects easily.

- Observer → Subscribe and react to changes.

- Prototype → Share methods efficiently.

---

### 56. Difference between Deep equality ans Strict equality
<a id="deep-equality-vs-strict-equality"></a>

<b>What is Strict Equality (===)?</b>
- Strict equality checks if two values are exactly the same in both type and value.

- It does NOT look inside objects or arrays — it just checks if they refer to the same thing.

👉 Example:

```javascript

2 === 2;          // true
'hello' === 'hello'; // true
2 === '2';        // false (different types)
```
For objects or arrays:

```javascript

const obj1 = { a: 1 };
const obj2 = { a: 1 };

console.log(obj1 === obj2); // false
```
Even though obj1 and obj2 have the same content, they are different objects in memory — so === says false.

<b>What is Deep Equality?</b>
- Deep equality means comparing the actual content inside two values.

- It recursively checks all properties if they are equal in value.

👉 Example:

```javascript

const obj1 = { a: 1, b: { c: 2 } };
const obj2 = { a: 1, b: { c: 2 } };

console.log(deepEqual(obj1, obj2)); // true
```
(You would need a custom function like deepEqual or a library like lodash to perform deep equality.)

Simple deep equality function:

```javascript

function deepEqual(a, b) {
  if (a === b) return true;

  if (typeof a !== 'object' || typeof b !== 'object' || a == null || b == null) {
    return false;
  }

  let keysA = Object.keys(a);
  let keysB = Object.keys(b);

  if (keysA.length !== keysB.length) return false;

  for (let key of keysA) {
    if (!keysB.includes(key) || !deepEqual(a[key], b[key])) {
      return false;
    }
  }

  return true;
}
```
In short:
- Strict equality (===) → Direct comparison. Fast.
(Does not check inside objects/arrays.)

- Deep equality → Content comparison.
(Recursively checks properties inside.)

---

### 57. How the JS engine works internally?
<a id="how-the-js-engine-works-internally"></a>

When you run JavaScript code, the JavaScript engine (like V8 in Chrome, SpiderMonkey in Firefox) does several important jobs step by step:

<b>1. Parsing</b>
- The engine reads your code, checks for errors, and converts it into an intermediate structure called the Abstract Syntax Tree (AST).

- Think of the AST like a map of your code's meaning — it helps the engine understand what your program wants to do.

Example:
```javascript
const a = 5;
```

<b>2. Compilation (Just-In-Time Compilation - JIT)</b>
- JavaScript engines use Just-In-Time (JIT) Compilation.

- Instead of interpreting line-by-line or compiling everything before running, JIT does both:

Quickly interpret code and start running it immediately.

Meanwhile, optimize parts of the code that are used a lot (hot code).

- This makes JavaScript fast without needing you to manually compile it.

<b>3. Execution</b>
- After parsing and compiling, the engine executes the code.

- Execution happens inside something called the Call Stack.

The Call Stack:

- It keeps track of which function is currently running.

- When a function is called, it's pushed onto the stack.

- When a function finishes, it's popped off the stack.

Example:

```javascript
function greet() {
  console.log('Hello!');
}
greet();
```
- greet() is added to the call stack.

- console.log() is added.

- After logging, console.log() and greet() are removed.

<b>4. Memory Management</b>
- JS engines allocate memory when variables and objects are created.

- Later, they free up memory automatically when data is no longer used — this is Garbage Collection.

⚙️ What important components are inside a JS Engine?

- Memory Heap → Where memory allocation happens.

- Call Stack → Where function calls are tracked.

- Web APIs (in browsers) → Like setTimeout, fetch, etc., handled outside the engine.

- Callback Queue → Functions waiting to be executed (especially from asynchronous tasks).

- Event Loop → Continuously checks if the Call Stack is empty and moves tasks from Callback Queue into Call Stack.

---

### 58. Difference between Generators and Iterators
<a id="generators-vs-iterators"></a>

First: What are Iterators?

- An iterator is any object that has a .next() method.

- Every call to .next() returns an object like { value: something, done: true/false }.

- You can manually control the flow by calling .next().

👉 Example of a custom iterator:

```javascript

function createIterator(array) {
  let index = 0;

  return {
    next: function() {
      if (index < array.length) {
        return { value: array[index++], done: false };
      } else {
        return { done: true };
      }
    }
  };
}

const iterator = createIterator(['a', 'b', 'c']);

console.log(iterator.next()); // { value: 'a', done: false }
console.log(iterator.next()); // { value: 'b', done: false }
console.log(iterator.next()); // { value: 'c', done: false }
console.log(iterator.next()); // { done: true }
```

🔹 You manually define how it moves through data.

Second: What are Generators?

- A generator is a special type of function that automatically creates an iterator.

- You define it with a function* and use the yield keyword to "pause" and "resume" the function.

- Much easier and cleaner than writing manual iterators!

👉 Example of a generator:

```javascript

function* generatorFunction() {
  yield 'a';
  yield 'b';
  yield 'c';
}

const gen = generatorFunction();

console.log(gen.next()); // { value: 'a', done: false }
console.log(gen.next()); // { value: 'b', done: false }
console.log(gen.next()); // { value: 'c', done: false }
console.log(gen.next()); // { value: undefined, done: true }
```
🔹 Generator functions take care of creating an iterator and managing the done status for you.
