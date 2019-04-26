# ES6 (EcmaScript 6)

## Table of Contents
* [Destructuring](#destructuring)
* [Classes](#classes)
* [Functions](#functions)
  - Arrow Functions
* [Modules](#modules)
  - Exports
  - Imports
* [Operators](#operators)
  - Spread & Rest Operators
* [Variables](#variables)
  - `let`
  - `const`

---

## Destructuring
* **Destructuring**: extract array elements or object properties and store them in variables

```
# array destructuring
[ a, b ] = ["Hello", "Tea"];
console.log(a)              # output "Hello"
console.log(b)              # output "Tea"

# object destructuring
{ name } = { name: "Tea", greet: "Hi there" }
console.log(name)           # output "Tea"
console.log(greet)          # output undefined
```

---

## Classes
`Class` have:
* properties
* methods

```
class Human {
  constructor() {
    this.gender = "female"
  }
}

class Person extends Human {
  constructor() {
    super()
    this.name = "Tea"
  }

  thisMethod() {
    // do something
  }
}
```

---

## Functions

### Arrow Functions
* removes issues with `this` keyword
* `this` keyword is implicitly added to arrow function

```
# arrow function

const foo = () => {
  // do something
}

const foo = (arg1, arg2) => {
  // do something
}

# syntax below only works for ONE argument
const foo = arg1 => {
  // do something
}

# syntax below one-liner arrow function with ONE argument with one return (omit)
const foo = arg1 => "hello" + arg1;
```

Arrow Function is equivalent to function declaration:

```
# function declaration
function foo() {
  // do something
}
```

---

## Modules

Let's assume you have a `utility.js`:
* named export with names in { }

```
# utility.js
export const greet = () => { ... }
```

### Export
* `default` keyword => exports name of const or function

```
# person.js
const person = {
  name: "Tea"
}

export default person
```


### Import

```
# app.js
import person from './person.js'        # imports default file

import { greet } from './utility.js'    # imports specific const from utility.js

import * as bundled from './utility.js' # imports everything from utility.js and name everything as "bundled"
```

---

## Operators


### Spread & Rest Operators
**Spread Operator**: used to split an array of elements OR object properties

```
const oldArray = [ 4, 5 ]
const oldObject = {
  oldObject: 1
}

# spread operator use below
const newArray = [ ...oldArray, 1, 2 ]
const newObject = {
  ...oldObject,
  newProp: 5;
}
```

**Rest Operator**: used to merge a list of function arguments into an array

```
function sortArgs(...args) {
  return args.sort();
}
```

---

## Variables
* `var` is no longer used. Use these new variables instead:
  - `let`
  - `const`
