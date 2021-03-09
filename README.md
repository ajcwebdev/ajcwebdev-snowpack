### index.html

```html
<!doctype html>
<html>
  <head>
      <title>ajcwebdev</title>
  </head>
  
  <body>
    <h1>ajcwebdev</h1>
  </body>
</html>
```

### index.js

```javascript
import App from "./App.svelte";

let app = new App({
  target: document.body,
});

export default app;
```

### App.svelte

```html
<div class="App">
  <header class="App-header">
    <a
      class="App-link"
      href="https://svelte.dev"
      target="_blank"
      rel="noopener noreferrer"
    >
      Learn Svelte
    </a>
  </header>
</div>
```

### snowpack.config.js

```javascript
/** @type {import("snowpack").SnowpackUserConfig } */
module.exports = {
  plugins: [
    '@snowpack/plugin-svelte'
  ],
}
```