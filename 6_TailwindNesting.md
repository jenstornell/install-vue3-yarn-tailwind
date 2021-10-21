# Tailwind Nesting

### postcss.config.js

Look for the line with `require("tailwindcss/nesting"),` and insert it in the right place in your `postcss.config.js`.

```js
module.exports = {
  plugins: [
    // require("postcss-import"),
    require("tailwindcss/nesting"),
    require("tailwindcss"),
    // require("autoprefixer"),
  ],
};
```

### That's it!

Nesting it included by default. It does not need to be installed. Just make sure it's added in the `postcss.config.js` like above.
