# Quickstart template
The code from the video tutorial Getting started with Vue 3 + Vite in 2021 (feat. Tailwind CSS, Vue Router, Vuex, ESLint & Prettier): https://www.youtube.com/watch?v=O8epzPrsADI

After cloning, go to the project folder and install node modules
`npm install`

This is essentially a fresh install of Vue 3 + Vite, ESLint, Prettier, TailwindCSS, Vue Router, Vuex

### Create Vite App
`npm init @vitejs/app project-name`

### Install Tailwind + dependencies
`npm install -D tailwindcss@latest postcss@latest autoprefixer@latest`

### Install ESLint + Prettier
`npm install --save-dev eslint prettier eslint-plugin-vue eslint-config-prettier`

### Install Vue Router
`npm install vue-router@4`

### Install Vuex
`npm install vuex@next --save`

### Config Files
.eslintrc.js:
```
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
```

.prettierrc.js:
```
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
```

### Altro
Ho inserito una rotta, un dato nello store e un component giusto per avere degli esempi
