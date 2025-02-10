# Data Types in JavaScript

In JavaScript, data types define the kind of values that variables can hold. JavaScript has two main categories of data types:

1. **Primitive Data Types**
2. **Reference Data Types**

---

## 1. Primitive Data Types

Primitive types are immutable, meaning their values cannot be altered. They are also stored directly in memory.

### Types of Primitive Data:

### 1.1 **Number**

- Represents both integer and floating-point numbers.
- Example:
  ```javascript
  let age = 25; // Integer
  let price = 19.99; // Floating-point number
  let infinityValue = Infinity; // Special numeric value
  let notANumber = NaN; // Result of invalid number operations
  ```

### 1.2 **String**

- Used for textual data. Strings are enclosed in quotes (single, double, or backticks).
- Example:
  ```javascript
  let name = "John";
  let greeting = "Hello";
  let template = `Welcome, ${name}!`;
  ```

### 1.3 **Boolean**

- Represents two values: `true` or `false`.
- Example:
  ```javascript
  let isAdmin = true;
  let isLoggedIn = false;
  ```

### 1.4 **Undefined**

- A variable that has been declared but has not been assigned a value.
- Example:
  ```javascript
  let user;
  console.log(user); // undefined
  ```

### 1.5 **Null**

- Represents an intentional absence of any object value. `null` is not the same as `undefined`.
- Example:
  ```javascript
  let selectedOption = null;
  ```

### 1.6 **Symbol** (ES6)

- Represents unique and immutable values. Often used as object property keys to avoid naming conflicts.
- Example:
  ```javascript
  let id = Symbol("id");
  let anotherId = Symbol("id");
  console.log(id === anotherId); // false
  ```

### 1.7 **BigInt** (ES2020)

- Used to represent integers beyond the safe limit for `Number`.
- Example:
  ```javascript
  let bigNumber = 1234567890123456789012345678901234567890n;
  let anotherBigNumber = BigInt("12345678901234567890");
  ```

### 1.8 **Safe Integers and BigInt**

- JavaScript can safely represent integers between `-(2^53 - 1)` and `2^53 - 1`, which is `-9007199254740991` to `9007199254740991`.
- Example of safe integers:
  ```javascript
  let safeNumber = 9007199254740991; // Safe integer
  console.log(safeNumber); // 9007199254740991
  ```

---

## 2. Reference Data Types

Reference types are objects that are mutable. Variables do not store the value directly but hold a reference to the memory location where the object is stored.

### Types of Reference Data:

### 2.1 **Object**

- Used to store collections of data or more complex entities.
- Example:
  ```javascript
  let user = {
    name: "John",
    age: 30,
  };
  ```

### 2.2 **Array**

- A special type of object used to store ordered collections.
- Example:
  ```javascript
  let fruits = ["apple", "banana", "cherry"];
  ```

### 2.3 **Function**

- A block of reusable code that performs a specific task. Functions are also objects.
- Example:
  ```javascript
  function greet() {
    console.log("Hello!");
  }
  ```

### 2.4 **Date**

- A built-in object for working with dates and times.
- Example:
  ```javascript
  let today = new Date();
  ```

---

## Type Checking

To check the type of a variable, use the `typeof` operator.

### Example:

```javascript
let number = 42;
let text = "Hello";
let isTrue = true;
let nothing = null;
let notDefined;
let uniqueId = Symbol("id");

console.log(typeof number); // "number"
console.log(typeof text); // "string"
console.log(typeof isTrue); // "boolean"
console.log(typeof nothing); // "object" (quirk of JavaScript)
console.log(typeof notDefined); // "undefined"
console.log(typeof uniqueId); // "symbol"
```

### Special Notes:

- The `typeof null` returns `object`. This is a known issue in JavaScript.
- Arrays and functions are technically objects but have special behavior.

---

## Mutable vs Immutable

| Type      | Mutable | Example                    |
| --------- | ------- | -------------------------- |
| Primitive | No      | Strings, numbers, etc.     |
| Reference | Yes     | Arrays, objects, functions |

---

## Dynamic Typing

JavaScript allows you to reassign variables to values of different types.

### Example:

```javascript
let value = 42; // Initially a number
value = "Hello"; // Now a string
value = true; // Now a boolean
```

This dynamic nature makes JavaScript flexible but can also lead to unexpected behavior if not handled carefully.

---

## Summary

- **Primitive Types**: Number, String, Boolean, Undefined, Null, Symbol, BigInt.
- **Reference Types**: Object, Array, Function, Date.
- Use `typeof` to check variable types.
- JavaScript is dynamically typed, allowing flexible and rapid development.
