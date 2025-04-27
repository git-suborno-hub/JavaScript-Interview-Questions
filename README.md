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
-- Falsy Values:
These are the values that are considered false when coerced into a Boolean. There are only 6 falsy values in JavaScript:

-false (the Boolean false)

-0 (zero)

-"" (empty string)

-null

-undefined

-NaN (Not-a-Number)

--Truthy Values:
All values except the falsy ones are considered truthy. This means that any value that is not falsy will be treated as true in a Boolean context.

-For example:

Non-empty strings (e.g., "Hello")

Non-zero numbers (e.g., 1, -1, 3.14)

Objects (including arrays, functions, etc.)

true (the Boolean true)

Infinity (positive and negative infinity)

Dates (e.g., new Date())

