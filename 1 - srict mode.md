### Strict Mode in JavaScript

**Strict Mode** is a way to enforce stricter parsing and error handling in your JavaScript code. It helps developers write cleaner, more secure, and error-free code by throwing errors for common coding mistakes that JavaScript might otherwise allow silently.

---

### Enabling Strict Mode

You can enable strict mode in two ways:

1. **Globally for a script:** Add `"use strict";` at the beginning of the script.

   ```javascript
   "use strict";

   let x = 3.14; // Works fine
   undeclaredVariable = 10; // Throws an error: "undeclaredVariable is not defined"
   ```

2. **Locally for a function:** Add `"use strict";` inside a function.
   ```javascript
   function myFunction() {
     "use strict";
     let y = 3.14; // Works fine
     undeclaredVariable = 10; // Throws an error: "undeclaredVariable is not defined"
   }
   ```

---

### Why Use Strict Mode?

Strict mode prevents certain actions and throws more errors to help you:

1. **Catch Common Bugs:** Avoid mistakes like using undeclared variables.
2. **Prevent Accidental Globals:** Disallows assigning values to undeclared variables.
3. **Simplify Debugging:** Makes it easier to detect errors.
4. **Secure JavaScript:** Eliminates some silent behaviors that can lead to bugs or security vulnerabilities.

---

### Features of Strict Mode

#### 1. **Disallows Undeclared Variables**

```javascript
"use strict";
undeclaredVariable = 10; // Error: undeclaredVariable is not defined
```

#### 2. **Throws Errors for Assigning to Read-Only Properties**

```javascript
"use strict";
const obj = {};
Object.defineProperty(obj, "property", { value: 42, writable: false });

obj.property = 100; // Error: Cannot assign to read-only property
```

#### 3. **Prevents Deleting Non-Configurable Properties**

```javascript
"use strict";
delete Object.prototype; // Error: Cannot delete property 'prototype'
```

#### 4. **Disallows Duplicate Parameters in Functions**

```javascript
"use strict";
function add(a, a) {
  // Error: Duplicate parameter name not allowed in strict mode
  return a + a;
}
```

#### 5. **Restricts `this` Keyword**

- In strict mode, `this` is `undefined` in functions that are not called as methods.

```javascript
"use strict";
function showThis() {
  console.log(this);
}
showThis(); // Output: undefined
```

#### 6. **Reserved Words**

- Prevents the use of reserved words like `implements`, `interface`, `let`, etc.

```javascript
"use strict";
let let = 10; // Error: Unexpected strict mode reserved word
```

---

### Example Without and With Strict Mode

#### Without Strict Mode:

```javascript
x = 10; // No error, even though 'x' is undeclared
console.log(x); // Output: 10
```

#### With Strict Mode:

```javascript
"use strict";
x = 10; // Error: x is not defined
console.log(x);
```

---

### Scenarios to Use Strict Mode

1. **Best Practices:**
   - Always use strict mode for better coding discipline.
2. **Legacy Code:**
   - Add strict mode to specific functions when converting old code to modern JavaScript.
3. **Modules:**
   - ES6 modules automatically run in strict mode, so you don't need to declare it explicitly.

---

### Advantages of Strict Mode

- Catches coding errors earlier.
- Prevents unintended behaviors.
- Improves code readability and maintainability.
- Makes your code future-proof by aligning with modern JavaScript standards.

---

### Exercises for Students

1. **Basic Task:**
   - Write a script with and without `"use strict"` and observe the differences.
2. **Debugging Practice:**
   - Introduce an undeclared variable in strict mode and fix the error.
3. **Function Behavior:**
   - Create a function in strict mode and observe how `this` behaves.

Strict mode is an essential tool for writing better JavaScript. It encourages good practices and ensures your code is less prone to errors!
