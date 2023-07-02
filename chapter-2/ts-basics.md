TypeScript cheat sheet for beginners

1. **Basic Types**
   - TypeScript includes several data types like `string`, `number`, `boolean`, `array`, `any`, `unknown`, `void`, `null`, `undefined`, `never`, `object`, and more.
   - Example:
   ```typescript
   let isDone: boolean = false;
   let decimal: number = 6;
   let color: string = "blue";
   ```

2. **Interfaces**
   - Interfaces define the shape of an object.
   - Example:
   ```typescript
   interface LabelledValue {
     label: string;
   }

   function printLabel(labelledObj: LabelledValue) {
     console.log(labelledObj.label);
   }
   ```

3. **Classes**
   - TypeScript supports object-oriented programming and includes classes, inheritance, and interfaces.
   - Example:
   ```typescript
   class Greeter {
     greeting: string;
     constructor(message: string) {
       this.greeting = message;
     }
     greet() {
       return "Hello, " + this.greeting;
     }
   }
   ```

4. **Generics**
   - Generics allow you to write reusable code that works with different types.
   - Example:
   ```typescript
   function identity<T>(arg: T): T {
     return arg;
   }
   ```

5. **Enums**
   - Enums allow a developer to define a set of named constants.
   - Example:
   ```typescript
   enum Color {
     Red,
     Green,
     Blue,
   }
   let c: Color = Color.Green;
   ```

6. **Type Assertion**
   - Type assertion is like type casting in other languages, but it doesn't perform any special checking or restructuring of data.
   - Example:
   ```typescript
   let someValue: unknown = "this is a string";
   let strLength: number = (someValue as string).length;
   ```

7. **Using TypeScript with Vue.js**
   - With Vue 3 and Vue CLI, you can easily set up a new project to use TypeScript. You can define the types of your data, props, computed properties, and more.
   - Example:
   ```typescript
   import { defineComponent } from 'vue';

   export default defineComponent({
     name: 'App',
     data(): { message: string } {
       return {
         message: 'Hello Vue 3 with TypeScript!',
       };
     },
   });
   ```
   
Remember, TypeScript is a statically typed superset of JavaScript, meaning it adds new features to JavaScript, including static types. While TypeScript can help catch errors at compile-time and make your code more robust and maintainable, it's also more complex and has a steeper learning curve than plain JavaScript. So, it's beneficial for large-scale projects but might be overkill for smaller, simpler ones.