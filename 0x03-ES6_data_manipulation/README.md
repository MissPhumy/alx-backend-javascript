# 0x03. ES6 data manipulation

### Resources
    • Array
    • Typed Array
    • Set Data Structure
    • Map Data Structure
    • WeakMap
### Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

### Requirements
Ubuntu 18.04 LTS using NodeJS 12.11.x
Editors: vi, vim, emacs, Visual Studio Code

### Tests
Jest and the command npm run test
ESLint

### Setup
NodeJS 12.11.x
Jest, Babel, and ESLint

### Configuration files
package.json
babel.config.js
.eslintrc.js

## Tasks
0. Basic list of objects
Create a function named getListStudents that returns an array of objects.
Each object should have three attributes: id (Number), firstName (String), and location (String).

1. More mapping
Create a function getListStudentIds that returns an array of ids from a list of object.

2. Filter
Create a function getStudentsByLocation that returns an array of objects who are located in a specific city.
  
3. Reduce
Create a function getStudentIdsSum that returns the sum of all the student ids.
  
4. Combine
Create a function updateStudentGradeByCity that returns an array of students for a specific city with their new grade.
  
5. Typed Arrays

Create a function named createInt8TypedArray that returns a new ArrayBuffer with an Int8 value at a specific position.

6. Set data structure
Create a function named setFromArray that returns a Set from an array.

7. More set data structure
Create a function named hasValuesFromArray that returns a boolean if all the elements in the array exist within the set.

8. Clean set
Create a function named cleanSet that returns a string of all the set values that start with a specific string (startString).

9. Map data structure
Create a function named groceriesList that returns a map of groceries with the following items (name, quantity):

10. More map data structure
Create a function named update UniqueItems that returns an updated map for all items with initial quantity at 1.

11. Weak link data structure
Export a constinstance of WeakMap and name it weakMap. Export a new function named queryAPI.
