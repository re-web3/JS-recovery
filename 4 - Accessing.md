[Accessing string characters in JavaScript](<https://dev.to/charlesamakoye/three-ways-of-accessing-string-characters-in-javascript-3gbn#:~:text=using%20charAt()%20method,the%20character%20to%20be%20returned.>)

---

### Accessing Characters in Strings

Strings in JavaScript are **zero-indexed**, meaning the first character has an index of `0`, the second character has an index of `1`, and so on. You can access characters using two main methods:

---

### 1. **Bracket Notation (`str[index]`)**

**Explanation:** Use square brackets with the index to access a specific character in a string.

**Example:**  
Access the first and last character of a string.

```javascript
let str = "Hello";

console.log(str[0]); // Output: H (first character)
console.log(str[4]); // Output: o (last character)
```

---

### 2. **Using the `.charAt(index)` Method**

**Explanation:** Similar to bracket notation, `.charAt()` retrieves the character at a specified index.

**Example:**

```javascript
let str = "World";

console.log(str.charAt(0)); // Output: W (first character)
console.log(str.charAt(4)); // Output: d (last character)
```

**Key Difference:** If the index is out of range:

- `str[index]` returns `undefined`.
- `str.charAt(index)` returns an empty string (`""`).

---

### Accessing the Last Character Dynamically

You can use the `length` property to calculate the index of the last character.

```javascript
let str = "JavaScript";
let lastChar = str[str.length - 1];

console.log(lastChar); // Output: t
```

---

### Iterating Over Characters

Use a loop to access each character in a string.

**Example:**  
Print all characters of the string.

```javascript
let str = "Loop";

for (let i = 0; i < str.length; i++) {
  console.log(str[i]);
}
/* Output:
L
o
o
p
*/
```

---

### Real-Life Examples

1. **Checking the First Letter:**
   - Is the first letter of a username capitalized?

```javascript
let username = "Alice";

if (username[0] === username[0].toUpperCase()) {
  console.log("The first letter is capitalized.");
} else {
  console.log("The first letter is not capitalized.");
}
```

2. **Finding a Specific Character:**
   - Does the word contain a specific letter?

```javascript
let word = "banana";
let target = "n";

if (word.includes(target)) {
  console.log(`${target} is found in ${word}.`);
}
```

---

### Exercises for Students

1. **Basic Tasks:**

   - Access the first and last characters of the string `"Learning"`.
   - Create a function to return the character at a given position in a string.

2. **Intermediate Challenges:**

   - Write a function to reverse a string by iterating over its characters.
   - Count how many times a specific character appears in a string.

3. **Real-Life Task:**
   - Check if a password starts with a specific character (e.g., `"@"`).
