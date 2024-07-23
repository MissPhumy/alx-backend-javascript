# 0x05. NodeJS Basics

## Resources
- [Node JS getting started](https://nodejs.org/en/docs/guides/getting-started-guide/)
- [Process API doc](https://nodejs.org/dist/latest-v14.x/docs/api/process.html)
- [Child process](https://nodejs.org/dist/latest-v14.x/docs/api/child_process.html)
- [Express getting started](https://expressjs.com/en/starter/installing.html)
- [Mocha documentation](https://mochajs.org/)
- [Nodemon documentation](https://nodemon.io/)

## Learning Objectives
By the end of this project, you should be able to explain the following without needing to refer to Google:
- Run JavaScript using NodeJS
- Use NodeJS modules
- Use specific NodeJS modules to read files
- Use `process` to access command line arguments and the environment
- Create a small HTTP server using NodeJS
- Create a small HTTP server using ExpressJS
- Create advanced routes with ExpressJS
- Use ES6 with NodeJS using Babel-node
- Use Nodemon to develop faster

## Requirements
- Allowed editors: `vi`, `vim`, `emacs`, `Visual Studio Code`
- All your files will be interpreted/compiled on Ubuntu 18.04 LTS using Node.js (version 12.x.x)
- All your files should end with a new line
- A `README.md` file, at the root of the folder of the project, is mandatory
- Your code should use the `.js` extension
- Your code will be tested using Jest and the command `npm run test`
- Your code will be verified against lint using ESLint
- Your code needs to pass all the tests and lint. You can verify the entire project by running `npm run full-test`
- All of your functions/classes must be exported using this format: `module.exports = myFunction;`

## Provided files

### database.csv

firstname,lastname,age,field
Johann,Kerbrou,30,CS
Guillaume,Salou,30,SWE
Arielle,Salou,20,CS
Jonathan,Benou,30,CS
Emmanuel,Turlou,40,CS
Guillaume,Plessous,35,CS
Joseph,Crisou,34,SWE
Paul,Schneider,60,SWE
Tommy,Schoul,32,SWE
Katie,Shirou,21,CS

## Project Configuration

### package.json

json
`{
  "name": "nodejs-basics",
  "version": "1.0.0",
  "description": "NodeJS Basics Project",
  "main": "index.js",
  "scripts": {
    "test": "jest",
    "full-test": "npm run lint && npm run test",
    "lint": "eslint ."
  },
  "author": "",
  "license": "ISC",
  "dependencies": {
    "express": "^4.17.1",
    "nodemon": "^2.0.7"
  },
  "devDependencies": {
    "babel-jest": "^26.6.3",
    "babel-preset-env": "^1.7.0",
    "eslint": "^7.14.0",
    "jest": "^26.6.3"
  }
}`

## babel.config.js

js
`module.exports = {
  presets: [
    ['@babel/preset-env', { targets: { node: 'current' } }]
  ]
};`

.eslintrc.js
js
`module.exports = {
  env: {
    browser: true,
    commonjs: true,
    es6: true,
    node: true,
    jest: true
  },
  extends: 'eslint:recommended',
  parserOptions: {
    ecmaVersion: 2018
  },
  rules: {
    'no-console': 'off',
    'indent': ['error', 2],
    'linebreak-style': ['error', 'unix'],
    'quotes': ['error', 'single'],
    'semi': ['error', 'always']
  }
};`
# Getting Started

1. Clone the repository.
2. Run `$ npm install` to install all dependencies.

## Running the Tests

Run `npm run test` to execute the tests.

## Linting

Run `npm run lint` to check the code for linting errors.

## Full Test

Run `npm run full-test` to run both linting and tests.

## Note

Don't forget to run `$ npm install` when you have the `package.json` file.
