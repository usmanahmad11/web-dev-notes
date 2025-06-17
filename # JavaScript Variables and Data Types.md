# JavaScript Variables and Data Types

## Introduction
Variables are used to store data in JavaScript, and data types define the kind of data a variable can hold. Understanding how to declare variables and work with different data types is fundamental to programming in JavaScript.

## Learning Objectives
By the end of this lecture, you will:
- Learn how to declare variables using `let`, `const`, and `var`.
- Understand primitive data types like `string`, `number`, and `boolean`.
- Explore arrays and basic array methods.
- Learn variable naming conventions.

## Content

### Declaring Variables
Variables are containers for storing data. In JavaScript, you can declare variables using `let`, `const`, or `var`.

#### `let`
The `let` keyword is used to declare variables that can be reassigned.

#### Example: Using `let`
```javascript
let name = 'Alice'; // Declare a variable
console.log(name); // Output: Alice

name = 'Bob'; // Reassign the variable
console.log(name); // Output: Bob
```

#### `const`
The `const` keyword is used to declare variables that cannot be reassigned.

#### Example: Using `const`
```javascript
const age = 25; // Declare a constant variable
console.log(age); // Output: 25

// age = 30; // Error: Assignment to constant variable
```

#### `var`
The `var` keyword is an older way to declare variables. It has different scoping rules compared to `let` and `const`.

#### Example: Using `var`
```javascript
var city = 'New York'; // Declare a variable
console.log(city); // Output: New York

city = 'Los Angeles'; // Reassign the variable
console.log(city); // Output: Los Angeles
```

#### Key Differences:
- Use `let` for variables that may change.
- Use `const` for variables that should remain constant.
- Avoid `var` in modern JavaScript as it can lead to unexpected behavior due to its scoping rules.

### Primitive Data Types
JavaScript has several primitive data types:
1. **String**: Represents text.
2. **Number**: Represents numeric values.
3. **Boolean**: Represents `true` or `false`.

#### Example: String
```javascript
let greeting = 'Hello, World!';
console.log(greeting); // Output: Hello, World!
```

#### Example: Number
```javascript
let score = 100;
console.log(score); // Output: 100
```

#### Example: Boolean
```javascript
let isLoggedIn = true;
console.log(isLoggedIn); // Output: true
```

### Arrays and Basic Array Methods
An array is a collection of values stored in a single variable. Arrays can hold multiple data types.

#### Example: Declaring an Array
```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits); // Output: ['Apple', 'Banana', 'Cherry']
```

#### Accessing Array Elements
Array elements are accessed using their index (starting from 0).

```javascript
console.log(fruits[0]); // Output: Apple
console.log(fruits[1]); // Output: Banana
```

#### Basic Array Methods:
1. **`push()`**: Adds an element to the end of the array.
   ```javascript
   fruits.push('Orange');
   console.log(fruits); // Output: ['Apple', 'Banana', 'Cherry', 'Orange']
   ```

2. **`pop()`**: Removes the last element from the array.
   ```javascript
   fruits.pop();
   console.log(fruits); // Output: ['Apple', 'Banana', 'Cherry']
   ```

3. **`length`**: Returns the number of elements in the array.
   ```javascript
   console.log(fruits.length); // Output: 3
   ```

### Variable Naming Conventions
Follow these conventions when naming variables:
1. Use descriptive names that reflect the variable's purpose.
   ```javascript
   let userName = 'Alice'; // Good
   let x = 'Alice'; // Avoid
   ```

2. Use camelCase for multi-word variable names.
   ```javascript
   let firstName = 'Alice';
   let lastName = 'Smith';
   ```

3. Avoid starting variable names with numbers or special characters.
   ```javascript
   let 1name = 'Alice'; // Invalid
   let $name = 'Alice'; // Valid but avoid
   ```

4. Do not use reserved keywords as variable names.
   ```javascript
   let let = 'Alice'; // Invalid
   ```

### Viewing Your JavaScript Program
To test your JavaScript code:
1. Save the code in an HTML file with a `<script>` tag or in a `.js` file.
2. Open the file in a web browser and use the developer tools console to view the output.

## Exercises
1. Declare three variables using `let`, `const`, and `var`. Assign values to them and log the values to the console.
2. Create an array of your favorite colors. Use `push()` to add a new color and `pop()` to remove the last color.
3. Write a program that declares a variable for a user's name and logs a greeting message to the console.

## Summary
Variables store data in JavaScript, and data types define the kind of data they hold. Use `let` and `const` for modern variable declarations. Arrays allow you to store collections of values, and basic methods like `push()` and `pop()` help manipulate them. Follow naming conventions to write clean and readable code.

## Further Reading
- [JavaScript Variables - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#declarations)
- [JavaScript Data Types - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)
- [JavaScript Arrays - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)