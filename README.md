Tailwind setup:

first install tailwind with command => npm install -D tailwindcss postcss autoprefixer

2-> run command => npx tailwindcss init -p (To get postcss configuration file)

3->in tailwind.config.js file replace
/** @type {import('tailwindcss').Config} \*/
module.exports = {
content: ["./src/**/\*.{html,js}"],
theme: {
extend: {},
},
plugins: [],
}

4-> in index.css paste
@tailwind base;
@tailwind components;
@tailwind utilities;

5-> Stop the server and restart. Your application works fine.
