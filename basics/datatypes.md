# Data Types in JS
# 🔐 Closures in JavaScript

✅ What is a Closure?
A closure is a function that remembers variables from its outer scope, even after the outer function has finished executing.

📦 Example:

### js
function outer() {
  let count = 0;
  return function inner() {
    count++;
    console.log(count);
  }
}

const counter = outer();
counter(); // 1
counter(); // 2
