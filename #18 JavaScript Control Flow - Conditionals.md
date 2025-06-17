# JavaScript Control Flow - Conditionals

## Introduction
Control flow allows you to dictate the behavior of your program based on conditions. JavaScript provides several tools for implementing conditional logic, including `if`, `else if`, `else`, `switch`, and the ternary operator. Understanding control flow is essential for writing dynamic and responsive programs.

## Learning Objectives
By the end of this lecture, you will:
- Learn how to use `if`, `else if`, and `else` statements.
- Understand how to use `switch` statements for multiple conditions.
- Explore the ternary operator for concise conditional expressions.
- Understand Boolean logic and truthiness in JavaScript.

## Content

### If, Else If, and Else Statements
The `if` statement executes a block of code if a condition is true. You can use `else if` for additional conditions and `else` for a fallback.

#### Syntax:
```javascript
if (condition) {
  // Code to execute if condition is true
} else if (anotherCondition) {
  // Code to execute if anotherCondition is true
} else {
  // Code to execute if none of the conditions are true
}
```

#### Example: If, Else If, and Else
```javascript
let age = 20;

if (age < 18) {
  console.log('You are a minor.');
} else if (age >= 18 && age < 65) {
  console.log('You are an adult.');
} else {
  console.log('You are a senior.');
}
```

#### Explanation:
- The `if` block checks if `age` is less than 18.
- The `else if` block checks if `age` is between 18 and 65.
- The `else` block executes if none of the conditions are true.

### Switch Statements
The `switch` statement evaluates an expression and matches it against multiple cases. It is useful for handling multiple conditions.

#### Syntax:
```javascript
switch (expression) {
  case value1:
    // Code to execute if expression matches value1
    break;
  case value2:
    // Code to execute if expression matches value2
    break;
  default:
    // Code to execute if no cases match
}
```

#### Example: Switch Statement
```javascript
let day = 'Monday';

switch (day) {
  case 'Monday':
    console.log('Start of the work week.');
    break;
  case 'Friday':
    console.log('End of the work week.');
    break;
  case 'Saturday':
  case 'Sunday':
    console.log('Weekend!');
    break;
  default:
    console.log('Midweek day.');
}
```

#### Explanation:
- The `switch` statement matches the value of `day` against the cases.
- The `break` statement prevents execution from falling through to the next case.
- Multiple cases (`'Saturday'` and `'Sunday'`) can share the same code block.

### Ternary Operator
The ternary operator is a shorthand for `if-else` statements. It evaluates a condition and returns one of two values.

#### Syntax:
```javascript
condition ? valueIfTrue : valueIfFalse;
```

#### Example: Ternary Operator
```javascript
let age = 20;
let message = age >= 18 ? 'You are an adult.' : 'You are a minor.';
console.log(message); // Output: You are an adult.
```

#### Explanation:
- The condition `age >= 18` is evaluated.
- If true, `'You are an adult.'` is returned; otherwise, `'You are a minor.'` is returned.

### Boolean Logic and Truthiness
Boolean logic involves combining conditions using logical operators (`&&`, `||`, `!`). Truthiness refers to whether a value is considered `true` or `false` in a Boolean context.

#### Truthy Values:
- Non-zero numbers (`1`, `-1`)
- Non-empty strings (`'hello'`)
- Objects and arrays (`{}`, `[]`)

#### Falsy Values:
- `false`
- `0`
- `''` (empty string)
- `null`
- `undefined`
- `NaN`

#### Example: Boolean Logic and Truthiness
```javascript
let name = 'Alice';
let isLoggedIn = true;

if (name && isLoggedIn) {
  console.log('Welcome, Alice!');
} else {
  console.log('Please log in.');
}
```

#### Explanation:
- The `if` condition checks if both `name` and `isLoggedIn` are truthy.
- If either value is falsy, the `else` block executes.

### Viewing Your JavaScript Program
To test your JavaScript code:
1. Save the code in an HTML file with a `<script>` tag or in a `.js` file.
2. Open the file in a web browser and use the developer tools console to view the output.

## Exercises
1. Write a program that:
   - Checks if a number is positive, negative, or zero using `if`, `else if`, and `else`.
   - Logs the result to the console.

2. Create a program that:
   - Uses a `switch` statement to log different messages based on the value of a variable (`'red'`, `'blue'`, `'green'`).
   - Includes a `default` case for unrecognized values.

3. Write a program that:
   - Uses the ternary operator to check if a user is logged in and display a welcome message or a login prompt.
   - Demonstrates truthy and falsy values in a conditional statement.

## Summary
JavaScript control flow allows you to execute code based on conditions. Use `if`, `else if`, and `else` for flexible conditional logic, and `switch` for handling multiple cases. The ternary operator provides a concise way to write conditional expressions, while Boolean logic and truthiness help evaluate complex conditions.

## Further Reading
- [JavaScript If Statements - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else)
- [JavaScript Switch Statements - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch)
- [JavaScript Ternary Operator - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator)
