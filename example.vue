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