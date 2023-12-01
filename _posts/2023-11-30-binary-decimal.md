---
toc: True
comments: False
layout: post
title: Binary-Decimal
description: convert from binary to decimal
type: hacks
courses: {'compsci': {'week': 2}}
---

# Binary to Decimal Converter Game

Guess the decimal equivalent of the following binary number:

<div id="binaryNumber"></div>

<input type="text" id="guessInput" placeholder="Enter your guess">
<button onclick="checkGuess()">Check Guess</button>
<p id="result"></p>

<script>
  // Function to generate a random binary number
  function generateRandomBinary() {
    const binaryLength = 8; // Change the length as needed
    let binary = '';
    for (let i = 0; i < binaryLength; i++) {
      binary += Math.floor(Math.random() * 2);
    }
    return binary;
  }

  // Initialize the game
  const randomBinary = generateRandomBinary();
  document.getElementById('binaryNumber').innerText = `Binary Number: ${randomBinary}`;

  // Function to check the user's guess
  function checkGuess() {
    const userGuess = document.getElementById('guessInput').value;

    if (!/^\d+$/.test(userGuess)) {
      document.getElementById('result').innerText = 'Please enter a valid integer guess.';
      return;
    }

    const decimalEquivalent = parseInt(randomBinary, 2);
    if (parseInt(userGuess) === decimalEquivalent) {
      document.getElementById('result').innerText = 'Congratulations! Your guess is correct.';
    } else {
      document.getElementById('result').innerText = `Sorry, the correct answer is ${decimalEquivalent}. Better luck next time!`;
    }
  }
</script>