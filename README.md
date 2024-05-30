# ES6 Classes Project

This project consists of implementing various classes and understanding the concepts of ES6 classes in JavaScript.

## Learning Objectives

By completing this project, you will be able to:

- Define a Class in JavaScript
- Add methods to a class
- Implement and utilize static methods within a class
- Extend a class from another
- Understand metaprogramming and symbols in JavaScript

## Requirements

- All files should be executed on Ubuntu 18.04 LTS using NodeJS 12.11.x
- Allowed editors: vi, vim, emacs, Visual Studio Code
- All files should end with a new line
- A `README.md` file, at the root of the project folder, is mandatory
- Code files should use the `.js` extension
- Code will be tested using Jest and linted using ESLint
- Setup:
  - Install NodeJS 12.11.x
  - Install Jest, Babel, and ESLint in your project directory using the supplied `package.json`

## Tasks Overview

### 0. You used to attend a place like this at some point
- Implement a class named `ClassRoom` with a constructor attribute `maxStudentsSize`.

### 1. Let's make some classrooms
- Import the `ClassRoom` class and implement a function to initialize multiple classrooms.

### 2. A Course, Getters, and Setters
- Implement a class named `HolbertonCourse` with constructor attributes and getter/setter methods.

### 3. Methods, static methods, computed methods names..... MONEY
- Implement a class named `Currency` with constructor attributes and a method to display currency.

### 4. Pricing
- Implement a class named `Pricing` with constructor attributes and methods to display price and convert price.

### 5. A Building
- Implement an abstract class named `Building` with a getter and ensure subclasses implement a specific method.

### 6. Inheritance
- Implement a subclass named `SkyHighBuilding` that extends `Building` and overrides a method.

### 7. Airport
- Implement a class named `Airport` with constructor attributes and a custom `toString()` method.

### 8. Primitive - Holberton Class
- Implement a class named `HolbertonClass` with constructor attributes and behaviors when cast into different types.

### 9. Hoisting
- Fix provided code and make it work as expected.

### 10. Vroom
- Implement a class named `Car` with constructor attributes and a method to clone the object.

## Project Structure

- Directory: `0x02-ES6_classes`
- Code Files: `0-classroom.js`, `1-make_classrooms.js`, `2-hbtn_course.js`, `3-currency.js`, `4-pricing.js`, `5-building.js`, `6-sky_high.js`, `7-airport.js`, `8-hbtn_class.js`, `9-hoisting.js`, `10-car.js`
- Test Files: `0-classroom.test.js`, `1-make_classrooms.test.js`, `2-hbtn_course.test.js`, `3-currency.test.js`, `4-pricing.test.js`, `5-building.test.js`, `6-sky_high.test.js`, `7-airport.test.js`, `8-hbtn_class.test.js`, `9-hoisting.test.js`, `10-car.test.js`
- Configuration Files: `package.json`, `babel.config.js`, `.eslintrc.js`

