[Learn more about JS Template string](https://www.w3schools.com/js/js_string_templates.asp)

---

### What Are Template Literals?

Template literals are a way to create strings in JavaScript using backticks (`` ` ``) instead of quotes (`'` or `"`). They allow:

1. **String Interpolation** (embedding variables or expressions directly into strings).
2. **Multi-Line Strings**.
3. **Improved Readability** for dynamic strings.

---

### Syntax

```javascript
`String text`;
```

---

### 1. **String Interpolation**

**Explanation:** Embed variables or expressions directly into strings using `${}`.

**Example:**  
Imagine you want to greet a user by name.

```javascript
let name = "Alice";
let age = 25;

let greeting = `Hello, my name is ${name} and I am ${age} years old.`;
console.log(greeting);
// Output: Hello, my name is Alice and I am 25 years old.
```

---

### 2. **Multi-Line Strings**

**Explanation:** Create multi-line strings easily without using `\n`.

**Example:**  
Write a multi-line address.

```javascript
let address = `123 Main Street
Apartment 4B
New York, NY 10001`;

console.log(address);
/* Output:
123 Main Street
Apartment 4B
New York, NY 10001
*/
```

---

### 3. **Expression Evaluation**

**Explanation:** Evaluate JavaScript expressions directly inside `${}`.

**Example:**  
Calculate the total price of items in a shopping cart.

```javascript
let price = 50;
let quantity = 3;

let total = `The total price is $${price * quantity}.`;
console.log(total);
// Output: The total price is $150.
```

---

### 4. **Nesting Template Literals**

**Explanation:** You can embed one template literal inside another.

**Example:**  
Include a quote inside a dynamic message.

```javascript
let userName = "Bob";
let quote = `Success is not final, failure is not fatal: It is the courage to continue that counts.`;

let message = `${userName} says: "${quote}"`;
console.log(message);
// Output: Bob says: "Success is not final, failure is not fatal: It is the courage to continue that counts."
```

---

### 5. **Tagged Templates** (Advanced)

> **Note:** This section covers advanced concepts that are intended for future learning.

**Explanation:** Use a function to process template literals for custom formatting.

**Example:**  
Format currency values.

```javascript
function currency(strings, amount) {
  let value = parseFloat(amount).toFixed(2);
  return `${strings[0]}$${value}`;
}

let price = 99.99;
console.log(currency`The price is ${price}`);
// Output: The price is $99.99
```

---

### Real-Life Scenarios

1. **Dynamic Messages:**  
   Create dynamic error messages or logs.

```javascript
let errorCode = 404;
let message = `Error ${errorCode}: Page not found.`;
console.log(message);
// Output: Error 404: Page not found.
```

2. **HTML Templates:**

> **Note:** This section covers advanced concepts that are intended for future learning.

Build dynamic HTML content.

```javascript
let title = "Welcome to My Website";
let content = "This is a dynamic paragraph created using template literals.";

let html = `
  <h1>${title}</h1>
  <p>${content}</p>
`;

console.log(html);
/* Output:
  <h1>Welcome to My Website</h1>
  <p>This is a dynamic paragraph created using template literals.</p>
*/
```

3. **Personalized Notifications:**  
   Send custom alerts or notifications.

```javascript
let userName = "Jane";
let points = 120;

let notification = `Hi ${userName}, you have earned ${points} points!`;
console.log(notification);
// Output: Hi Jane, you have earned 120 points!
```

---

### Exercises for Students

1. **Basic Exercise:**

   - Create a greeting message that includes a person's name and age.
   - Calculate and display the total cost of buying multiple items.

2. **Multi-Line Task:**

   - Write a poem or song lyrics using multi-line template literals.

3. **Real-Life Scenarios:**

   > **Note:** This section covers advanced concepts that are intended for future learning.

   - Generate an HTML snippet for a product with a name, price, and description.
   - Create a dynamic message showing a countdown from 5 seconds.

---

### Why Use Template Literals?

1. Cleaner syntax for dynamic strings.
2. No need for string concatenation (`+`).
3. Great for multi-line strings and HTML generation.
