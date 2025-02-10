[Learn more about JS Assignment Operators](https://www.w3schools.com/js/js_assignment.asp)

---

### What Are Assignment Operators?

Assignment operators are used to assign values to variables. They often combine with arithmetic operators for concise code.

---

### 1. **Basic Assignment (`=`)**

**Explanation:** Assigns a value to a variable.

**Example:**  
You set your starting score to 10 in a game.

```javascript
let score = 10; // Assign 10 to score
console.log(`Score: ${score}`); // Output: Score: 10
```

---

### 2. **Addition Assignment (`+=`)**

**Explanation:** Adds a value to a variable and updates it.

**Example:**  
A player earns 5 bonus points in a game.

```javascript
let score = 10;
score += 5; // Add 5 to score
console.log(`Updated score: ${score}`); // Output: Updated score: 15
```

---

### 3. **Subtraction Assignment (`-=`)**

**Explanation:** Subtracts a value from a variable and updates it.

**Example:**  
A player loses 3 points for a penalty.

```javascript
let score = 10;
score -= 3; // Subtract 3 from score
console.log(`Updated score: ${score}`); // Output: Updated score: 7
```

---

### 4. **Multiplication Assignment (`*=`)**

**Explanation:** Multiplies a variable by a value and updates it.

**Example:**  
You double your savings in a piggy bank.

```javascript
let savings = 50;
savings *= 2; // Multiply savings by 2
console.log(`Updated savings: ${savings}`); // Output: Updated savings: 100
```

---

### 5. **Division Assignment (`/=`)**

**Explanation:** Divides a variable by a value and updates it.

**Example:**  
You split your total bill equally among 4 friends.

```javascript
let totalBill = 100;
totalBill /= 4; // Divide totalBill by 4
console.log(`Each friend's share: ${totalBill}`); // Output: Each friend's share: 25
```

---

### 6. **Modulus Assignment (`%=`)**

**Explanation:** Calculates the remainder and updates the variable.

**Example:**  
You check how many candies are left after dividing them among 3 kids.

```javascript
let candies = 10;
candies %= 3; // Find the remainder when divided by 3
console.log(`Leftover candies: ${candies}`); // Output: Leftover candies: 1
```

---

### 7. **Exponentiation Assignment (`**=`)\*\*

**Explanation:** Raises a variable to the power of a value and updates it.

**Example:**  
You calculate the area of a square where the side length doubles each time.

```javascript
let sideLength = 2;
sideLength **= 3; // Raise sideLength to the power of 3
console.log(`Volume: ${sideLength}`); // Output: Volume: 8
```

---

### 8. **Bitwise Assignment Operators**

> **Note:** This section covers advanced concepts that are intended for future learning.

- `&=`: Bitwise AND assignment
- `|=`: Bitwise OR assignment
- `^=`: Bitwise XOR assignment
- `<<=`: Left shift assignment
- `>>=`: Right shift assignment

---

### Practice Exercise for Students

1. **Basic Tasks:**

   - Start with a variable `wallet = 100`.
   - Add 50 to it using `+=`.
   - Subtract 20 using `-=`.
   - Double the value using `*=`.
   - Divide it by 4 using `/=`.

2. **Story Problem:**  
   You start a business with $100. Each day:
   - You earn $50 (add using `+=`).
   - You spend 10% on expenses (calculate and subtract using `-=`).  
     Write a program to calculate your wallet balance after 3 days.
