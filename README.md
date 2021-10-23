# Vue + Tailwind

- A really simple guide
- Great performance in mind
- No missing steps and no fluff

## Table of contents

### Setup environment

1. [NodeJS](chapters/environment/NODEJS.md)
1. [NPM](chapters/environment/NPM.md)

## Install Vue

### Vue

1. Start the terminal.
1. Go to your projects folder like `cd projects`, or add one first with `mkdir projects`.
1. Run `npm init vite@latest my-project -- --template vue` to setup `my-project` as project folder.
1. Go to the folder with `cd my-project`.
1. Run `npm install` to install Vue.
1. Run `npm dev` to start the server.
1. Visit `http://localhost:3000` in your browser to see if it's running correctly.

[Detailed instructions](chapters/vue/VUE.md)

<details>
  <summary>### Vuex (optional)</summary>

1. Start the terminal.
1. Go to your store folder like `cd projects/my-project` if you are not there already.
1. Add a new folder with `mkdir store` to add a location for your store.
1. Start your code editor.
1. Add a new file `index.js` and place it in your `store` folder.

EJ KLAR!!!

[Detailed instructions](chapters/vue/VUEX.md)

</details>

### Vue Router (optional)

[Detailed instructions)](chapters/vue/VUE-ROUTER.md)

## Install Tailwind

### Tailwind

1. Start the terminal.
1. Run `npm install -D tailwindcss@latest postcss@latest` to install Tailwind.
1. Run `npx tailwindcss init -p` to add `postcss.config.js` and `tailwind.config.js`.
1. Start a code editor.
1. Edit `tailwind.config.js` and add `mode: "jit",` after `module.exports = {`.
1. Edit `tailwind.config.js` and replace `purge: [],` with `purge: ["./index.html", "./src/**/*.{vue,js,ts,jsx,tsx}"],`.

[Detailed instructions](chapters/tailwind/TAILWIND.md)

### Tailwind with Autoprefixer (optional)

1. Run `npm install -D autoprefixer@latest` in the terminal to install Autoprefixer.
1. Edit `postcss.config.js` and add `require("autoprefixer"),` after `require("tailwindcss"),`.

[Detailed instructions](chapters/tailwind/AUTOPREFIXER.md)

### Tailwind with Nesting (optional)

1. Edit `postcss.config.js` and add `require("tailwindcss/nesting"),` just before `require("tailwindcss"),`.

[Detailed instructions)](chapters/tailwind/NESTING.md)

### Tailwind with PostCSS Import (optional)

[Detailed instructions](chapters/tailwind/POSTCSS-IMPORT.md)
