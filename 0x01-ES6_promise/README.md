# 0x01. ES6 Promises

## Description
This project focuses on understanding and implementing JavaScript Promises, async and await, as well as error handling using try and catch.

## Learning Objectives
- Gain understanding of Promises, their structure, and their usage.
- Learn how to use the `then`, `resolve`, `catch`, and `try` methods.
- Practice working with async functions and the `await` operator.
- Understand error handling with `try` and `catch`.

## Requirements
- Ubuntu 18.04 LTS
- NodeJS 12.11.x
- Editors: `vi`, `vim`, `emacs`, `Visual Studio Code`
- All files should have a trailing newline.
- All files should use the `.js` extension.
- Tests should be conducted using Jest (`npm run test`).
- Code should be verified against ESLint.
- All functions must be exported.

## Setup
### Install NodeJS 12.11.x:
```bash
curl -sL https://deb.nodesource.com/setup_12.x -o nodesource_setup.sh
sudo bash nodesource_setup.sh
sudo apt install nodejs -y
nodejs -v
npm -v
Install Jest, Babel, and ESLint:
bash
Copy code
npm install
Configuration Files:
package.json
babel.config.js
.eslintrc.js
utils.js
Response Data Format
uploadPhoto returns a response in the format:
javascript
Copy code
{
  status: 200,
  body: 'photo-profile-1',
}
createUser returns a response in the format:
javascript
Copy code
{
  firstName: 'Guillaume',
  lastName: 'Salva',
}
Tasks
Keep every promise you make and only make promises you can keep
Prototype: getResponseFromAPI()
Don't make a promise...if you know you can't keep it
Prototype: getFullResponseFromAPI(success)
Catch me if you can!
Prototype: handleResponseFromAPI(promise)
Handle multiple successful promises
Prototype: handleProfileSignup()
Simple promise
Prototype: signUpUser(firstName, lastName)
Reject the promises
Prototype: uploadPhoto(filename)
Handle multiple promises
Prototype: handleProfileSignup(firstName, lastName, fileName)
Load balancer
Prototype: loadBalancer(chinaDownload, USDownload)
Throw error / try catch
Prototype: divideFunction(numerator, denominator)
Throw an error
Prototype: guardrail(mathFunction)
Directory Structure
css
Copy code
css
0x01-ES6_promise/
│
├── 0-main.js
├── 0-promise.js
├── 1-main.js
├── 1-promise.js
├── 2-main.js
├── 2-then.js
├── 3-all.js
├── 3-main.js
├── 4-main.js
├── 4-user-promise.js
├── 5-main.js
├── 5-photo-reject.js
├── 6-final-user.js
├── 6-main.js
├── 7-load_balancer.js
├── 7-main.js
├── 8-try.js
├── 8-main.js
├── 9-try.js
├── 9-main.js
├── package-lock.json
├── package.json
└── utils.js
