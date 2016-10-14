# Karmapa JavaScript Style Guide
The style guide of Dharma Treasure Organization

## Table of Contents

  1. [Objects](#objects)

## Objects

```javascript

// bad
// don't do jQuery style spacing for object literals
const obj = { name: 'karmapa' };

// good
// when only a property in an object, use one liner
const simpleData = {name: 'karmapa'};

// when multiple propteries in an object, use multiple lines
const complexData = {
  name: 'karmapa',
  age: 18,
  lang: 'bo'
};

```

