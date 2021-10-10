Setup
- Go to a folder with the terminal

Vue
- $ yarn create vite my-project --template vue
- $ cd my-project
- $ yarn
- $ yarn dev

Tailwind
- $ yarn add -D tailwindcss@latest postcss@latest autoprefixer@latest
- $ npx tailwindcss init -p
- Change purge in tailwind.config.js to purge: ['./index.html', './src/**/*.{vue,js,ts,jsx,tsx}'],
- Create /src/tailwind.css
- Add below
@import "tailwindcss/base";
@import "components/buttons.css";
@import "tailwindcss/utilities";

Tailwind postcss-import
- Edit /src/main.js and add import "./tailwind.css"; before the line that starts with createApp
- $ yarn add -D postcss-import
