---
title: "Article 2 – FizzBuzz"
draft: false
---

# Problem Summary
This article covers the classic “FizzBuzz” exercise.  
The goal is simple: print the numbers from 1 to 100, but replace certain numbers with words.

- Numbers divisible by **3** → “Fizz”
- Numbers divisible by **5** → “Buzz”
- Numbers divisible by **both** → “FizzBuzz”

# How I Approached It
I knew I needed a basic loop that runs from 1 to 100.  
Inside the loop, I checked the special cases first (like numbers divisible by both 3 and 5), because those need to be caught before the single checks. After that, it’s just simple `if` statements.

The main idea was:  
**check the biggest condition first, then work your way down.**

# Key Code Snippet

```js
for (let i = 1; i <= 100; i++) {
  if (i % 15 === 0) {
    console.log("FizzBuzz");
  } else if (i % 3 === 0) {
    console.log("Fizz");
  } else if (i % 5 === 0) {
    console.log("Buzz");
  } else {
    console.log(i);
  }
}
