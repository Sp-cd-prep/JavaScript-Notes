
### 1. JavaScript Introduction:
JavaScript (JS) is a high-level, dynamic, and versatile programming language primarily used for front-end web development. It allows you to add interactivity and dynamic behavior to websites. Here are some key features of JavaScript:

- **Interactivity:** JavaScript enables you to create interactive web pages by responding to user actions like clicks, inputs, and more.

- **Versatility:** It can be used not only for web development but also for server-side scripting (Node.js), game development, mobile app development, and more.

- **Dynamic:** JavaScript is dynamically typed, meaning you don't need to declare variable types explicitly.

- **Client-Side:** In web development, it's mainly used for client-side scripting, meaning it runs in the user's browser.

- **Easy to Learn:** It has a relatively low entry barrier for beginners.

### 2. JavaScript Variables:
Variables are used to store data in JavaScript. There are three ways to declare variables:

- **let:** Variables declared with `let` can be reassigned, and they have block scope.

  ```javascript
  let x = 5;
  x = 10; // You can reassign 'x'
  ```

- **const:** Variables declared with `const` cannot be reassigned, but they also have block scope.

  ```javascript
  const pi = 3.14159;
  // pi = 3.14; // This will result in an error, you can't reassign 'pi'
  ```

- **var:** Variables declared with `var` can be reassigned and have function scope (or global scope if declared outside any function). However, it's considered outdated, and it's better to use `let` and `const` for better scoping.

### 3. JavaScript Data Types:
JavaScript has several data types, including:

- **Number:** Represents numeric values. It can be integers or floating-point numbers.

  ```javascript
  let age = 30;
  let price = 19.99;
  ```

- **String:** Represents text. You can use single or double quotes to create strings.

  ```javascript
  let name = "John";
  let message = 'Hello, World!';
  ```

- **Undefined:** Represents a variable that has been declared but has no value assigned to it.

  ```javascript
  let x;
  console.log(x); // Outputs 'undefined'
  ```

- **null:** Represents an intentional absence of any object or value.

  ```javascript
  let empty = null;
  ```

- **Boolean:** Represents true or false values.

  ```javascript
  let isTrue = true;
  let isFalse = false;
  ```

- **Symbol:** Introduced in ES6, Symbols are unique and immutable values often used as object property keys.

  ```javascript
  const uniqueKey = Symbol('description');
  ```

- **Non-primitive Data Types:** These include Objects and Functions, which are more complex data structures.

  ```javascript
  let person = { name: "Alice", age: 25 };
  let greet = function() {
      console.log("Hello!");
  };
  ```


### JavaScript Operators

#### 1. Arithmetic Operators
Arithmetic operators are used to perform mathematical operations in JavaScript. Here are some common ones:

- **Addition (+):** Adds two numbers.

  ```javascript
  let sum = 5 + 3; // sum is 8
  ```

- **Subtraction (-):** Subtracts one number from another.

  ```javascript
  let difference = 10 - 3; // difference is 7
  ```

- **Multiplication (*):** Multiplies two numbers.

  ```javascript
  let product = 4 * 6; // product is 24
  ```

- **Division (/):** Divides one number by another.

  ```javascript
  let quotient = 15 / 3; // quotient is 5
  ```

- **Modulus (%):** Returns the remainder of a division.

  ```javascript
  let remainder = 10 % 3; // remainder is 1
  ```

#### 2. Relational Operators
Relational operators are used to compare values. They return a Boolean result (true or false).

- **Equality (==):** Checks if two values are equal, but it may perform type coercion.

  ```javascript
  5 == "5"; // true (value comparison, type coerced)
  ```

- **Inequality (!=):** Checks if two values are not equal, but it may perform type coercion.

  ```javascript
  5 != "6"; // true (value comparison, type coerced)
  ```

- **Strict Equality (===):** Checks if two values are equal without type coercion (same value and same type).

  ```javascript
  5 === "5"; // false (strict equality)
  ```

- **Strict Inequality (!==):** Checks if two values are not equal without type coercion.

  ```javascript
  5 !== "5"; // true (strict inequality)
  ```

#### 3. Logical Operators
Logical operators are used to perform logical operations.

- **AND (&&):** Returns true if both operands are true.

  ```javascript
  true && true; // true
  true && false; // false
  ```

- **OR (||):** Returns true if at least one operand is true.

  ```javascript
  true || false; // true
  false || false; // false
  ```

- **NOT (!):** Negates the value of an operand.

  ```javascript
  !true; // false
  !false; // true
  ```

#### 4. Bitwise Operators
Bitwise operators perform operations on binary representations of numbers.

- **Bitwise AND (&):** Performs a bitwise AND operation.

  ```javascript
  5 & 3; // 1
  ```

- **Bitwise OR (|):** Performs a bitwise OR operation.

  ```javascript
  5 | 3; // 7
  ```

- **Bitwise XOR (^):** Performs a bitwise XOR (exclusive OR) operation.

  ```javascript
  5 ^ 3; // 6
  ```

#### 5. Increment vs. Decrement Operators
Increment and decrement operators are used to increase or decrease the value of a variable.

- **Increment (++):** Increases the value of a variable by 1.

  ```javascript
  let x = 5;
  x++; // x is now 6
  ```

- **Decrement (--):** Decreases the value of a variable by 1.

  ```javascript
  let y = 10;
  y--; // y is now 9
  ```

#### 6. Assignment Operators
Assignment operators are used to assign values to variables.

- **Assignment (=):** Assigns a value to a variable.

  ```javascript
  let z = 15;
  ```

- **Other Assignment Operators (e.g., +=, -=, *=, /=):** Perform an operation and assign the result to a variable in a single step.

  ```javascript
  let a = 5;
  a += 3; // Equivalent to: a = a + 3; (a is now 8)
  ```

#### 7. Ternary Operator (Conditional Operator)
The ternary operator is a shorthand for an if-else statement. It returns one of two values based on a condition.

```javascript
let age = 18;
let canVote = age >= 18 ? "Yes" : "No";
console.log(canVote); // "Yes"
```

#### 8. Nullish Coalescing Operator (??)
The nullish coalescing operator returns the right-hand operand when the left-hand operand is null or undefined; otherwise, it returns the left-hand operand.

```javascript
let value = null;
let defaultValue = "Default Value";
let result = value ?? defaultValue;
console.log(result); // "Default Value"
```

### Decision-Making Statements in JavaScript
#### 1. `if` Statement
The `if` statement is used for conditional execution of code. It evaluates a condition and executes a block of code if the condition is true.

**Syntax:**
```javascript
if (condition) {
    // Code to execute if the condition is true
}
```

**Example:**
```javascript
let age = 20;
if (age >= 18) {
    console.log("You are an adult.");
}
```

#### 2. `if-else` Statement
The `if-else` statement allows you to execute one block of code if a condition is true and another block of code if the condition is false.

**Syntax:**
```javascript
if (condition) {
    // Code to execute if the condition is true
} else {
    // Code to execute if the condition is false
}
```

**Example:**
```javascript
let isRaining = true;
if (isRaining) {
    console.log("Bring an umbrella.");
} else {
    console.log("No need for an umbrella.");
}
```

#### 3. Nested `if-else` Statement
You can nest `if-else` statements inside each other to handle more complex conditions.

**Syntax:**
```javascript
if (condition1) {
    // Code to execute if condition1 is true
    if (condition2) {
        // Code to execute if condition2 is true
    } else {
        // Code to execute if condition2 is false
    }
} else {
    // Code to execute if condition1 is false
}
```

**Example:**
```javascript
let score = 75;
if (score >= 60) {
    console.log("You passed.");
    if (score >= 90) {
        console.log("You got an A grade!");
    } else {
        console.log("You got a B grade.");
    }
} else {
    console.log("You failed.");
}
```

#### 4. Cascaded `if-else` Statement
A cascaded `if-else` statement is used when you have multiple conditions to check one after the other.

**Syntax:**
```javascript
if (condition1) {
    // Code to execute if condition1 is true
} else if (condition2) {
    // Code to execute if condition2 is true
} else if (condition3) {
    // Code to execute if condition3 is true
} else {
    // Code to execute if none of the conditions are true
}
```

**Example:**
```javascript
let grade = 'B';
if (grade === 'A') {
    console.log("Excellent!");
} else if (grade === 'B') {
    console.log("Good job!");
} else if (grade === 'C') {
    console.log("You can do better.");
} else {
    console.log("Needs improvement.");
}
```

#### 5. `switch-case` Statement
The `switch-case` statement is used to select one of many code blocks to be executed.

**Syntax:**
```javascript
switch (expression) {
    case value1:
        // Code to execute if expression === value1
        break;
    case value2:
        // Code to execute if expression === value2
        break;
    // More cases...
    default:
        // Code to execute if none of the cases match
}
```

**Example:**
```javascript
let dayOfWeek = 'Monday';
switch (dayOfWeek) {
    case 'Monday':
        console.log("It's the start of the week.");
        break;
    case 'Friday':
        console.log("Weekend is almost here!");
        break;
    default:
        console.log("It's a weekday.");
}
```

### 1. `break` Statement

The `break` statement is used to exit a loop prematurely when a certain condition is met. It is commonly used to terminate a loop early, preventing further iterations.

**Example: Using `break` in a `for` loop**

```javascript
for (let i = 1; i <= 10; i++) {
    if (i === 5) {
        break; // Exit the loop when i equals 5
    }
    console.log(i);
}
```

In this example, the loop runs from 1 to 10, but when `i` becomes equal to 5, the `break` statement is executed, and the loop terminates. So, only the numbers 1 through 4 are printed.

### 2. `continue` Statement

The `continue` statement is used to skip the current iteration of a loop and proceed to the next iteration. It allows you to skip over specific values or conditions without terminating the loop entirely.

**Example: Using `continue` in a `for` loop**

```javascript
for (let i = 1; i <= 5; i++) {
    if (i === 3) {
        continue; // Skip iteration when i equals 3
    }
    console.log(i);
}
```

In this example, when `i` is equal to 3, the `continue` statement is executed, and the loop proceeds to the next iteration. As a result, the number 3 is skipped in the output, and the loop continues to print 1, 2, 4, and 5.


### JavaScript Math functions

### 1. `Math.abs(x)`

- **Description:** Returns the absolute (positive) value of a number.

- **Example:**
   ```javascript
   let num = -5;
   let absoluteValue = Math.abs(num); // absoluteValue is 5
   ```

### 2. `Math.round(x)`

- **Description:** Rounds a number to the nearest integer.

- **Example:**
   ```javascript
   let num = 5.49;
   let rounded = Math.round(num); // rounded is 5
   ```

### 3. `Math.ceil(x)`

- **Description:** Rounds a number up to the nearest integer.

- **Example:**
   ```javascript
   let num = 5.01;
   let roundedUp = Math.ceil(num); // roundedUp is 6
   ```

### 4. `Math.floor(x)`

- **Description:** Rounds a number down to the nearest integer.

- **Example:**
   ```javascript
   let num = 5.99;
   let roundedDown = Math.floor(num); // roundedDown is 5
   ```

### 5. `Math.random()`

- **Description:** Generates a random decimal number between 0 (inclusive) and 1 (exclusive).

- **Example:**
   ```javascript
   let randomNumber = Math.random(); // Generates a random number between 0 and 1 (e.g., 0.123456)
   ```

### 6. `Math.max(x, y, z, ...)`

- **Description:** Returns the largest of zero or more numbers.

- **Example:**
   ```javascript
   let maxNumber = Math.max(10, 5, 20, 8); // maxNumber is 20
   ```

### 7. `Math.min(x, y, z, ...)`

- **Description:** Returns the smallest of zero or more numbers.

- **Example:**
   ```javascript
   let minNumber = Math.min(10, 5, 20, 8); // minNumber is 5
   ```

### 8. `Math.pow(x, y)`

- **Description:** Returns the value of x to the power of y.

- **Example:**
   ```javascript
   let result = Math.pow(2, 3); // result is 8 (2^3 = 8)
   ```

### 9. `Math.sqrt(x)`

- **Description:** Returns the square root of a number.

- **Example:**
   ```javascript
   let squareRoot = Math.sqrt(25); // squareRoot is 5 (√25 = 5)
   ```

### 10. `Math.PI`

- **Description:** A predefined constant representing the mathematical constant π (pi).

- **Example:**
   ```javascript
   let circleArea = Math.PI * Math.pow(5, 2); // Calculates the area of a circle with radius 5
   ```
### 11. `Math.trunc(x)`

- **Description:** Returns the integer part of a number by removing the fractional part, effectively truncating the decimal portion.

- **Example:**
   ```javascript
   let num = 5.78;
   let truncated = Math.trunc(num); // truncated is 5
   ```


### JavaScript Arrays

#### 1. JavaScript Arrays

Arrays in JavaScript are ordered collections of values under one variable name, where each value is assigned a unique index or we can access those values or elements using index no. and generally the index number starts from 0. 
They are versatile and commonly used to store and manipulate multiple data elements.

**Syntax of Creating an Array:**
```javascript
let fruits = ["apple", "banana", "cherry"];
```

**Accessing Elements:**
You can access elements in an array using square brackets and the index of the element.

```javascript
console.log(fruits[0]); // "apple"
console.log(fruits[1]); // "banana"
```

**Length Attribute:**
The `length` property of an array returns the number of elements in the array.

```javascript
console.log(fruits.length); // 3
```

**display the array elements:**

```javascript
let arr = [1,2,3,4,5,6]
for(i=0;i<arr.length;i++){
  console.log(arr[i]);
}
```
**find out all the even numbers from an array:**

```javascript
let arr = [1,2,3,4,5,6]
for(i=0;i<arr.length;i++){
  if(arr[i]%2===0)
  console.log(arr[i]);
}
```

**Add 3 to each element in an array:**

```javascript
let arr = [1,2,3,4,5,6]
for(i=0;i<arr.length;i++){
  arr[i]=arr[i]+3;
  console.log(arr[i]);
}
```

**Find out the maximum element in an array:**

```javascript
let arr = [4,5,8,2,7,1]
let max=arr[0];
for(i=0;i<arr.length;i++){
    if(arr[i]>max){
        max=arr[i];
    }
}
console.log(max);
```

**Sort the numbers in an array:**

```javascript
let arr = [4,5,8,2,7,1];
let c=0;
for(i=0;i<arr.length;i++){
    for(j=i+1;j<arr.length;j++){
        if(arr[i]>arr[j]){
            c=arr[i];
            arr[i]=arr[j];
            arr[j]=c;
        }
    }
    console.log(arr[i]);
}

s
```


**Multidimensional Array:**
JavaScript arrays can also hold other arrays, creating multidimensional arrays.

```javascript
let matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]];
console.log(matrix[1][2]); // Accesses the element 6
```

#### 2. Array Methods

JavaScript provides various methods to manipulate arrays effectively. Here are some commonly used array methods:

- **`map(callback)`**: Creates a new array by applying a callback function to each element of the original array.

   ```javascript
   let numbers = [1, 2, 3];
   let doubled = numbers.map(x => x * 2); // [2, 4, 6]
   ```

- **`filter(callback)`**: Creates a new array with elements that satisfy a condition defined in the callback function.

   ```javascript
   let scores = [85, 92, 78, 90, 88];
   let highScores = scores.filter(score => score >= 90); // [92, 90]
   ```

- **`reduce(callback)`**: Applies a callback function to reduce an array to a single value (e.g., summing all elements).

   ```javascript
   let numbers = [1, 2, 3, 4, 5];
   let sum = numbers.reduce((acc, current) => acc + current, 0); // 15
   ```

- **`indexOf(element)`**: Returns the first index at which a specified element is found in the array. Returns -1 if the element is not found.

   ```javascript
   let fruits = ["apple", "banana", "cherry"];
   let index = fruits.indexOf("banana"); // 1
   ```

- **`push(element)`**: Adds an element to the end of the array and returns the new length of the array.

   ```javascript
   let fruits = ["apple", "banana"];
   let newLength = fruits.push("cherry"); // 3
   ```

- **`pop()`**: Removes the last element from the array and returns that element.

   ```javascript
   let fruits = ["apple", "banana", "cherry"];
   let removed = fruits.pop(); // "cherry"
   ```

- **`shift()`**: Removes the first element from the array and returns that element.

   ```javascript
   let fruits = ["apple", "banana", "cherry"];
   let removed = fruits.shift(); // "apple"
   ```

- **`unshift(element)`**: Adds one or more elements to the beginning of the array and returns the new length.

   ```javascript
   let fruits = ["banana", "cherry"];
   let newLength = fruits.unshift("apple"); // 3
   ```

- **`slice(start, end)`**: Returns a new array containing elements from the original array within the specified range (from `start` to `end`, not inclusive).

   ```javascript
   let numbers = [1, 2, 3, 4, 5];
   let sliced = numbers.slice(1, 4); // [2, 3, 4]
   ```

- **`some(callback)`**: Checks if at least one element in the array satisfies the condition specified in the callback function. Returns `true` if any element meets the condition; otherwise, `false`.

   ```javascript
   let numbers = [1, 3, 5, 7, 9];
   let hasEven = numbers.some(x => x % 2 === 0); // false
   ```

- **`every(callback)`**: Checks if all elements in the array satisfy the condition specified in the callback function. Returns `true` if all elements meet the condition; otherwise, `false`.

   ```javascript
   let numbers = [2, 4, 6, 8, 10];
   let allEven = numbers.every(x => x % 2 === 0); // true
   ```

- **`concat(array)`**: Combines the current array with another array(s) and returns a new concatenated array.

   ```javascript
   let fruits1 = ["apple", "banana"];
   let fruits2 = ["cherry", "orange"];
   let combined = fruits1.concat(fruits2); // ["apple", "banana", "cherry", "orange"]
   ```

- **`splice(start, deleteCount, item1, item2, ...)`**: Changes the contents of an array by removing or replacing existing elements and/or adding new elements.

   ```javascript
   let fruits = ["apple", "banana", "cherry"];
   fruits.splice(1, 1, "orange", "grape"); // Removes "banana" and adds "orange" and "grape"
   ```

- **`reverse()`**: Reverses the order of elements in the array.

   ```javascript
   let numbers = [1, 2, 3, 4, 5];
   numbers.reverse(); // [5, 4, 3, 2, 1]
   ```

These array methods are powerful tools for manipulating and working with arrays in JavaScript. They are essential for tasks such as filtering data, transforming data, and modifying arrays to suit your specific needs in programming.
