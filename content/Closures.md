---
title: "Explaining JavaScript scope and closures - Godsgift Akari"
date: 2019-05-14T14:46:10+06:00
description: "JavaScript closure"
type: "post"
image: ""
categories:
  - "JavaScript"
tags:
  - "Web"
  - "Software"
---

## Sample of Closure

```js
// Declare a variabe addValues and assign function to it
let addValues = (function() {
  let counter = 0;
  return function() {
    counter += 1;
    return counter;
  };
})(); //Immediately Invoked

// Call the function
addValues();
addValues();
addValues();
```

The variable addValue is assigned the return value of a immediately invoked function.

The Immediately invoked function only runs once. It sets the counter to zero (0), and returns a function expression.

This way addValue becomes a function. The good thing is that it can get right of entry to the counter in the parent scope.

This is called a JavaScript closure. It makes it viable for a functions to have "private" variables.

The counter is included by means of the scope of the anonymous function, and can solely be modified the use of the addValue function.
