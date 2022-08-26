# Configuration of Tailwind in Vue 3 + Vite

 (feat. Tailwind CSS, Vue Router, ESLint & Prettier)
 
 After cloning, go to the project folder and install node modules npm install

Since the Vue CLI does not support Vite as yet, we need to configure these things manually.
- Vite + Vue 3 app
- ESLint + Prettier
- Tailwind CSS
- Vue Router


Installation commands that I paste in:

Create Vite App
npm init @vitejs/app project-name

Install Tailwind + dependencies
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest

Install ESLint + Prettier
npm install --save-dev eslint prettier eslint-plugin-vue eslint-config-prettier

Install Vue Router
npm install vue-router@4


.eslintrc.js:
module.exports = {
extends: [
  'plugin:vue/vue3-essential',
  'prettier',
],
rules: {
  // override/add rules settings here, such as:
  'vue/no-unused-vars': 'error',
},
}

.prettierrc.js:
module.exports = {
    semi: false,
    tabWidth: 4,
    useTabs: false,
    printWidth: 80,
    endOfLine: 'auto',
    singleQuote: true,
    trailingComma: 'es5',
    bracketSpacing: true,
    arrowParens: 'always',
  }
