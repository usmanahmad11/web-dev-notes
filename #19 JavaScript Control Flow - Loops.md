# JavaScript Control Flow - Loops

## Introduction
Loops allow you to execute a block of code multiple times, making repetitive tasks easier to handle. JavaScript provides several types of loops, including `for`, `while`, and `do-while`. Understanding loops is essential for iterating over data and automating tasks.

## Learning Objectives
By the end of this lecture, you will:
- Learn how to use `for` loops and understand their structure.
- Understand `while` and `do-while` loops.
- Explore breaking and continuing loops.
- Learn how to loop through arrays.

## Content

### For Loops and Loop Structure
The `for` loop is used to repeat a block of code a specific number of times. It consists of three parts:
1. **Initialization**: Sets the starting value of the loop variable.
2. **Condition**: Specifies when the loop should stop.
3. **Increment/Decrement**: Updates the loop variable after each iteration.

#### Syntax:
```javascript
for (initialization; condition; increment) {
  // Code to execute
}
```

#### Example: For Loop
```javascript
for (let i = 0; i < 5; i++) {
  console.log('Iteration:', i);
}
```

#### Explanation:
- `let i = 0;` initializes the loop variable `i` to 0.
- `i < 5;` specifies that the loop runs while `i` is less than 5.
- `i++` increments `i` by 1 after each iteration.

### While and Do-While Loops
The `while` loop repeats a block of code as long as a condition is true. The `do-while` loop is similar but guarantees at least one iteration.

#### While Loop Syntax:
```javascript
while (condition) {
  // Code to execute
}
```

#### Example: While Loop
```javascript
let count = 0;

while (count < 3) {
  console.log('Count:', count);
  count++;
}
```

#### Explanation:
- The loop runs while `count` is less than 3.
- `count++` increments the variable after each iteration.

#### Do-While Loop Syntax:
```javascript
do {
  // Code to execute
} while (condition);
```

#### Example: Do-While Loop
```javascript
let count = 0;

do {
  console.log('Count:', count);
  count++;
} while (count < 3);
```

#### Explanation:
- The loop executes the code block once before checking the condition.

### Breaking and Continuing Loops
You can control the flow of loops using `break` and `continue`.

#### `break`
The `break` statement exits the loop immediately.

#### Example: Breaking a Loop
```javascript
for (let i = 0; i < 5; i++) {
  if (i === 3) {
    break; // Exit the loop when i equals 3
  }
  console.log('Iteration:', i);
}
```

#### `continue`
The `continue` statement skips the current iteration and moves to the next one.

#### Example: Continuing a Loop
```javascript
for (let i = 0; i < 5; i++) {
  if (i === 3) {
    continue; // Skip the iteration when i equals 3
  }
  console.log('Iteration:', i);
}
```

### Looping Through Arrays
You can use loops to iterate over arrays and access their elements.

#### Example: Looping Through an Array with a For Loop
```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];

for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}
```

#### Explanation:
- `fruits.length` returns the number of elements in the array.
- `fruits[i]` accesses the element at index `i`.

#### Example: Looping Through an Array with a For-Of Loop
The `for-of` loop is a simpler way to iterate over arrays.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];

for (let fruit of fruits) {
  console.log(fruit);
}
```

#### Explanation:
- The `for-of` loop iterates directly over the values in the array.

### Viewing Your JavaScript Program
To test your JavaScript code:
1. Save the code in an HTML file with a `<script>` tag or in a `.js` file.
2. Open the file in a web browser and use the developer tools console to view the output.

## Exercises
1. Write a program that:
   - Uses a `for` loop to print numbers from 1 to 10.
   - Uses a `while` loop to print numbers from 10 to 1.

2. Create a program that:
   - Iterates over an array of colors using a `for` loop.
   - Skips the color `'red'` using the `continue` statement.

3. Write a program that:
   - Uses a `do-while` loop to prompt the user for input until they enter `'exit'`.

## Summary
Loops allow you to repeat code efficiently. Use `for` loops for fixed iterations, `while` loops for conditional repetition, and `do-while` loops for guaranteed execution. The `break` and `continue` statements control loop flow, while looping through arrays simplifies data manipulation.

## Further Reading
- [JavaScript Loops - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)
- [JavaScript For Loop - W3Schools](https://www.w3schools.com/js/js_loop_for.asp)
- [JavaScript While Loop - W3Schools](https://www.w3schools.com/js/js_loop_while.asp)
