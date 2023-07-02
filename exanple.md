If you want to use Vue.js without a build step (like Vite or Webpack), you can include it directly in your HTML files via a `<script>` tag. This is known as using Vue through a CDN (Content Delivery Network). Here's how you can do it:

1. Include Vue.js in your HTML file:

```html
<!DOCTYPE html>
<html>
<head>
  <!-- Include Vue.js from a CDN -->
  <script src="https://unpkg.com/vue@next"></script>
</head>
<body>
  <!-- Your Vue.js code will go here -->
</body>
</html>
```

2. Create a Vue app:

Now you can create a Vue application in a `<script>` tag in your HTML file. Here's a simple example:

```html
<!DOCTYPE html>
<html>
<head>
  <script src="https://unpkg.com/vue@next"></script>
</head>
<body>
  <div id="app">
    {{ message }}
  </div>

  <script>
    const App = {
      data() {
        return {
          message: 'Hello Vue 3!'
        }
      }
    }

    Vue.createApp(App).mount('#app')
  </script>
</body>
</html>
```

In this example, we're creating a new Vue app and mounting it to the `#app` element. We're also defining some reactive data (`message`) that we're using in our template.

Please note that while this approach is great for small projects or for learning Vue.js, it's not ideal for larger projects. For larger projects, it's recommended to use a build step (like Vite or Webpack) to help manage your project's complexity and to take advantage of features like single-file components, hot module replacement, ES6 modules, etc.