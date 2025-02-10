[Learn more about JS Popup Boxes](https://www.w3schools.com/js/js_popup.asp)

---

When teaching **`alert()`, `confirm()`, and `prompt()`** in JavaScript, focus on their purpose for interacting with users. These are simple yet powerful tools for displaying messages, getting user input, and making decisions.

---

### 1. **`alert()`**

**Purpose:** Display a simple message to the user.

- It shows a pop-up box with an "OK" button.
- Typically used for notifications or warnings.

**Syntax:**

```javascript
alert(message);
```

**Example:**  
Display a welcome message.

```javascript
alert("Welcome to our website!");
```

**Scenario:** Notify the user of an action.

```javascript
let username = "Alice";
alert(`Hello, ${username}! You have successfully logged in.`);
```

---

### 2. **`confirm()`**

**Purpose:** Ask the user for confirmation.

- It displays a message with "OK" and "Cancel" buttons.
- Returns `true` if the user clicks "OK" and `false` if "Cancel".

**Syntax:**

```javascript
confirm(message);
```

**Example:**  
Confirm before deleting an item.

```javascript
let isConfirmed = confirm("Are you sure you want to delete this item?");
if (isConfirmed) {
  alert("Item deleted.");
} else {
  alert("Action canceled.");
}
```

**Scenario:** Exit a page.

```javascript
let exit = confirm("Do you really want to leave this page?");
if (exit) {
  alert("Goodbye!");
} else {
  alert("Thanks for staying with us!");
}
```

---

### 3. **`prompt()`**

**Purpose:** Get input from the user.

- Displays a message, a text input field, and "OK"/"Cancel" buttons.
- Returns the input as a string or `null` if the user clicks "Cancel".

**Syntax:**

```javascript
prompt(message, defaultValue);
```

**Example:**  
Ask for the user's name.

```javascript
let name = prompt("What is your name?");
if (name) {
  alert(`Hello, ${name}!`);
} else {
  alert("You didn't provide a name.");
}
```

**Scenario:** Get a number and double it.

```javascript
let number = prompt("Enter a number to double:");
if (number !== null && !isNaN(number)) {
  alert(`The double of ${number} is ${number * 2}.`);
} else {
  alert("Invalid input. Please enter a number.");
}
```

---

### Combining `alert()`, `confirm()`, and `prompt()`

**Scenario:** Simulate a simple login flow.

```javascript
let username = prompt("Enter your username:");
if (username) {
  let isConfirmed = confirm(`Is your username "${username}"?`);
  if (isConfirmed) {
    alert("Welcome back, " + username + "!");
  } else {
    alert("Please re-enter your username.");
  }
} else {
  alert("No username entered.");
}
```

---

### Key Points for Each

1. **`alert()`**
   - One-way communication (only shows a message).
   - Best for notifications and warnings.
2. **`confirm()`**
   - Two options: OK and Cancel.
   - Best for asking simple Yes/No questions.
3. **`prompt()`**
   - Two-way communication (asks for user input).
   - Returns a string or `null`.

---

### Exercises for Students

1. **Basic Tasks:**

   - Use `alert()` to greet a user with their name.
   - Use `confirm()` to ask the user if they want to continue.

2. **Intermediate Challenges:**

   - Write a program that asks for a number using `prompt()` and calculates the square of the number.
   - Create a script that asks the user for their age and alerts if they are eligible to vote (`>= 18`).

3. **Advanced Scenarios:**
   - Simulate a "Delete Account" flow using `confirm()` and `alert()`.
   - Write a calculator program that uses `prompt()` to get two numbers and an operator, performs the calculation, and displays the result.

---
