````markdown
# JavaScript Methods

## 1. String()

- Converts a value to a string.
- Example:
  ```javascript
  let num = 123;
  let str = String(num);
  console.log(str); // "123"
  console.log(typeof str); // "string"
  ```
````

## 2. Boolean()

- Converts a value to a boolean.
- Example:
  ```javascript
  let value = 1;
  let bool = Boolean(value);
  console.log(bool); // true
  <!--  -->
  console.log(typeof bool); // "boolean"
  console.log(Boolean(0)); // false
  console.log(Boolean(NaN)); // false
  console.log(Boolean("")); // false
  console.log(Boolean(null)); // false
  console.log(Boolean(undefined)); // false
  ```

## 3. Number()

- Converts a value to a number.
- Example:
  ```javascript
  let str = "123";
  let num = Number(str);
  console.log(num); // 123
  console.log(typeof num); // "number"
  ```

## 4. parseInt()

- Parses a string and returns an integer.
- Example:
  ```javascript
  let str = "123.45";
  let int = parseInt(str);
  console.log(int); // 123
  console.log(typeof int); // "number"
  ```

## 5. parseFloat()

- Parses a string and returns a floating point number.
- Example:
  ```javascript
  let str = "123.45";
  let float = parseFloat(str);
  console.log(float); // 123.45
  console.log(typeof float); // "number"
  ```

## 6. toString()

- Converts a number to a string.
- Example:
  ```javascript
  let num = 123;
  let str = num.toString();
  console.log(str); // "123"
  console.log(typeof str); // "string"
  ```

## 7. toFixed()

- Formats a number using fixed-point notation.
- Example:
  ```javascript
  let num = 123.456;
  let fixed = num.toFixed(2);
  console.log(fixed); // "123.46"
  console.log(typeof fixed); // "string"
  ```

```

```
