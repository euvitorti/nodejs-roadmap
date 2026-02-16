## Why Use Node.js?

* **Speed:** Thanks to the V8 engine and non-blocking I/O.
* **JavaScript Everywhere:** You can use the same language for the front-end (browser) and back-end (server).
* **NPM (Node Package Manager):** Access to the world's largest library of open-source packages to help build your app faster.

---

## Simple Code Example

Here is how a non-blocking "sandwich order" might look in code:

```javascript
const fs = require('fs');

// Non-blocking: We start reading a file and provide a 'callback' function
fs.readFile('sandwich_recipe.txt', 'utf8', (err, data) => {
    if (err) throw err;
    console.log("Your sandwich is ready: " + data);
});

console.log("Taking the next customer's order...");

```

**Output:**

1. `Taking the next customer's order...`
2. `Your sandwich is ready: [File Content]`

## Learn more

[5 Reasons to Choose Node.js](https://www.bitovi.com/blog/5-reasons-to-choose-nodejs)
