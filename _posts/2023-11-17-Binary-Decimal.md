---
comments: True
layout: post
title: Binary
type: plan
toc: True
courses: { compsci: {week: 1} }
---

/**
 * Convert a binary number to its decimal equivalent.
 * @param {string} binary - Binary number represented as a string.
 * @returns {number} - Decimal representation of the binary number.
 * @throws {Error} - Throws an error for an invalid binary number.
 */
function binaryToDecimal(binary) {
  if (!/^[01]+$/.test(binary)) {
    throw new Error('Invalid binary number. Please provide a valid binary string.');
  }
  return parseInt(binary, 2);
}

/**
 * Convert a decimal number to its binary equivalent.
 * @param {number} decimal - Decimal number.
 * @returns {string} - Binary representation of the decimal number.
 * @throws {Error} - Throws an error for an invalid decimal number.
 */
function decimalToBinary(decimal) {
  if (isNaN(decimal) || decimal < 0 || Math.floor(decimal) !== decimal) {
    throw new Error('Invalid decimal number. Please provide a non-negative integer.');
  }
  return decimal.toString(2);
}

// Example usage:
const binaryNumber = '1010';  // This is a string representation of a binary number.
const decimalNumber = 15;

try {
  const convertedToDecimal = binaryToDecimal(binaryNumber);
  console.log(`Binary ${binaryNumber} is equivalent to Decimal: ${convertedToDecimal}`);
} catch (error) {
  console.error(error.message);
}

try {
  const convertedToBinary = decimalToBinary(decimalNumber);
  console.log(`Decimal ${decimalNumber} is equivalent to Binary: ${convertedToBinary}`);
} catch (error) {
  console.error(error.message);
}