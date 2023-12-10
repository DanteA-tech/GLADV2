---
toc: True
comments: False
layout: post
title: Binary-Decimal
description: convert from binary to decimal
type: hacks
courses: {'compsci': {'week': 2}}
---

<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Binary-Decimal Guessing Game</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background-color: #f5f5f5;
      margin: 0;
      padding: 0;
    }

    .container {
      max-width: 600px;
      margin: 20px auto;
      padding: 20px;
      background-color: #fff;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    h1 {
      margin-top: 0;
      font-size: 36px;
      color: #333;
    }

    p {
      font-size: 18px;
      color: #555;
    }

    .carnival-ride {
      width: 300px;
      height: 200px;
      background-color: #222;
      border-radius: 10px;
      margin: 20px auto;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
      position: relative;
      overflow: hidden;
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #fff;
      font-size: 24px;
    }

    .binary-digits {
      display: flex;
      gap: 5px;
    }

    .binary-digit {
      transition: transform 0.5s ease-in-out;
    }

    .carnival-cart {
      width: 30px;
      height: 30px;
      background-color: #f39c12;
      border-radius: 50%;
      position: absolute;
      bottom: -30px;
      left: 50%;
      transform: translateX(-50%);
      transition: bottom 1s ease-in-out;
    }

    input[type="text"],
    button {
      padding: 10px;
      margin: 10px;
      font-size: 16px;
      border: none;
      border-radius: 5px;
      background-color: #f39c12;
      color: white;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Binary Guesseing game</h1>
    <p>Get ready for a binary ride!</p>
    <p>Guess the decimal equivalent of the binary number you see</p>
    <p id="binaryNumber"></p>
    <input type="text" id="guessInput" placeholder="Enter your guess">
    <button onclick="startRide()">Check Guess</button>
    <p id="result"></p>

    <!-- Interactive carnival ride representing binary-to-decimal conversion -->
    <div class="carnival-ride" onclick="startRide()">
      <div class="binary-digits"></div>
      <div class="carnival-cart"></div>
    </div>
  </div>

    <!-- Show Hint button -->
<!-- Hint button -->
<button onclick="showHint()">Show Hint</button>
<div id="hintContent" style="display: none;">
  <!-- Visual Hint content -->
  <!-- Visual Hint content -->
  <p>Hint: Binary to Decimal Conversion</p>
  <p>Imagine a series of switches or lights that can be ON (1) or OFF (0).</p>
  <img src="{{site.baseurl}}/images/Lightbulb.png" alt="Visual representation of binary numbers">
  <p>In binary, each position represents a power of 2, similar to counting in units, tens, hundreds, etc.</p>
  <p>For example, from right to left: 1, 2, 4, 8, 16...</p>
  </div>

  <script>
    let rideStarted = false;
    let binaryToShow = '';

    // Function to generate a random binary number
    function generateRandomBinary() {
      const binaryLength = 8; // Change the length as needed
      let binary = '';
      for (let i = 0; i < binaryLength; i++) {
        const randomBit = Math.floor(Math.random() * 2);
        binary += randomBit;
        binaryToShow += randomBit;
      }
      return binary;
    }

    // Initialize the game
    let randomBinary = generateRandomBinary();
    let binaryNumberElement = document.getElementById('binaryNumber');
    binaryNumberElement.innerText = `Binary Number: ${binaryToShow}`;

    // Display binary digits on the ride
    const binaryDigitsContainer = document.querySelector('.binary-digits');
    randomBinary.split('').forEach((digit) => {
      const digitElement = document.createElement('div');
      digitElement.classList.add('binary-digit');
      digitElement.innerText = digit;
      binaryDigitsContainer.appendChild(digitElement);
    });

    // Function to start the interactive ride animation
    function startRide() {
      if (!rideStarted) {
        rideStarted = true;
        const cart = document.querySelector('.carnival-cart');
        cart.style.bottom = '10px'; // Adjust cart position to simulate movement

        setTimeout(() => {
          cart.style.bottom = 'calc(100% - 30px)';
          document.querySelectorAll('.binary-digit').forEach((digit, index) => {
            setTimeout(() => {
              digit.style.transform = 'scale(0)';
            }, 100 * index);
          });
        }, 10);
      } else {
        checkGuess();
      }
    }

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
        moveCarnivalCart();
        binaryToShow = '';
        randomBinary = generateRandomBinary();
        binaryNumberElement.innerText = `Binary Number: ${binaryToShow}`;
        const binaryDigitsContainer = document.querySelector('.binary-digits');
        binaryDigitsContainer.innerHTML = '';
        randomBinary.split('').forEach((digit) => {
          const digitElement = document.createElement('div');
          digitElement.classList.add('binary-digit');
          digitElement.innerText = digit;
          binaryDigitsContainer.appendChild(digitElement);
        });
      } else {
        document.getElementById('result').innerText = `Sorry, the correct answer is ${decimalEquivalent}. Better luck next time!`;
      }
    }

    // Function to move the carnival cart
    function moveCarnivalCart() {
      const cart = document.querySelector('.carnival-cart');
      cart.style.bottom = '10px';
      setTimeout(() => {
        cart.style.bottom = 'calc(100% - 30px)';
      }, 500);
    }

        // Function to show/hide the hint content
    function showHint() {
      const hintContent = document.getElementById('hintContent');
      hintContent.style.display = hintContent.style.display === 'none' ? 'block' : 'none';
    }
  </script>
</body>
</html>