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



