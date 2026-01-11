# JavaScript – Interview Ready Notes

> Comprehensive JavaScript notes for interviews and day-to-day development  
> Level: Beginner → Intermediate → Advanced

---

## 📚 Index (Table of Contents)

1. [What is JavaScript](#what-is-javascript)
2. [Features of JavaScript](#features-of-javascript)
3. [Key ES6 Features](#key-features-of-es6)
4. [var vs let vs const](#difference-between-var-let--const)
5. [Template Literals](#template-literals-es6)
6. [Data Types in JavaScript](#data-types-in-javascript)
7. [Primitive vs Non-Primitive Data Types](#primitive-vs-non-primitive-data-types)
8. [Hoisting](#hoisting)
9. [Temporal Dead Zone (TDZ)](#temporal-dead-zone-tdz)
10. [Scope in JavaScript](#scope-in-javascript)
11. [Lexical Scope & Scope Chain](#lexical-scope--scope-chain)
12. [Closures](#closures)
13. [this Keyword](#this-keyword)
14. [Shallow Copy vs Deep Copy](#shallow-copy-vs-deep-copy)
15. [Functions in JavaScript](#functions-in-javascript)
16. [Arrow Functions](#arrow-functions)
17. [IIFE (Immediately Invoked Function Expression)](#iife-immediately-invoked-function-expression)
18. [Objects in JavaScript](#objects-in-javascript)
19. [Array Methods: map, filter, reduce, forEach](#array-methods-map-filter-reduce-foreach)
20. [Synchronous vs Asynchronous JavaScript](#synchronous-vs-asynchronous-javascript)
21. [Execution Context & Call Stack](#execution-context--call-stack)
22. [Event Loop, Callback Queue & Microtask Queue](#event-loop-callback-queue--microtask-queue)
23. [Promises](#promises)
24. [Async / Await](#async--await)
25. [call(), apply(), bind()](#call-apply-bind)
26. [Prototype & Prototype Chain](#prototype--prototype-chain)
27. [Event Bubbling, Capturing & Delegation](#event-bubbling-capturing--delegation)
28. [Debouncing & Throttling](#debouncing--throttling)

---

## What is JavaScript

**Definition:**  
JavaScript is a high-level, interpreted, lightweight, and dynamic programming language mainly used to make web pages interactive.

- Runs inside browsers using JS engines (V8, SpiderMonkey)
- Core web technology along with HTML & CSS
- Can run outside browsers (Node.js)

---

## Features of JavaScript

| Feature                   | Explanation                           |
| ------------------------- | ------------------------------------- |
| Lightweight & Interpreted | Executes directly in browser          |
| Dynamic Typing            | Type decided at runtime               |
| Prototype-based OOP       | Uses prototypes                       |
| First-class Functions     | Functions treated as values           |
| Event-driven              | Responds to user events               |
| Asynchronous              | Uses callbacks, promises, async/await |
| Cross-platform            | Works on all browsers & OS            |
| DOM Manipulation          | Modify HTML & CSS dynamically         |

---

## Key Features of ES6

| Feature           | Description            | Example          |
| ----------------- | ---------------------- | ---------------- |
| let / const       | Block scoped variables | `let x = 10`     |
| Arrow Functions   | Shorter syntax         | `(a,b)=>a+b`     |
| Template Literals | String interpolation   | `Hello ${name}`  |
| Destructuring     | Extract values         | `const {a}=obj`  |
| Spread / Rest     | Expand & collect       | `...arr`         |
| Classes           | OOP syntax             | `class Person{}` |
| Modules           | import/export          | `import x from`  |
| Promises          | Async handling         | `new Promise()`  |

---

## Difference between var, let & const

| Feature       | var       | let   | const |
| ------------- | --------- | ----- | ----- |
| Scope         | Function  | Block | Block |
| Reassignment  | ✅        | ✅    | ❌    |
| Redeclaration | ✅        | ❌    | ❌    |
| Hoisting      | undefined | TDZ   | TDZ   |
| Global object | Yes       | No    | No    |

---

## Template Literals (ES6)

- String interpolation
- Multi-line strings
- Tagged templates

```js
const name = "Sam";
console.log(`Hello ${name}`);
```
