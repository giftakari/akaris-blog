---
title: "JavaScript Promises, Async -Godsgift Akari "
date: 2019-09-14T14:46:10+06:00
description: "JavaScript Promises, Async functions"
type: "post"
image: ""
categories:
  - "JavaScript"
tags:
  - "Web"
  - "Software"
---

## JavaScript Promises, Asycn Function

JavaScript is single threaded, what means is that JavaScript executes the code we write line my line . Javascript depends on Callback functions, Promises and the use of Async and Await to handle deferred operations in JavaScript.

### Examples of Deferred operations

```js
setInterval(function() {
  console.log("hello World!");
}, 3000);

console.log(`I'll run first`);

/*
"i'll run first "
"hello World!"
"Welcome giftakari"
*/
```

The setInterval function is should have been called before the last **"i'll run first"**. We execution was delayed for 3 seconds then JavaScript called the last console.log before calling the setInterval function.
