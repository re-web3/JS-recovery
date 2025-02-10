[Learn more about JS Logical Operators](https://www.w3schools.com/js/js_comparisons.asp)

---

### What Are Logical Operators?

Logical operators are used to combine multiple conditions or invert a condition's result. They are commonly used in `if` statements or loops to make decisions.

---

### 1. **AND (`&&`)**

**Explanation:** Returns `true` if **both conditions** are `true`.

**Example:**  
"You can go to the amusement park if it's sunny **and** you have money."

```javascript
let isSunny = true;
let hasMoney = true;

if (isSunny && hasMoney) {
  console.log("You can go to the amusement park!"); // Output: You can go to the amusement park!
} else {
  console.log("You can't go to the amusement park.");
}
```

---

### 2. **OR (`||`)**

**Explanation:** Returns `true` if **at least one condition** is `true`.

**Example:**  
"You can stay indoors if it's raining **or** it's too cold."

```javascript
let isRaining = true;
let isTooCold = false;

if (isRaining || isTooCold) {
  console.log("Stay indoors."); // Output: Stay indoors.
} else {
  console.log("Go outside!");
}
```

---

### 3. **NOT (`!`)**

**Explanation:** Inverts the result of a condition. If a condition is `true`, it becomes `false`, and vice versa.

**Example:**  
"You're not allowed to enter if you're **not** an adult."

```javascript
let isAdult = false;

if (!isAdult) {
  console.log("You're not allowed to enter."); // Output: You're not allowed to enter.
} else {
  console.log("Welcome!");
}
```

---

### Combining Logical Operators

**Example:**  
"You can go on a vacation if you have money **and** either you have time **or** it's a holiday."

```javascript
let hasMoney = true;
let hasTime = false;
let isHoliday = true;

if (hasMoney && (hasTime || isHoliday)) {
  console.log("You can go on a vacation!"); // Output: You can go on a vacation!
} else {
  console.log("No vacation for you.");
}
```

---

### Truthy and Falsy with Logical Operators

Logical operators can also work with "truthy" and "falsy" values:

- **Falsy values**: `false`, `0`, `""` (empty string), `null`, `undefined`, and `NaN`.
- **Truthy values**: Everything else.

**Example:**  
Short-circuiting with `||` to provide a default value.

```javascript
let userName = ""; // Empty string is falsy
let defaultName = "Guest";

let nameToDisplay = userName || defaultName;
console.log(nameToDisplay); // Output: Guest
```

---

### Real-Life Scenarios

1. **Movie Ticket Example:**  
   "You can watch the movie if you're 18 or older **and** you have a ticket."

```javascript
let age = 18;
let hasTicket = true;

if (age >= 18 && hasTicket) {
  console.log("You can watch the movie."); // Output: You can watch the movie.
} else {
  console.log("You can't watch the movie.");
}
```

2. **Alarm System Example:**  
   "The alarm will trigger if there's motion **or** the door is open."

```javascript
let isMotionDetected = false;
let isDoorOpen = true;

if (isMotionDetected || isDoorOpen) {
  console.log("Alarm triggered!"); // Output: Alarm triggered!
} else {
  console.log("All is secure.");
}
```

---

### Exercises for Students

1. **Basic Practice:**

   - Write a program that checks if a user can log in only if their username **and** password are correct.
   - Write a program that outputs a default value if a variable is `null` or `undefined`.

2. **Real-World Scenario:**
   - A game allows a player to proceed if they have a key or if the door is unlocked. Use `||` to implement this logic.
   - A person can board a flight only if they have both a passport **and** a valid ticket. Use `&&` to implement this.

---
