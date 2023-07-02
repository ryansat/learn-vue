1. **Installation**
   - Yarn can be installed globally on your system using npm:
   ```bash
   npm install -g yarn
   ```

2. **Initializing a New Project**
   - This will create a new `package.json` file:
   ```bash
   yarn init
   ```

3. **Adding Dependencies**
   - Add a package as a dependency for your project:
   ```bash
   yarn add [package]
   ```

4. **Adding Dev Dependencies**
   - Add a package as a development-only dependency:
   ```bash
   yarn add --dev [package]
   ```

5. **Upgrading Dependencies**
   - Upgrade a package to its latest version:
   ```bash
   yarn upgrade [package]
   ```
   
6. **Removing Dependencies**
   - Remove a package from your project:
   ```bash
   yarn remove [package]
   ```

7. **Installing All Dependencies**
   - Install all the dependencies defined in your `package.json` file:
   ```bash
   yarn install
   ```

8. **Running Scripts**
   - If you have defined scripts in your `package.json` file, you can run them with Yarn:
   ```bash
   yarn run [script]
   ```

9. **Creating a new Vite Project with Yarn**
   - Here's how you can create a new Vue 3 project with Vite using Yarn:
   ```bash
   yarn create @vitejs/app my-vue-app --template vue
   ```

Yarn provides a fast, reliable, and secure dependency management system. It caches every package it downloads, so you don't need to download it again. It also parallelizes operations, which can significantly speed up build times. However, it's worth noting that as of npm 5, many of the advantages of Yarn are less relevant, as npm has also implemented similar features.