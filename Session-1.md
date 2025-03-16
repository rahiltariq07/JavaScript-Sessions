# Session 1: JavaScript Basics

The session covers:

- An introduction to JavaScript
- Using `console.log`
- Basic syntax
- Variables
- Data types (Primitive and Reference)
- Operators

---

## 1. Introduction to JavaScript

- **What is JavaScript?**
  - A programming language used to make websites interactive.
  - Runs directly in your web browser (Chrome, Firefox, etc.).


---

## 2. Using `console.log`

- **Purpose:**  
  Prints messages or values to the browser’s console for debugging and testing your code.

- **Example:**  
  ```js
  console.log('Hello, world!');
  ```
  
---

## 3. Basic Syntax

- **Statements & Semicolons:**  
  - Every instruction is a statement.
  - End statements with a semicolon (`;`)

- **Code Blocks:**  
  - Use curly braces `{}` to group multiple statements (e.g., in loops or conditionals).

- **Comments:**  
  - **Single-line:** `// This is a comment`
  - **Multi-line:**  
    ```js
    /* This is a multi-line comment.
       It spans more than one line. */
    ```

---

## 4. Variables

- **Definition:**  
  Variables are containers for storing data values.

- **Declaring Variables:**  
  - Use `let` for variables whose values can change.
  - Use `const` for variables whose values remain constant.
  
- **Examples:**  
  ```js
  let age = 25;          // A variable that may change
  const name = 'Alice';  // A constant variable
  console.log(age, name);
  ```

- **Naming Rules:**
  - Can include letters, numbers, underscores (_), and dollar signs ($).
  - Cannot begin with a number.
  - Use descriptive names (e.g., `age`, `score`, `favoriteColor`).

---

## 5. Data Types

JavaScript data types are divided into **Primitive** and **Reference** types.

### 5.1 Primitive Data Types

- **Numbers:**  
  Stores numeric values (e.g., `let count = 100;`).

- **Strings:**  
  Stores text (e.g., `let greeting = 'Hello';`).

- **Booleans:**  
  Represents logical values: `true` or `false` (e.g., `let isSunny = true;`).

- **Undefined:**  
  A variable that is declared but not assigned a value.

- **Null:**  
  Represents "no value" or an empty value.


### 5.2 Reference Data Types

- **Objects:**  
  Collections of key-value pairs.  
  Example:
  ```js
  let person = { name: 'Bob', age: 30 };
  ```

- **Arrays:**  
  Ordered lists of values.  
  Example:
  ```js
  let colors = ['red', 'green', 'blue'];
  ```

- **Functions:**  
  A function is a block of code that performs a specific task. Think of it as a mini-program within your program. Instead of writing the same code over and over, you write a function once and call it whenever you need to perform that task

---

## 6. Operators

Operators allow you to perform calculations and make comparisons.

### 6.1 Arithmetic Operators
- **Addition (`+`):**  
  `console.log(5 + 3);` // 8

- **Subtraction (`-`):**  
  `console.log(10 - 4);` // 6

- **Multiplication (`*`):**  
  `console.log(4 * 2);` // 8

- **Division (`/`):**  
  `console.log(20 / 5);` // 4

- **Remainder (`%`):**  
  `console.log(10 % 3);` // 1

### 6.2 Assignment Operators
- **Simple Assignment:**  
  `let result = 100;`
- **Combined Assignment (e.g., `+=`):**  
  ```js
  let x = 10;
  x += 5; // x is now 15
  ```

### 6.3 Comparison Operators
- **Equal (`==`) and Strict Equal (`===`):**  
  - `==` checks for equality of value.
  - `===` checks for equality of value and type.
  ```js
  console.log(5 == 5);      // true
  console.log(5 === '5');   // false
  ```

- **Not Equal (`!=`) and Strict Not Equal (`!==`):**
  ```js
  console.log(5 != 3);      // true
  console.log(5 !== '5');   // true
  ```

### 6.4 Logical Operators
- **AND (`&&`):** Returns true if both conditions are true.
- **OR (`||`):** Returns true if at least one condition is true.
- **NOT (`!`):** Inverts a boolean value.

---