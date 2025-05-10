#  **JavaScript Session 3: Strings, Arrays, Date, and Math**

##  1. Strings

* A **string** is a set of characters written inside quotes.
* Example: `"Hello"` or `'JavaScript'`

###  Common String Methods:

| Method               | Description                  | Example                                 |
| -------------------- | ---------------------------- | --------------------------------------- |
| `.length`            | Returns number of characters | `"hello".length` → 5                    |
| `.toUpperCase()`     | Converts to uppercase        | `"hello".toUpperCase()` → `"HELLO"`     |
| `.toLowerCase()`     | Converts to lowercase        | `"HELLO".toLowerCase()` → `"hello"`     |
| `.includes("text")`  | Checks if text is in string  | `"hello".includes("he")` → `true`       |
| `.indexOf("text")`   | Finds position of text       | `"hello".indexOf("e")` → `1`            |
| `.replace("a", "b")` | Replaces part of string      | `"hello".replace("e", "a")` → `"hallo"` |
| `.slice(start, end)` | Cuts part of string          | `"hello".slice(0, 2)` → `"he"`          |

---

##  2. Arrays

* An **array** stores multiple values in one variable.

```javascript
let fruits = ["apple", "banana", "mango"];
```

###  Common Array Methods:

| Method            | Description                |
| ----------------- | -------------------------- |
| `.push(item)`     | Adds item at the end       |
| `.pop()`          | Removes last item          |
| `.shift()`        | Removes first item         |
| `.unshift(item)`  | Adds item at the beginning |
| `.includes(item)` | Checks if item is present  |
| `.indexOf(item)`  | Finds position of item     |
| `.join()`         | Converts array to string   |

 Example:

```javascript
let arr = ["a", "b"];
arr.push("c"); // ["a", "b", "c"]
arr.pop();     // ["a", "b"]
```

---

##  3. Date Object

* Used to work with current **date and time**.

```javascript
let today = new Date();
```

###  Date Methods:

| Method           | Description          |
| ---------------- | -------------------- |
| `.getFullYear()` | Returns year         |
| `.getMonth()`    | Returns month (0–11) |
| `.getDate()`     | Day of month         |
| `.getDay()`      | Day of week (0–6)    |

 Example:

```javascript
let d = new Date();
console.log(d.getFullYear());
```

---

##  4. Math Object

* Built-in object for mathematical operations.

###  Useful Math Methods:

| Method              | Description                  |
| ------------------- | ---------------------------- |
| `.round()`          | Rounds to nearest integer    |
| `.floor()`          | Rounds down                  |
| `.ceil()`           | Rounds up                    |
| `.max()` / `.min()` | Finds max or min             |
| `.random()`         | Gives random number (0 to 1) |
| `.sqrt()`           | Square root                  |

Example:

```javascript
console.log(Math.round(4.6)); // 5
console.log(Math.random());   // Random number
```

---

# DOM and Events

##  1. What is DOM?

* **DOM = Document Object Model**
* DOM is a tree structure of your webpage.
* Each HTML tag becomes a **node**.

---

##  2. `document` Keyword

* JavaScript uses the `document` object to talk to the webpage.
* It helps you **read**, **change**, or **remove** elements.

 Examples:

```javascript
document.getElementById("title");
document.querySelector("p");
```

---

##  3. Changing Content and Style

* Use `.innerText` or `.innerHTML` to change content.

```javascript
let title = document.getElementById("title");
title.innerText = "New Title";
```

* Use `.style` to change CSS styles:

```javascript
title.style.color = "red";
title.style.fontSize = "30px";
```

---

##  4. Events

* **Events** happen when user clicks, types, hovers, etc.
* We can use `addEventListener()` to respond.

 Example:

```javascript
let btn = document.getElementById("btn");
btn.addEventListener("click", function() {
  alert("You clicked me!");
});
```

 Common Events: `click`, `mouseover`, `keydown`, `submit`, `change`

---

## 5. Creating and Removing Elements

### Create New Element:

```javascript
let para = document.createElement("p");
para.innerText = "New paragraph";
document.body.appendChild(para);
```

### Remove Element:

```javascript
let old = document.getElementById("oldPara");
old.remove();
```

---

## Summary

* DOM lets JavaScript control HTML.
* Use `document` to get elements.
* Use `addEventListener()` to add events.
* You can create and delete elements dynamically.