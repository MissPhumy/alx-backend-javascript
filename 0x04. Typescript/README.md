# 0x04. TypeScript


## Resources
**Read or watch**:
- [TypeScript in 5 minutes](https://alx-intranet.hbtn.io/rltoken/waTSa9Mguj912pel9On57w "TypeScript in 5 minutes")
- [TypeScript documentation](https://alx-intranet.hbtn.io/rltoken/iPO8DlHCGzc1jnojLoP9HA "TypeScript documentation")

## Learning Objectives
- Basic types in Typescript
- Interfaces, Classes, and functions
- How to work with the DOM and Typescript
- Generic types
- How to use namespaces
- How to merge declarations
- How to use an ambient Namespace to import an external library
- Basic nominal typing with Typescript

## Requirements
- Allowed editors: `vi`, `vim`, `emacs`, `Visual Studio Code`
- All files should end with a new line
- All files will be transpiled on Ubuntu 18.04
- TS scripts checked with `jest` (version 24.9.* )
- A `README.md` file at the root of the folder is mandatory
- Use the `ts` extension when possible
- No compiler warnings or errors

## Configuration Files

### `package.json`
```json
{
  "name": "typescript_dependencies",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "start-dev": "webpack-dev-server --open",
    "build": "webpack",
    "test": "jest"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "@babel/plugin-proposal-export-default-from": "^7.5.2",
    "@babel/preset-typescript": "^7.7.2",
    "@types/jest": "^24.0.23",
    "@typescript-eslint/eslint-plugin": "^2.4.0",
    "@typescript-eslint/parser": "^2.4.0",
    "clean-webpack-plugin": "^3.0.0",
    "fork-ts-checker-webpack-plugin": "^1.5.1",
    "html-webpack-plugin": "^3.2.0",
    "jest": "^24.9.0",
    "source-map": "^0.7.3",
    "ts-jest": "^
json
Copy code
24.0.2",
    "typescript": "^3.7.2",
    "webpack": "^4.41.2",
    "webpack-cli": "^3.3.10",
    "webpack-dev-server": "^3.9.0",
    "webpack-merge": "^4.2.2"
  }
}
tsconfig.json
json
Copy code
{
  "compilerOptions": {
    "target": "es5",
    "module": "commonjs",
    "strict": true,
    "esModuleInterop": true,
    "skipLibCheck": true,
    "forceConsistentCasingInFileNames": true
  }
}
webpack.config.js
js
Copy code
const path = require('path');
const HtmlWebpackPlugin = require('html-webpack-plugin');
const { CleanWebpackPlugin } = require('clean-webpack-plugin');
const ForkTsCheckerWebpackPlugin = require('fork-ts-checker-webpack-plugin');

module.exports = {
  entry: './src/index.ts',
  devtool: 'inline-source-map',
  module: {
    rules: [
      {
        test: /\.ts$/,
        use: 'ts-loader',
        exclude: /node_modules/
      }
    ]
  },
  resolve: {
    extensions: ['.ts', '.js']
  },
  output: {
    filename: 'bundle.js',
    path: path.resolve(__dirname, 'dist')
  },
  plugins: [
    new CleanWebpackPlugin(),
    new HtmlWebpackPlugin({
      template: './src/index.html'
    }),
    new ForkTsCheckerWebpackPlugin()
  ],
  devServer: {
    contentBase: './dist'
  }
};
Tasks
0. Basic types
File: task_0/main.ts

Write a function printUserInfo that takes in firstName, lastName, and age as arguments and returns a formatted string.

1. Interfaces
File: task_1/main.ts

Create an interface User with firstName, lastName, and age properties. Write a function printUser that takes a User object as an argument.

2. Classes
File: task_2/main.ts

Define a class User with a constructor that takes firstName, lastName, and age. Implement a method getFullName that returns the user's full name.

3. Functions
File: task_3/main.ts

Write a generic function identity that returns the argument passed to it.

4. Working with the DOM
File: task_4/main.ts

Use TypeScript to manipulate the DOM by creating an element and appending it to the body.

5. Generic types
File: task_5/main.ts

Write a generic class Stack with methods push, pop, and peek.

6. Namespaces
File: task_6/main.ts

Create a namespace Utils with a function add and another namespace MathUtils with a function multiply.

7. Merging declarations
File: task_7/main.ts

Merge two declarations of an interface Point with properties x, y, and a method translate.

8. Using an ambient Namespace to import an external library
File: task_8/main.ts

Use the moment library to manipulate dates. Import the library using an ambient namespace.

9. Basic nominal typing in TypeScript
File: task_9/main.ts

Implement nominal typing using branded types to ensure type safety.

