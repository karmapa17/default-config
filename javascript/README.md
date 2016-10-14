# Karmapa JavaScript Style Guide
The style guide of Dharma Treasure Organization

## Table of Contents

  1. [Basic](#basic)
  2. [Objects](#objects)
  3. [Modules](#modules)
  4. [Functions](#functions)

## Basic
Follow [Google JavaScript Style Guide](https://google.github.io/styleguide/javascriptguide.xml)

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
