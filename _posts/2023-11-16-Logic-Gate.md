---
comments: True
layout: post
title: Logic Gate
type: plan
toc: True
courses: { compsci: {week: 14} }
---
%%js
// Binary to Decimal
function binaryToDecimal(binary) {
  return parseInt(binary, 2);
}

// Decimal to Binary
function decimalToBinary(decimal) {
  return (decimal >>> 0).toString(2); // Using bit-wise operator to convert
}

// Example usage:
const binaryNumber = '1010';
const decimalNumber = 15;

console.log(binaryToDecimal(binaryNumber)); // Output: 10
console.log(decimalToBinary(decimalNumber)); // Output: 1111
