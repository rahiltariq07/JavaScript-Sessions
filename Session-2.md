# Session 2: Conditionals, Loops, Functions, Arrays, and Objects

The session covers:

- **Conditionals**
- **Loops**
- **Functions**
- **Arrays**
- **Objects**

---

## 1. Conditionals

### What are Conditionals?

- **Purpose**:  
  - Allow the program to choose different paths based on conditions.
  - Execute different blocks of code depending on whether a condition is true or false.

### Types of Conditional Statements

- **if Statement**  
  Checks a condition and runs a code block if it’s true.

  ```js
  if (condition) {
    // code to execute if condition is true
  }
  ```


- **if-else Statement**  
  Provides an alternative block of code when the condition is false.

  ```js
  if (condition) {
    // code if condition is true
  } else {
    // code if condition is false
  }


- **else if Clause**  

  Tests multiple conditions in order.

  ```js
  if (condition1) {
    // code if condition1 is true
  } else if (condition2) {
    // code if condition2 is true
  } else {
    // code if none of the above conditions are true
  }
  ```

### Key Points

- Conditionals help in decision-making.
- The code stops checking further conditions once a true condition is found.

---

## 2. Loops

### What are Loops?

- **Purpose**:  
  - To repeat a block of code multiple times.
  - Prevents the need to write repetitive code.

### Types of Loops

- **for Loop**  
  Ideal when you know how many times you want to run the code.

  ```js
  for (let i = 0; i < 5; i++) {
    console.log('Iteration number:', i);
  }
  ```

- **while Loop**  
  Runs as long as the condition is true. The condition is checked before each iteration.

  ```js
  let i = 0;
  while (i < 5) {
    console.log('Count:', i);
    i++;
  }
  ```

- **do-while Loop**  
  Executes the code block once before checking the condition.

  ```js
  let i = 0;
  do {
    console.log('Value:', i);
    i++;
  } while (i < 5);
  ```

---

## 3. Functions

### What are Functions?

Functions are blocks of code that perform a specific task. They let us reuse code without writing the same lines again and again.

- **Purpose**:  
  - Group code into reusable blocks.
  
### Function Declaration

- **Basic Syntax:**

  ```js
  function functionName() {
    // code to execute
  }
  ```

  **Example:**

  ```js
  function sayHello() {
    console.log('Hello, everyone!');
  }
  // Call the function
  sayHello();
  ```

### Functions with Parameters and Return Values

- **Parameters**: Inputs that the function can process.
- **Return Value**: The output that the function gives back.

  ```js
  function add(a, b) {
    return a + b;
  }
  let sum = add(3, 4);
  console.log(sum);  // Prints 7
  ```

### Arrow Functions

- A shorter syntax for writing functions.

  ```js
  const multiply = (a, b) => {
    return a * b;
  };
  console.log(multiply(5, 2));  // Prints 10
  ```

---

## 4. Arrays

### What are Arrays?

- **Purpose**:  
  - Store a collection of values in a single variable.

### Array Structure

- **Syntax:**

  ```js
  let fruits = ['apple', 'banana', 'orange'];
  console.log(fruits);
  ```

- **Accessing Elements:**  
  - Elements are indexed starting at 0.
  
  ```js
  console.log(fruits[0]); // Prints 'apple'
  ```

### Looping Through Arrays

- **Using a for Loop:**

  ```js
  for (let i = 0; i < fruits.length; i++) {
    console.log('Fruit:', fruits[i]);
  }
  ```

---

## 5. Objects

### What are Objects?

- **Purpose**:  
  - Organize related data using key-value pairs.

### Object Structure

- **Syntax:**

  ```js
  let person = {
    name: 'Alice',
    age: 25,
    city: 'New York'
  };
  console.log(person);
  ```

- **Accessing Object Properties:**
  
  ```js
  console.log(person.name); // Prints 'Alice'
  ```

### Modifying Objects

- **Adding/Updating Properties:**

  ```js
  person.job = 'Developer';
  console.log(person);
  ```
