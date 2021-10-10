# How to install Vue3 with ViteJS and Yarn

**Instructions for Tailwind, PostcssImport, nesting, autoprefixer**

## Setup

1. Install NodeJS
2. Install Yarn
3. Go to a folder with the terminal

## Install Vue

In the termial in the folder you just created, do the following:

### Create a project

Change `my-project` to anything you like.

```
yarn create vite my-project --template vue
```

Go the your project folder.

```
cd my-project
```

### Run the installation

```
yarn
```

### Start the server

```
yarn dev
```

To make sure the server is working go to `https://localhost:3000` or where it says it's installed.

Tailwind
- $ yarn add -D tailwindcss@latest postcss@latest autoprefixer@latest
- $ npx tailwindcss init -p
- Change purge in tailwind.config.js to purge: ['./index.html', './src/**/*.{vue,js,ts,jsx,tsx}'],
- Create /src/tailwind.css
- Add below
@import "tailwindcss/base";
@import "components/buttons.css";
@import "tailwindcss/utilities";

postcss.config.js
module.exports = {
  plugins: [
    require("postcss-import"),
    require("tailwindcss/nesting"),
    require("tailwindcss"),
    require("autoprefixer"),
  ],
};

Tailwind postcss-import
- Edit /src/main.js and add import "./tailwind.css"; before the line that starts with createApp
- $ yarn add -D postcss-import

Tailwind nesting
Nothing needs to be imported
