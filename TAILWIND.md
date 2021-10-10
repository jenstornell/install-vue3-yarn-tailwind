# Step 2 - Tailwind (optional)

### Install Tailwind, PostCSS and Autoprefixer

It's installed with Yarn because it's known to be faster than NPM.

```
yarn add -D tailwindcss@latest postcss@latest autoprefixer@latest
```

### Add `postcss.config.js` and `tailwind.config.js`

To be able to change configuration, it's better to have these files visible.

```
npx tailwindcss init -p
```

### Set purge options

Purge is a way to only add the CSS you need.

In the tailwind.config.js change the purge option to the below:

```
purge: ['./index.html', './src/**/*.{vue,js,ts,jsx,tsx}'],
```

### Add tailwind.css 

In the /src folder, add tailwind.css. You need it to add custom CSS or import additional stylesheet files.

### Set tailwind.css imports

In the tailwind.css you need to add the tailwind imports.

```
@import "tailwindcss/base";
@import "tailwindcss/components";
@import "tailwindcss/utilities";
```

### Set postcss.config.js

It will enable imports from the tailwind.css file, nesting and autoprefixer. Minifier it build in and don't need to be added. Remove if there is something you don't need.

```
module.exports = {
  plugins: [
    require("postcss-import"),
    require("tailwindcss/nesting"),
    require("tailwindcss"),
    require("autoprefixer"),
  ],
};
```

### Tailwind postcss-import

Edit /src/main.js and add import "./tailwind.css"; before the line that starts with createApp

```
yarn add -D postcss-import
```

### Tailwind nesting

Nesting it included by default so it does not need to be installed. Just make sure it's added in the postcss.config.js like above.
