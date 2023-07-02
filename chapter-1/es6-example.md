Sure, understanding ES6 (ECMAScript 2015) features is important as Vue.js frequently uses them. Here are some ES6 topics to include with examples:

1. **Let and Const**
   - These keywords are new ways to declare variables.
   ```javascript
   let variable = "I can be reassigned";
   const constant = "I cannot be reassigned";
   ```

2. **Arrow Functions**
   - Arrow functions offer a more concise syntax to declare functions and automatically bind `this`.
   ```javascript
   const numbers = [1, 2, 3, 4, 5];
   const doubled = numbers.map(number => number * 2); // [2, 4, 6, 8, 10]
   ```

3. **Template Literals**
   - Template literals are a new way to work with strings.
   ```javascript
   let name = "John";
   let greeting = `Hello, ${name}!`; // "Hello, John!"
   ```

4. **Destructuring Assignment**
   - Destructuring assignment syntax makes it possible to unpack values from arrays or properties from objects.
   ```javascript
   let [a, b] = [1, 2];
   let {name, age} = {name: "John", age: 30};
   ```

5. **Default Parameters**
   - Default function parameters allow named parameters to be initialized with default values if no value or undefined is passed.
   ```javascript
   function greet(name = "World") {
     return `Hello, ${name}!`;
   }
   ```

6. **Spread Operator**
   - The spread operator is used to expand elements of an iterable (like an array) in places where zero or more arguments or elements are expected.
   ```javascript
   let arr1 = [1, 2, 3];
   let arr2 = [...arr1, 4, 5, 6]; // [1, 2, 3, 4, 5, 6]
   ```

7. **Rest Parameters**
   - Rest parameters are used to create functions that can take a variable number of arguments.
   ```javascript
   function sum(...numbers) {
     return numbers.reduce((total, num) => total + num, 0);
   }
   ```

8. **Promises**
   - Promises are used to handle asynchronous operations.
   ```javascript
   let promise = new Promise((resolve, reject) => {
     // Async operation
   });

   promise.then(result => {
     // Handle result
   }).catch(error => {
     // Handle error
   });
   ```

9. **Async/Await**
   - Async/await make it easier to work with Promises.
   ```javascript
   async function fetchData() {
     try {
       let response = await fetch(url);
       let data = await response.json();
       // Handle data
     } catch (error) {
       // Handle error
     }
   }
   ```

10. **Modules (import/export)**
    - Modules are a way to split code into reusable parts.
    ```javascript
    // myModule.js
    export function hello() {
      return "Hello, world!";
    }

    // main.js
    import { hello } from './myModule.js';
    hello(); // "Hello, world!"
    ```  

These features are fundamental to modern JavaScript development and are extensively used in Vue.js. Each section can be expanded as needed to provide more detailed explanations and examples.