# Vue + Tailwind

Install Vue and Tailwind with no missing steps and completely without fluff.

Vue is installed with ViteJS and Tailwind uses JIT (Just In Time) which makes this installation increddible fast.

## Table of contents

### Required

1. [Vue](#vue)
1. [Tailwind](#tailwind)

### Optional

1. [Vue - Vuex](#vue)
1. [Vue - Vue Router](#vue-router)
1. [Tailwind - Autoprefixer](#autoprefixer)
1. [Tailwind - Nesting](#nesting)
1. [Tailwind - Import](#import)

<!--

## Setup environment

1. [NodeJS](chapters/environment/NODEJS.md)
1. [NPM](chapters/environment/NPM.md)

-->

## Vue

1. Start the terminal.
   1. Go to your projects folder like `cd projects`, or add one first with `mkdir projects`.
   1. Run `npm init vite@latest my-project -- --template vue` to setup `my-project` as project folder.
   1. Go to the folder with `cd my-project`.
   1. Run `npm install` to install Vue.
   1. Run `npm dev` to start the server.
1. Visit `http://localhost:3000` in your browser to see if it's running correctly.

[Detailed instructions](chapters/vue/VUE.md)

## Tailwind

1. Start the terminal.
   1. Run `npm install -D tailwindcss@latest postcss@latest` to install Tailwind.
   1. Run `npx tailwindcss init -p` to add `postcss.config.js` and `tailwind.config.js`.
1. Start a code editor.
   1. Edit `tailwind.config.js` and add `mode: "jit",` after `module.exports = {`.
   1. Edit `tailwind.config.js` and replace `purge: [],` with `purge: ["./index.html", "./src/**/*.{vue,js,ts,jsx,tsx}"],`.

[Detailed instructions](chapters/tailwind/TAILWIND.md)

## For Vue (optional)

<details>
  <summary><strong>Vuex</strong></summary>

### Vuex

1. Start the terminal.
   1. Go to your store folder like `cd projects/my-project` if you are not there already.
   1. Add a new folder with `mkdir store` to add a location for your store.
1. Start your code editor.
   1. Add a new file `index.js` and place it in your `store` folder.

EJ KLAR!!!

[Detailed instructions](chapters/vue/VUEX.md)

</details>
<details>
  <summary><strong>Vue Router</strong></summary>

### Vue Router

[Detailed instructions)](chapters/vue/VUE-ROUTER.md)

</details>

## For Tailwind (optional)

<details>
  <summary><strong>Autoprefixer</strong></summary>

### Autoprefixer

[Autoprefixer](https://www.npmjs.com/package/autoprefixer) is adding prefixed versions of new features for backward compability.

1. Start the terminal.
   1. Run `npm install -D autoprefixer@latest` to install Autoprefixer.
1. Start your code editor.
   1. Edit `postcss.config.js` and add `require("autoprefixer"),` after `require("tailwindcss"),`.

[Detailed instructions](chapters/tailwind/AUTOPREFIXER.md)

</details>
<details>
  <summary><strong>Nesting</strong></summary>

### Nesting

To enable nested CSS selectors, you can enable the built in nesting feature, which works like [SASS](https://sass-lang.com/guide#topic-3). You don't need to install an additional package.

1. Start the terminal.
1. Edit `postcss.config.js` and add `require("tailwindcss/nesting"),` just before `require("tailwindcss"),`.

[Detailed instructions)](chapters/tailwind/NESTING.md)

</details>
<details>
  <summary><strong>Import</strong></summary>

### Import

To enable [CSS @import](https://developer.mozilla.org/en-US/docs/Web/CSS/@import) like `@import 'menu.css';` you can install [PostCSS Import](https://www.npmjs.com/package/postcss-import).

1. Start the terminal.
   1. Run `npm install -D postcss-import` to install PostCSS Import.
1. Start your code editor.
   1. Edit `postcss.config.js` and add `require("postcss-import"),` after `plugins: [`.

[Detailed instructions](chapters/tailwind/POSTCSS-IMPORT.md)

</details>
