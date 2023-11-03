---
author: alexjmackey
type: normal
category: must-know
tags:
  - introduction
practiceQuestion:
  formats:
    - fill-in-the-gap
  context: standalone
revisionQuestion:
  formats:
    - fill-in-the-gap
  context: standalone
---

# Dynamic Typing


---

## Content


Unlike some other languages, you do not need to tell JavaScript what type a variable is when declaring it:

```javascript
// because we assign a string
let name = "john smith";

// JavaScript knows it's a string
typeof name; // "string"
```

Javascript's typing is dynamic which means you can also change a variable's type at any time:

```javascript
let name = "john smith";

// change string to number
name = 5;
typeof name; // "number"
```


---

## Practice

Which one of the following is **not** a primitive type:

???

- RegExp
- symbol
- string
- number


---

## Revision

Can you change a variable's type in JavaScript?

???

- yes
- no
- only if you declare it again
