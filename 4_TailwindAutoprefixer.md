# Tailwind Autoprefixer

### Install Autoprefixer

```
npm install -D autoprefixer@latest
```

### Set postcss.config.js

It will run autoprefixer as a PostCSS plugin. Add `require("autoprefixer"),` where it belongs like below:

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
