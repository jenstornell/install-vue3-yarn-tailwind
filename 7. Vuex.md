# VueX

## Install Vuex

```
npm install vuex
```

### Add `store/index.js`

1. Add a folder called `store` in `src`.
2. Add a file called `index.js` in `src/store`.

Edit the `src/store/index.js` file like below.

```js
import { createStore } from "vuex";

export default createStore({
  state() {
    return {
      count: 0,
    };
  },
  mutations: {
    increment(state) {
      state.count++;
    },
  },
});
```

### Edit `main.js`

```js
import { createApp } from "vue";
import App from "./App.vue";
import "./tailwind.css";
import store from "./store";

createApp(App).use(store).mount("#app");
```

### Edit your component

Directly after `<script setup>` add the code below.

```js
import { useStore } from "vuex";
const store = useStore();
store.commit("increment");
```

Add The following to your template.

```html
{{ store.state.count }}
```
