# Vue + Tailwind

A really simple guide with great performance in mind. No missing steps and not fluff. Vue is installed with ViteJS which is super fast. Tailwind uses JIT (Just In Time) which also is really fast.

## Table of contents

1. [Vue](#vue)
1. [Vue - Vuex](#vue---vuex-and-vue-router)
1. [Vue - Vue Router](#vue---vuex-and-vue-router)
1. [Tailwind](#tailwind)
1. [Tailwind - Autoprefixer](#tailwind---autoprefixer-nesting-and-import)
1. [Tailwind - Nesting](#tailwind---autoprefixer-nesting-and-import)
1. [Tailwind - Import](#tailwind---autoprefixer-nesting-and-import)

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

### Vue - Vuex and Vue Router

<details>
  <summary><strong>Vuex (optional)</strong></summary>

1. Start the terminal.
1. Go to your store folder like `cd projects/my-project` if you are not there already.
1. Add a new folder with `mkdir store` to add a location for your store.
1. Start your code editor.
1. Add a new file `index.js` and place it in your `store` folder.

EJ KLAR!!!

[Detailed instructions](chapters/vue/VUEX.md)

</details>
<details>
  <summary><strong>Vue Router (optional)</strong></summary>

[Detailed instructions)](chapters/vue/VUE-ROUTER.md)

</details>

## Tailwind - Autoprefixer, Nesting and Import

<details>
  <summary><strong>Tailwind with Autoprefixer (optional)</strong></summary>

1. Run `npm install -D autoprefixer@latest` in the terminal to install Autoprefixer.
1. Edit `postcss.config.js` and add `require("autoprefixer"),` after `require("tailwindcss"),`.

[Detailed instructions](chapters/tailwind/AUTOPREFIXER.md)

</details>
<details>
  <summary><strong>Tailwind with Nesting (optional)</strong></summary>

1. Edit `postcss.config.js` and add `require("tailwindcss/nesting"),` just before `require("tailwindcss"),`.

[Detailed instructions)](chapters/tailwind/NESTING.md)

</details>
<details>
  <summary><strong>Tailwind with PostCSS Import (optional)</strong></summary>

[Detailed instructions](chapters/tailwind/POSTCSS-IMPORT.md)

</details>
