- npm init @eslint/config

  - To check syntax, find problems, and enforce code style
  - Javascript modules (import/export)
  - React
  - Yes
  - Browser
  - Use a popular style guide
  - Airbnb
  - JSON
  - Yes

- npm i eslint-config-airbnb-typescript --save-dev

- add scripts in package.json

  - "lint": "eslint ."
  - "lint:fix": "eslint --fix ."

- edit eslintrc.json

  - add env for jest
  - edit extends
  - add rules to override rules from plugins,
  - add `"project": "./tsconfig.json" ` to parserOptions

- npm i prettier eslint-config-prettier eslint-plugin-prettier eslint-plugin-prettier eslint-config-prettier --save-dev

- edit eslintrc.json

  - add plugin:prettier/recommended in to extends
  - add prettier to plugins(make sure to add the last in the array)

- create a .prettierrc.json

  - add rules
  - eg: `{
    "tabWidth": 2,
    "useTabs": false,
    "semi": true,
    "singleQuote": false,
    "trailingComma": "none",
    "printWidth": 80
  }`

- npx husky init && npm install

