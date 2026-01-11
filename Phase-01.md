# Phase 1: JavaScript Language Fundamentals (Deep Level)

> Level: Intermediate → Advanced  
> Purpose: Interview preparation + long-term reference  
> Focus: Specification behavior, edge cases, and mental models

---

## 📌 Table of Contents

1. [ECMAScript Specification & Evolution](#1-ecmascript-specification--evolution-es5--esnext)
2. [Lexical Structure](#2-lexical-structure)
3. [Statements vs Expressions](#3-statements-vs-expressions)
4. [Strict Mode](#4-strict-mode-use-strict)
5. [Data Types: Primitive vs Reference](#5-data-types-primitive-vs-reference)
6. [Type Coercion & Abstract Equality](#6-type-coercion--abstract-equality-algorithm)
7. [Truthy & Falsy Edge Cases](#7-truthy--falsy-edge-cases)
8. [typeof, instanceof, Object.prototype.toString](#8-typeof-instanceof-objectprototypetostring)
9. [Immutability vs Mutability](#9-immutability-vs-mutability)
10. [Phase 1 Interview Summary](#phase-1-summary-interview-perspective)

---

## 1. ECMAScript Specification & Evolution (ES5 → ESNext)

### What is ECMAScript?

- **ECMAScript (ES)** defines the _language specification_
- **JavaScript** = ECMAScript + host environment APIs (DOM, Web APIs, Node APIs)

> Engines must follow the spec, but implementations vary.

---

### Evolution Overview

- **ES5 (2009)**
  - Strict mode
  - `Object.defineProperty`
  - Array iteration methods
- **ES6 / ES2015**
  - `let`, `const`
  - Arrow functions
  - Classes (syntax sugar)
  - Modules
  - Promises
- **ESNext**
  - Yearly releases
  - TC39 proposal stages (0 → 4)

---

### Interview Notes

- ECMAScript ≠ JavaScript runtime
- ES modules are always in strict mode
- Spec defines _behavior_, not _performance_

---

## 2. Lexical Structure

### Tokens

- Keywords: `if`, `return`, `class`
- Identifiers: variables, functions
- Operators: `+`, `===`
- Punctuators: `{}`, `()`, `;`

---

### Literals

- String, Number, BigInt
- Boolean, Object, Array
- Template literals support expressions

---

### Identifiers

- Unicode supported
- Can start with `_` or `$`
- Case-sensitive

---

### Interview Notes

- Automatic Semicolon Insertion (ASI) exists
- Relying on ASI can cause subtle bugs

---

## 3. Statements vs Expressions

### Expressions

- Produce a value

```js
a + b;
condition ? x : y;
```
