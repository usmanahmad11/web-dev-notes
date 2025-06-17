# JavaScript Objects

## Introduction
Objects are one of the fundamental data structures in JavaScript. They allow you to store data in key-value pairs and group related information together. Understanding objects is essential for organizing and managing complex data in your programs.

## Learning Objectives
By the end of this lecture, you will:
- Learn how to create objects using object literals and define properties.
- Understand how to access and modify object properties.
- Explore methods and the `this` keyword.
- Compare objects and arrays and understand when to use each.

## Content

### Object Literals and Properties
An object literal is a simple way to create an object by defining its properties directly.

#### Syntax:
```javascript
const objectName = {
  key1: value1,
  key2: value2,
};
```

#### Example: Object Literal
```javascript
const person = {
  name: 'Alice',
  age: 25,
  isStudent: true,
};

console.log(person); // Output: { name: 'Alice', age: 25, isStudent: true }
```

#### Explanation:
- `name`, `age`, and `isStudent` are keys (properties).
- `'Alice'`, `25`, and `true` are values associated with the keys.

### Accessing and Modifying Object Properties
You can access and modify object properties using dot notation or bracket notation.

#### Dot Notation
```javascript
console.log(person.name); // Output: Alice
person.age = 26; // Modify the age property
console.log(person.age); // Output: 26
```

#### Bracket Notation
```javascript
console.log(person['isStudent']); // Output: true
person['name'] = 'Bob'; // Modify the name property
console.log(person['name']); // Output: Bob
```

#### Explanation:
- Use dot notation for simple property names.
- Use bracket notation for property names with special characters or spaces.

### Methods and the `this` Keyword
Methods are functions defined inside an object. The `this` keyword refers to the object that the method belongs to.

#### Example: Object Methods
```javascript
const person = {
  name: 'Alice',
  age: 25,
  greet: function() {
    console.log('Hello, my name is ' + this.name + '!');
  },
};

person.greet(); // Output: Hello, my name is Alice!
```

#### Explanation:
- `greet` is a method of the `person` object.
- `this.name` refers to the `name` property of the `person` object.

#### Example: Arrow Functions and `this`
Arrow functions do not bind their own `this`. Avoid using arrow functions as methods in objects.

```javascript
const person = {
  name: 'Alice',
  greet: () => {
    console.log('Hello, my name is ' + this.name + '!'); // `this` is undefined
  },
};

person.greet(); // Output: Hello, my name is undefined!
```

### Objects vs Arrays - When to Use Each
Objects and arrays are both used to store data, but they serve different purposes.

#### Objects:
- Use objects to store data as key-value pairs.
- Ideal for representing entities with properties (e.g., a person, a car).

#### Example: Object
```javascript
const car = {
  brand: 'Toyota',
  model: 'Corolla',
  year: 2020,
};
console.log(car.brand); // Output: Toyota
```

#### Arrays:
- Use arrays to store ordered lists of data.
- Ideal for collections of similar items (e.g., a list of names, numbers).

#### Example: Array
```javascript
const fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits[0]); // Output: Apple
```

#### Comparison:
| Feature         | Objects                     | Arrays                     |
|-----------------|-----------------------------|----------------------------|
| Structure       | Key-value pairs             | Ordered list               |
| Access          | By key                      | By index                   |
| Use Case        | Represent entities          | Collections of similar data |

### Viewing Your JavaScript Program
To test your JavaScript code:
1. Save the code in an HTML file with a `<script>` tag or in a `.js` file.
2. Open the file in a web browser and use the developer tools console to view the output.

## Exercises
1. Create an object representing a book with properties like `title`, `author`, and `year`. Access and modify its properties using both dot and bracket notation.

2. Add a method to the book object that logs a message including the book's title and author. Use the `this` keyword.

3. Compare objects and arrays by:
   - Creating an object to represent a car with properties like `brand` and `model`.
   - Creating an array to store a list of car brands.

## Summary
Objects store data as key-value pairs and are ideal for representing entities with properties. Use dot or bracket notation to access and modify properties. Methods allow objects to perform actions, and the `this` keyword refers to the object itself. Choose objects for structured data and arrays for ordered collections.

## Further Reading
- [JavaScript Objects - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)
- [JavaScript Object Methods - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)
- [JavaScript Objects Tutorial - W3Schools](https://www.w3schools.com/js/js_objects.asp)
