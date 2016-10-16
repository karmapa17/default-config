# Karmapa JavaScript Style Guide
The style guide of Dharma Treasure Organization

## Table of Contents

  1. [Basic](#basic)
  2. [Variables](#variables)
  3. [Objects](#objects)
  4. [Modules](#modules)
  5. [Functions](#functions)
  6. [Blocks](#blocks)

## Basic
Follow [Google JavaScript Style Guide](https://google.github.io/styleguide/javascriptguide.xml)

## Variables

```javascript
// bad, b and c becomes globals
// should've used let or const instead of var
var a = b = c = 10;

// good
// use const for non re-assignment variables
const obj = {};
const arr = [];

// use let for re-assignment variables
let index = 0;
let isActive = false;
```

## Objects

```javascript

// bad
// don't do jQuery style spacing for object literals
const obj = { name: 'karmapa' };

// good
// when only a property in an object, use one liner
const simpleData = {name: 'karmapa'};

// good
// when multiple propteries in an object, use multiple lines
const complexData = {
  name: 'karmapa',
  age: 18,
  lang: 'bo'
};

```
## Modules

```javascript
// good
// same as object literal
import {Modal, Button, Nav} from 'react-bootstrap';

// good
// when a line is about to exceed 120 characters, wrap it
import {Modal, Button, Nav, NavBar, Form, Input, Glyphicons,
  Label, Alert} from 'react-bootstrap';    // notice here's 2 space indent at the second line

// file import starts with a new line after node module import
import {hashPassword, validate} from './../helpers';
import * as home from './../controllers/home';
```

## Functions

```javascript
// bad
// no php naming style here forever and ever
function do_something() {
}

// bad
// no c style here
function doSomething()
{
}

// bad
// no space after argument block
function doSomething () {
}

// good
// function name should be named in camelcase
function doSomething() {
}

// good
const add = (first, second) => first + second;

// good
// always have argument parentheses
// when a function is not too simple, wrap it whenever needed
const doIt = (arg) => {
  // lots stuff here
};
```

## blocks
```javascript
// bad
if (dreamComesTrue) {
  doThing1();
  doThing2();
} else {
  doThing3();
}

// good
// better readability to wrap else block
if (dreamComesTrue) {
  doThing1();
  doThing2();
}
else if (anotherDreamComesTrue) {
  doThing3();
}
else {
  doThing4();
}
```
