---
toc: False
comments: True
layout: notebook
title: Binary CPT Project Review Ticket 2
description: Binary CPT Project Review Ticket
type: tangibles
courses: {'compsci': {'week': 3}}
---

# Team

| Crossover Score | Runtime | Plans | Github | Analytics |
|-----------------|---------|-------|--------|-----------|
| 0.88/0.9 | [Color Conversions](https://dantea-tech.github.io/GLAD//2023/11/15/txtcol.html), [ASCII image generator](https://dantea-tech.github.io/GLAD//2023/11/27/Ascii.html), [RGB adjuster on image](https://dantea-tech.github.io/GLAD//2023/11/16/Binary.html), [Binary Guessing Game](https://dantea-tech.github.io/GLAD//2023/11/30/binary-decimal.html) | [Binary Guessing Game](https://dantea-tech.github.io/GLAD//2023/11/30/binary-decimal.html) | [Issues](https://github.com/DanteA-tech/GLAD/issues/3) | [Team Commits](https://github.com/DanteA-tech/GLAD/commits/main/) |

# Individuals

| Name | Team+Indi+Teacher | Runtime | Issues | Key Commit(s) | Analytics |
|------|-------------------|---------|--------|---------------|-----------|
| Lincoln C | 0.8+0.88+?=1.68 | [Binary Guessing Game](https://dantea-tech.github.io/GLAD//2023/11/30/binary-decimal.html) | [Issues](https://github.com/DanteA-tech/GLAD/issues/3) | [Binary-Decimal functioning](https://github.com/DanteA-tech/GLAD/commit/f6c9b0fe00a2240360085efe65be4843e69c9c3e) | [Commits](https://github.com/DanteA-tech/GLAD/commits/main/?after=21f4df088260dd7ecc55b0e036e5d8c2a183d4de+34), [Profile](https://github.com/LincolnC2008) |

| Name | Team+Indi+Teacher | Runtime | Issues | Key Commit | Key Commit | Analytics |
|------|-------------------|---------|--------|------------|------------|-----------|
| Dante A | 0.87+0.88+?=1.75 | [RGB adjuster on image](https://dantea-tech.github.io/GLAD//2023/11/16/Binary.html) | [Issues](https://github.com/DanteA-tech/GLAD/issues/6) | [Binary and Hex values](https://github.com/DanteA-tech/GLAD/commit/bd153610a994c4ca94f725edf70a8bce31ca4bb8) | [Scaling and revert](https://github.com/DanteA-tech/GLAD/actions/runs/7144912127) | [Commits](https://github.com/DanteA-tech/GLAD/graphs/contributors), [Profile](https://github.com/DanteA-tech) |

| Name | Team+Indi+Teacher | Runtime | Issues | Key Commit(s) | Plans | Analytics |
|------|-------------------|---------|--------|---------------|-------|-----------|
| Ashwin V | 0.85+0.88+?=1.73 | [ASCII image generator](https://dantea-tech.github.io/GLAD//2023/11/27/Ascii.html) | [Issues](https://github.com/DanteA-tech/GLAD/issues/5) | [Adding first version](https://github.com/DanteA-tech/GLAD/commit/12196e52424d34337deed44d0588905c28ea3179), [Adding color feature](https://github.com/DanteA-tech/GLAD/commit/be4830dafa66b1b005caa8a6f7706fd0f48f92d9) | [Plans](https://dantea-tech.github.io/GLAD//2023/11/29/Ashwin_Plans.html) | [Commits](https://github.com/DanteA-tech/GLAD/graphs/contributors), [Profile](https://github.com/Ashwinv93) |

| Name | Team+Indi+Teacher | Runtime | Issues | Key Commit(s) | Analytics |
|------|-------------------|---------|--------|---------------|-----------|
| Gurshawn B | 0.82+0.87+?=1.70 | [Color Conversions](https://dantea-tech.github.io/GLAD//2023/11/15/txtcol.html) | [Issues](https://github.com/DanteA-tech/GLAD/issues/2) | [Key Commit](https://github.com/DanteA-tech/GLAD/commit594f9963fdafb0c1da5ec53c38ffc99ed43997c1) | [Analytics](https://github.com/DanteA-tech/GLAD/graphs/contributors), [Profile](https://github.com/Gurbop) |


## Lincoln- Binary to Decimal Converter Game
What Lincoln did: After we met for our live review, I realized that I had a good idea going and it was fully functional vut I needed some sort of way for the audience to learn what a binary numbereven is so I added a hint button which would also qualify as my key commit.

1. Interactive Binary Game:
- Purpose: Engaging users in guessing decimal equivalents of binary numbers showcases the practical application of binary logic in a playful and interactive manner.
- Value: Offers users a hands-on experience to reinforce their understanding of binary-to-decimal conversion, a fundamental concept in computer science.

2. Visual and Explanatory Hint Button:
- Purpose: The "Hint" button provides visual aids and explanatory text, aiding users in comprehending the conversion process, thereby emphasizing the educational value of the project.
- Value: Illustrates binary logic by providing additional educational support, aligning with the project's intent to assist users in grasping the underlying concepts.

3. Meeting CPT Requirements:
- User Engagement: The interactive game engages users in actively participating, contributing to the user-centered design aspect.
- Educational Support: The provision of hints aligns with the educational component outlined in CPT requirements, ensuring users receive guidance for understanding binary logic.
- Functional Demonstration: The code functions as intended, demonstrating the conversion process, meeting the requirement for demonstrating functionality related to binary-to-decimal conversion.

4. HTML Structure: The HTML file sets up the structure of the game, providing elements for displaying the binary number, input field for guesses, buttons, and containers for visual elements.

5. JavaScript Logic:
- Random Binary Generation: The generateRandomBinary() function generates a random 8-bit binary number.
- Display Binary: It displays the generated binary number as both text and visually in the form of binary digits.
- Starting the Game: When the user clicks on the "Check Guess" button or the game area, it initiates the startRide() function.
Game Logic:
- If the game hasn't started (rideStarted = false) Once the animation completes or if the game has started, it checks the user's guess using the checkGuess() function.
- It validates the user input and compares it against the decimal equivalent of the randomly generated binary.
- If the guess is correct, it triggers a success message, updates the score (if implemented), animates the carnival cart, generates a new binary number, and resets the game for the next round.
- If the guess is incorrect, it provides the correct answer and prompts the user to try again.

6. Hint Functionality: 
- The "Hint" button, when clicked, reveals an explanatory hint regarding binary-to-decimal conversion, utilizing both textual and visual aids to assist users in understanding the conversion process.
- User Interaction: Users engage by inputting decimal guesses, receiving immediate feedback on correctness, and having access to educational hints to aid in comprehension.
[Lincoln's Video](https://clipchamp.com/watch/3dAmSQNwGxM)
[Lincoln Tangibles](https://dantea-tech.github.io/GLAD//2023/11/30/binary-decimal.html)
## Ashwin - ASCII image generator
What I did: After the week two review, the feedback I got from Mr. Mort and Sergi was to add some info about ascii and to explain to the user what exactly my feature is. I added a description about ascii at the top, and I also implemented a feature which allows you to add color to the image. This is controled by a toggle switch so the user can decide what they want. My feature is educational as it lets a user change any image they want into ascii characters, and do some modifications to them.

### Color to Ascii image
I added a feature that would allow you to click a button that will change the font colors of the ascii characters in to the colors of the original image. This was does by calculating the rgb values of each pixel, along with the brightness. I used Html canvas, which lets me paint out the picture using JS, and anylize the pixels, to do the calculations for rgb and brightness.

### What I could have done if I had more time
If I had more time I could have been able to perfect the image hight and width sliders, because right now, they are a bit buggy if not used correctly. Other than that I acomplished much more that what was in my plans. The initial idea was to just have a ascii image generate from a user imputed image, but I went above that and added features like the dimention sliders, and adding color to the image.

### Key Commits 
-  [Adding Color](https://github.com/DanteA-tech/GLAD/commit/be4830dafa66b1b005caa8a6f7706fd0f48f92d9)
- [Initial Ascii](https://github.com/DanteA-tech/GLAD/commit/12196e52424d34337deed44d0588905c28ea3179)

### Links
- [Ashwins Video](https://youtu.be/87nsno-dlis)

- [Ashwins Tangibles](https://dantea-tech.github.io/GLAD//2023/11/27/Ascii.html)

## Dante A - RGB adjuster
## What I added
## Revert to original
- After our group met with Mr Mort he discussed with me that the ability to change the RGB of the photo is cool, but there should be a way to reset teh image back to normal. I originally thought of maybe adding a marker on where the image's values started but ultimately decided on adding a simple button titled reset image colors. When the user first enters in the image the initial values are stored the button simply calls for those original values and implements them onto the photo.
## Scaling of photo
- After Sergi graded our group's work, one of his suggestions was that the image should be scaled to fix the window since it is annoying to have to move up and down. To my best ability,attempted to scale the image down so that it only takes up 80 percent of the length and width. Looking back I probably couldve made it smaller since teh image is still pretty big.
## Adding the binary and hex values to color wheel
- One of Mr morts main points was that the code has to be able to teach teh reader something about binary. I think my code helps the learner see how binary is used in colors which could be seen by the sliders. However, the color wheels I had were the most visual, but they had no information attached to them. I initially tried to make it so the user's click appears on the color wheel, but I was unable to do it. So I finished by just displaying the binary and hex values of where the user last clicked alongside the wheel.

## Retrospective, What I could've done looking back
Looking back on my actual code, I think my code would've extremely benefited if I got the color wheel indicator to work. This is because it would've served as a great visual example regarding the rgb color wheel. Also, another thing I can improve on in the future are my communication skills with my team. We could've checked in more frequently during class and through text messages. Lastly, we could've increased out usage of plans since it would help us be more up to date and see how much progress everyone has done, helping us start conversations in our checkups.

## Key commits
I had two main key commits, the commit for the scaling of teh image and the commit for the binary and hex.
[Scaling and revert](https://github.com/DanteA-tech/GLAD/actions/runs/7144912127)

[Binary and hex values](https://github.com/DanteA-tech/GLAD/commit/bd153610a994c4ca94f725edf70a8bce31ca4bb8)
[Dante's Video](https://www.capcut.com/s/CV_CJGpsQqO5W8gr/)
[Dante's tangibles](https://dantea-tech.github.io/GLAD//2023/11/16/Binary.html)
## Gurshawn - Text to Color
Functions added since last review:
- Decrypt: After our review with Mr. M, one of the features he recommended to add was a way to convert the image back to text.
- Show correlation with binary: When the image is uploaded a binary representation is outputed to help the user understand the different ways binary can be used by a computer.
- textToBinary(text): This function takes a string input (text), converts each character to its Unicode code point, and then converts those code points to an 8-bit binary representation. It returns the concatenated binary string.
- binaryToRGB(binary): Given a binary string (binary), this function parses it into sets of three 8-bit segments, which represent the red, green, and blue color values. It returns an array of RGB values excluding the color black.
- displayColor(rgbValues): This function takes an array of RGB values (rgbValues) and displays them as a series of colored blocks in a canvas element.
- convertText(): This function is triggered by the "Convert Text" button. It reads the text input, converts it to binary using textToBinary(), then converts that binary string to RGB values using
- binaryToRGB(), and finally displays the colors using displayColor().
- downloadImage(): This function is triggered by the "Download Image" button. It creates a data URL from the canvas containing the colored blocks and allows the user to download the canvas as an image.
convert
- ImageToBinary(event): When an image is uploaded using the "Upload Image" button, this function converts the image to binary data. It reads the image file using FileReader, extracts the pixel data, converts each non-black pixel's RGB values to binary, and displays the resulting binary in the text input field.
- convertImageToText(): When the "Convert Image to Text" button is pressed, this function takes the binary data from the text input field, converts it back to RGB values, and reconstructs the text from the RGB values. It removes duplicate color occurrences and displays the resulting text in the textOutput field.
## Retrospective
If I had more time I would add more SASS to the page and show more of the steps between each coversion the code runs while converting.

- [Gurshawn's Video](https://drive.google.com/drive/folders/1mk7B4i8eP-g4oUBEnsxQPUEfNo-OFVW-)
- [Gurshawn's Key Commit](https://github.com/DanteA-tech/GLAD/commit594f9963fdafb0c1da5ec53c38ffc99ed43997c1)
- [Gurshawn's Tangibles](https://dantea-tech.github.io/GLAD//2023/11/15/txtcol.html) 