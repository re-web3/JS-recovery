[Learn more about JS Comparison Operators](https://www.w3schools.com/js/js_comparisons.asp)

---

### What Are Comparison Operators?

Comparison operators compare two values and determine their relationship. They're used to make decisions in conditional statements like `if` or loops.

---

### 1. **Equal (`==`)**

**Explanation:** Checks if two values are equal, ignoring data type.

**Example:**  
"Is 5 the same as '5'?"

```javascript
console.log(5 == "5"); // Output: true
```

---

### 2. **Strict Equal (`===`)**

**Explanation:** Checks if two values are equal **and** of the same type.

**Example:**  
"Is 5 strictly the same as '5'?"

```javascript
console.log(5 === "5"); // Output: false
console.log(5 === 5); // Output: true
```

---

### 3. **Not Equal (`!=`)**

**Explanation:** Checks if two values are not equal, ignoring data type.

**Example:**  
"Is 5 not the same as '10'?"

```javascript
console.log(5 != "10"); // Output: true
```

---

### 4. **Strict Not Equal (`!==`)**

**Explanation:** Checks if two values are not equal **or** not of the same type.

**Example:**  
"Is 5 not strictly the same as '5'?"

```javascript
console.log(5 !== "5"); // Output: true
console.log(5 !== 5); // Output: false
```

---

### 5. **Greater Than (`>`)**

**Explanation:** Checks if the left value is greater than the right value.

**Example:**  
"Is 10 greater than 5?"

```javascript
console.log(10 > 5); // Output: true
```

---

### 6. **Less Than (`<`)**

**Explanation:** Checks if the left value is less than the right value.

**Example:**  
"Is 3 less than 8?"

```javascript
console.log(3 < 8); // Output: true
```

---

### 7. **Greater Than or Equal To (`>=`)**

**Explanation:** Checks if the left value is greater than or equal to the right value.

**Example:**  
"Is 7 greater than or equal to 7?"

```javascript
console.log(7 >= 7); // Output: true
```

---

### 8. **Less Than or Equal To (`<=`)**

**Explanation:** Checks if the left value is less than or equal to the right value.

**Example:**  
"Is 4 less than or equal to 6?"

```javascript
console.log(4 <= 6); // Output: true
```

---

### Real-Life Scenarios for Comparison Operators

1. **Game Score Example:**  
   "Did the player reach the target score of 100?"

```javascript
let score = 95;
let target = 100;
console.log(score >= target); // Output: false
```

2. **Age Verification Example:**  
   "Is the person old enough to vote?"

```javascript
let age = 18;
let votingAge = 18;
console.log(age >= votingAge); // Output: true
```

3. **Price Comparison Example:**  
   "Is the price of the item within your budget?"

```javascript
let itemPrice = 50;
let budget = 60;
console.log(itemPrice <= budget); // Output: true
```

---

### Exercise for Students

1. Write a program to check:

   - If two numbers are equal.
   - If one number is greater than the other.
   - If a string value is equal to a number value using both `==` and `===`.

2. Write a small app:
   - Input your current score and the target score.
   - Print whether you've reached or exceeded the target.

This will make the concepts engaging and relatable for your students!
