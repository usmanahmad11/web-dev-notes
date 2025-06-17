# JavaScript Operators and Expressions

## Introduction
Operators are symbols or keywords used to perform operations on values and variables. Expressions combine variables, values, and operators to produce a result. Understanding operators and expressions is essential for writing logic in JavaScript.

## Learning Objectives
By the end of this lecture, you will:
- Learn how to use arithmetic operators for calculations.
- Understand comparison operators for evaluating conditions.
- Explore logical operators for combining conditions.
- Learn assignment operators and operator precedence.

## Content

### Arithmetic Operators
Arithmetic operators perform mathematical operations on numbers.

#### Common Arithmetic Operators:
1. **`+`**: Addition
2. **`-`**: Subtraction
3. **`*`**: Multiplication
4. **`/`**: Division
5. **`%`**: Modulus (remainder)

#### Example: Arithmetic Operators
```javascript
let a = 10;
let b = 5;

console.log(a + b); // Output: 15 (Addition)
console.log(a - b); // Output: 5 (Subtraction)
console.log(a * b); // Output: 50 (Multiplication)
console.log(a / b); // Output: 2 (Division)
console.log(a % b); // Output: 0 (Modulus)
```

### Comparison Operators
Comparison operators are used to compare values and return a boolean (`true` or `false`).

#### Common Comparison Operators:
1. **`==`**: Equal to (compares values, ignores types)
2. **`===`**: Strict equal to (compares values and types)
3. **`!=`**: Not equal to
4. **`!==`**: Strict not equal to
5. **`<`**: Less than
6. **`>`**: Greater than
7. **`<=`**: Less than or equal to
8. **`>=`**: Greater than or equal to

#### Example: Comparison Operators
```javascript
let x = 10;
let y = '10';

console.log(x == y); // Output: true (values are equal)
console.log(x === y); // Output: false (values are equal, but types differ)
console.log(x != y); // Output: false (values are equal)
console.log(x !== y); // Output: true (values are equal, but types differ)
console.log(x > 5); // Output: true
console.log(x <= 10); // Output: true
```

### Logical Operators
Logical operators are used to combine or invert conditions.

#### Common Logical Operators:
1. **`&&`**: Logical AND (returns `true` if both conditions are true)
2. **`||`**: Logical OR (returns `true` if at least one condition is true)
3. **`!`**: Logical NOT (inverts the condition)

#### Example: Logical Operators
```javascript
let a = true;
let b = false;

console.log(a && b); // Output: false (both conditions are not true)
console.log(a || b); // Output: true (at least one condition is true)
console.log(!a); // Output: false (inverts the condition)
```

#### Combining Logical Operators:
```javascript
let age = 25;
let isStudent = true;

console.log(age > 18 && isStudent); // Output: true (both conditions are true)
console.log(age < 18 || isStudent); // Output: true (one condition is true)
```

### Assignment Operators
Assignment operators are used to assign values to variables.

#### Common Assignment Operators:
1. **`=`**: Assigns a value.
2. **`+=`**: Adds and assigns.
3. **`-=`**: Subtracts and assigns.
4. **`*=`**: Multiplies and assigns.
5. **`/=`**: Divides and assigns.
6. **`%=`**: Modulus and assigns.

#### Example: Assignment Operators
```javascript
let x = 10;

x += 5; // Equivalent to x = x + 5
console.log(x); // Output: 15

x -= 3; // Equivalent to x = x - 3
console.log(x); // Output: 12

x *= 2; // Equivalent to x = x * 2
console.log(x); // Output: 24

x /= 4; // Equivalent to x = x / 4
console.log(x); // Output: 6

x %= 2; // Equivalent to x = x % 2
console.log(x); // Output: 0
```

### Operator Precedence
Operator precedence determines the order in which operators are evaluated in an expression.

#### Example: Operator Precedence
```javascript
let result = 10 + 5 * 2; // Multiplication is evaluated first
console.log(result); // Output: 20

result = (10 + 5) * 2; // Parentheses change the precedence
console.log(result); // Output: 30
```

#### Precedence Order:
1. Parentheses `()`
2. Multiplication `*`, Division `/`, Modulus `%`
3. Addition `+`, Subtraction `-`
4. Comparison operators (`<`, `>`, `==`, `===`)
5. Logical operators (`&&`, `||`)

### Viewing Your JavaScript Program
To test your JavaScript code:
1. Save the code in an HTML file with a `<script>` tag or in a `.js` file.
2. Open the file in a web browser and use the developer tools console to view the output.

## Exercises
1. Write a program that:
   - Declares two variables and performs all arithmetic operations on them.
   - Logs the results to the console.

2. Create a program that:
   - Compares two values using `==` and `===`.
   - Combines two conditions using `&&` and `||`.

3. Write a program that:
   - Uses assignment operators (`+=`, `-=`, `*=`) to modify a variable.
   - Demonstrates operator precedence with parentheses.

## Summary
JavaScript operators allow you to perform calculations, compare values, and combine conditions. Arithmetic, comparison, logical, and assignment operators are essential for writing expressions. Understanding operator precedence ensures accurate evaluation of complex expressions.

## Further Reading
- [JavaScript Operators - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators)
- [JavaScript Expressions - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)
- [JavaScript Operators Tutorial - W3Schools](https://www.w3schools.com/js/js_operators.asp)