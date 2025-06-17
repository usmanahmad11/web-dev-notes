# JavaScript Functions

## Introduction
Functions are reusable blocks of code that perform specific tasks. They allow you to organize and modularize your code, making it easier to maintain and debug. JavaScript supports various ways to define functions, including function declarations, expressions, and arrow functions.

## Learning Objectives
By the end of this lecture, you will:
- Understand function declarations and expressions.
- Learn how to use parameters and arguments.
- Explore return statements and scope.
- Understand the basics of arrow functions.

## Content

### Function Declaration and Expression
Functions can be defined using **declarations** or **expressions**.

#### Function Declaration
A function declaration defines a named function.

#### Syntax:
```javascript
function functionName(parameters) {
  // Code to execute
}
```

#### Example: Function Declaration
```javascript
function greet(name) {
  console.log('Hello, ' + name + '!');
}

greet('Alice'); // Output: Hello, Alice!
```

#### Function Expression
A function expression defines a function as part of an expression. It can be anonymous or named.

#### Syntax:
```javascript
const functionName = function(parameters) {
  // Code to execute
};
```

#### Example: Function Expression
```javascript
const greet = function(name) {
  console.log('Hello, ' + name + '!');
};

greet('Bob'); // Output: Hello, Bob!
```

### Parameters and Arguments
Parameters are placeholders defined in the function declaration, while arguments are the actual values passed to the function when it is called.

#### Example: Parameters and Arguments
```javascript
function add(a, b) {
  console.log(a + b);
}

add(5, 10); // Output: 15
```

#### Explanation:
- `a` and `b` are parameters.
- `5` and `10` are arguments passed to the function.

### Return Statements and Scope
The `return` statement specifies the value a function should return to the caller. Scope determines the accessibility of variables within a function.

#### Example: Return Statement
```javascript
function multiply(a, b) {
  return a * b;
}

let result = multiply(4, 5);
console.log(result); // Output: 20
```

#### Explanation:
- The `return` statement returns the product of `a` and `b`.
- The returned value is stored in the `result` variable.

#### Example: Function Scope
```javascript
function calculate() {
  let x = 10; // Local scope
  console.log(x);
}

calculate(); // Output: 10
// console.log(x); // Error: x is not defined (x is local to the function)
```

#### Explanation:
- Variables declared inside a function are in local scope and cannot be accessed outside the function.

### Arrow Functions Basics
Arrow functions provide a concise syntax for writing functions. They are often used for shorter functions and callbacks.

#### Syntax:
```javascript
const functionName = (parameters) => {
  // Code to execute
};
```

#### Example: Arrow Function
```javascript
const greet = (name) => {
  console.log('Hello, ' + name + '!');
};

greet('Charlie'); // Output: Hello, Charlie!
```

#### Example: Implicit Return
If the function body contains only a single expression, you can omit the curly braces and `return` keyword.

```javascript
const add = (a, b) => a + b;

console.log(add(3, 7)); // Output: 10
```

#### Explanation:
- The expression `a + b` is implicitly returned.

### Viewing Your JavaScript Program
To test your JavaScript code:
1. Save the code in an HTML file with a `<script>` tag or in a `.js` file.
2. Open the file in a web browser and use the developer tools console to view the output.

## Exercises
1. Write a program that:
   - Declares a function using a function declaration.
   - Passes two arguments to the function and logs the result.

2. Create a program that:
   - Defines a function using a function expression.
   - Uses the `return` statement to return a value.

3. Write a program that:
   - Defines an arrow function to calculate the square of a number.
   - Uses implicit return for the arrow function.

## Summary
Functions are reusable blocks of code that simplify programming tasks. Use function declarations or expressions to define functions, and pass arguments to them for dynamic behavior. The `return` statement specifies the output of a function, while arrow functions provide a concise syntax for shorter functions.

## Further Reading
- [JavaScript Functions - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)
- [JavaScript Arrow Functions - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions)
- [JavaScript Functions Tutorial - W3Schools](https://www.w3schools.com/js/js_functions.asp)
