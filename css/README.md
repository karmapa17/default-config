# Karmapa CSS / Sass Style Guide
The CSS / Sass style guide of Dharma Treasure Organization

## Table of Contents

  1. [Basic](#basic)
  2. [Selectors](#selectors)
  
## Basic
 - Follow [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.xml#CSS_Style_Rules)
  
## Selectors

```css
/* bad */
/* should place one selector at a line and add a space before open brace to enhance readability */
a, p, div{
 font-size: 20px; 
}

/* good */
a,
p,
div {
  font-size: 20px;
}

/* bad */
a { font-size: 20px; padding: 10px; display: block; }

/* good */
a {
  font-size: 20px;
  padding: 10px;
  display: block;
}
```
