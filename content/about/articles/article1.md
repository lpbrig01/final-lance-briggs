---
title: "Article 1 – Reversing an Array"
draft: false
---

# Problem Summary
This article explains how I solved the “Reversing an Array” exercise from Eloquent JavaScript.  
In my own words, the problem is basically asking me to write two functions:

1. One that **creates a new reversed array**  
2. One that **reverses an array in place** without making a new one

# How I Approached It
For the first part, I knew I just needed to loop through the array from the last index back to the beginning and push each value into a new array. This one is pretty straightforward because you're not changing the original.

The second part (reversing the array in place) made me think a little more. I realized I had to swap the elements from the front and back, moving toward the center. Once the pointers meet in the middle, everything is reversed. No extra array needed.

# Key Code Snippet

```js
function reverseArray(array) {
  let result = [];
  for (let i = array.length - 1; i >= 0; i--) {
    result.push(array[i]);
  }
  return result;
}
