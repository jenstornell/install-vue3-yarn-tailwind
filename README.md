# Vue + Tailwind

- A really simple guide
- Great performance in mind
- No missing steps and no fluff

### Setup environment

1. [NodeJS](chapters/environment/NODEJS.md)
1. [NPM](chapters/environment/NPM.md)

### Install Vue with Vite

1. [Vue](chapters/vue/VUE.md)
1. [Vuex (optional)](chapters/vue/VUEX.md)
1. [Vue Router (optional)](chapters/vue/VUE-ROUTER.md)

## Install Tailwind

### Tailwind

[Tailwind - Detailed instructions](chapters/tailwind/TAILWIND.md)

1. Run `npm install -D tailwindcss@latest postcss@latest` to install Tailwind.
1. Run `npx tailwindcss init -p` in the terminal to add `postcss.config.js` and `tailwind.config.js`.
1. Add `mode: "jit",` after `module.exports = {` in your `tailwind.config.js`.
1. Replace `purge: [],` with `purge: ["./index.html", "./src/**/*.{vue,js,ts,jsx,tsx}"],` in your `tailwind.config.js`.

### Autoprefixer

1. [Autoprefixer (optional)](chapters/tailwind/AUTOPREFIXER.md)
1. [Nesting (optional)](chapters/tailwind/NESTING.md)
1. [PostCSS Import (optional)](chapters/tailwind/POSTCSS-IMPORT.md)

If you have something to say, just add an issue.
