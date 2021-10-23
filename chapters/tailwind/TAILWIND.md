# Tailwind

### Install Tailwind

```
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest
```

### Add `postcss.config.js` and `tailwind.config.js`

To be able to change configuration, it's good to have `postcss.config.js` and `tailwind.config.js` visible.

```
npx tailwindcss init -p
```

### Edit `tailwind.config.js`

In the `tailwind.config.js` change the JIT and purge option like below.

```js
module.exports = {
  mode: "jit",
  purge: ["./index.html", "./src/**/*.{vue,js,ts,jsx,tsx}"],
};
```

### Add `src/tailwind.css`

In the `/src` folder, add `tailwind.css` with the contents below.

```css
@import "tailwindcss/base";
@import "tailwindcss/components";
@import "tailwindcss/utilities";
```

### Edit `src/main.js`

Add `import './tailwind.css'` to your `/src/main.js` like below.

```js
import { createApp } from "vue";
import App from "./App.vue";
import "./tailwind.css";

createApp(App).mount("#app");
```
