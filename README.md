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
