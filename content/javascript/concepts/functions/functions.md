---
Title: "Functions"
Subjects:
  - "Web Development"
  - "Computer Science"
Tags: 
  - "Functions"
  - "Parameters"
  - "Arguments"
CatalogContent:
  - "introduction-to-javascript"
  - "paths/front-end-engineer-career-path"
---

Functions are one of the fundamental building blocks in JavaScript. A function is a reusable set of statements to perform a task or calculate a value. Functions can be passed one or more values and can return a value at the end of their execution. In order to use a function, you must define it somewhere in the scope where you wish to call it.

## Function Declaration

Function declarations are used to create named functions. These functions can be called using their declared name. Function declarations are built from:

- The function keyword.
- The function name.
- An optional list of parameters separated by commas enclosed by a set of parentheses `()`.
- A function body enclosed in a set of curly braces `{}`.

The example code provided contains a function named `add()` that takes in 2 values and prints the sum of those numbers:

```js
function add(number1, number2) {
  console.log(number1 + number2);
}
```

## Calling Functions

Functions can be called, or executed, elsewhere in code using parentheses following the function name. When a function is called, the code inside its function body runs. Arguments are values passed into a function when it is called.

```js
// Defining the function
function sum(num1, num2) {
  return num1 + num2;
}
 
// Calling the function
sum(2, 4);
```

The output would be:

```output
6
```

## Return Keyword

Functions return (pass back) values using the `return` keyword. `return` ends function execution and returns the specified value to the location where it was called. 

A common mistake is to forget the `return` keyword, in which case the function will return undefined by default.

```js
// With return
function sum(num1, num2) {
  return num1 + num2;
}
 
// Without return, so the function doesn't output the sum
function sum(num1, num2) {
  num1 + num2;
}
```

## Arrow Functions

Arrow function expressions were introduced in ES6. These expressions are clean and concise. The syntax for an arrow function expression does not require the `function` keyword and uses a fat arrow `=>` to separate the parameter(s) from the body.

There are several variations of arrow functions:

* Arrow functions with a single parameter do not require `()` around the parameter list.
* Arrow functions with a single expression can use the concise function body which returns the result of the expression without the `return` keyword.

Arrow function with no arguments:

```js
const printHello = () => { 
  console.log('hello'); 
}; 

printHello(); 
// Output: hello
```

Arrow function with a single argument:

```js
const checkWeight = weight => { 
  console.log(`Baggage weight : ${weight} kilograms.`); 
}; 

checkWeight(25); 
// Output: Baggage weight : 25 kilograms.
```

Arrow function with two arguments:

```js
const sum = (firstParam, secondParam) => { 
  return firstParam + secondParam; 
}; 

console.log(sum(2, 5)); 
// Output: 7 
```

Concise arrow function:

```js
const multiply = (a, b) => a * b; 

console.log(multiply(2, 30)); 
// Output: 60
```

## Anonymous Functions

Anonymous functions in JavaScript do not have a name property. They can be defined using the `function` keyword, or as an arrow function. See the code example for the difference between a named function and an anonymous function.

```js
// Named function
function rocketToMars() {
  return 'BOOM!';
}
 
// Anonymous function
const rocketToMars = function() {
  return 'BOOM!';
}
```
