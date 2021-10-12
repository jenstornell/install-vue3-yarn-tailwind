# Tailwind (optional)

### Install Tailwind

It's installed with Yarn because it's known to be faster than NPM.

```
yarn add -D tailwindcss postcss
```

### Add `postcss.config.js` and `tailwind.config.js`

To be able to change configuration, it's better to have these files visible.

```
npx tailwindcss init -p
```

### Set purge options

Purge is a way to only add the CSS you need.

In the `tailwind.config.js` change the purge option to the below:

```
purge: ['./index.html', './src/**/*.{vue,js,ts,jsx,tsx}'],
```

### Add tailwind.css 

In the `/src` folder, add `tailwind.css`. You need it to add custom CSS or import additional stylesheet files.

### Set tailwind.css imports

In the tailwind.css you need to add the tailwind imports.

```
@import "tailwindcss/base";
@import "tailwindcss/components";
@import "tailwindcss/utilities";
```
