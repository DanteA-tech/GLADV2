---
comments: True
layout: post
title: CPT PLan
type: plan
toc: True
courses: { compsci: {week: 1} }
---
## Goal
Integrate Binary and SASS into a practice project to prepare for our passion projct.
## Elements
Binary - convert RGB color codes to binary 
Color Code - convert messages into binary which will be converted into color.
Logic Gates- interactive place where buttons are pressed to show what gates do based on true/false values if a light turns off and on
Math In Binary-  Binary/Decimal calculator that shows the steps between conversion including left/right shiftss if specified

1. Convert RGB Color Codes to Binary:
HTML Structure: Similar to the previous plan.
SASS Integration:
Create SASS files for styling, e.g., styles/main.scss.
Utilize SASS features for styling the color display area, input fields, and buttons.
JavaScript Functionality: Remains the same as previously outlined.
3. RGB adjustor that takes an image and changes what the image looks like.
2. Convert Messages into Binary for Color Display:
HTML Structure: Similar to the previous plan.
SASS Integration:
Create SASS files for styling, e.g., styles/main.scss.
Utilize SASS for styling the message display area, input field, and button.
JavaScript Functionality: Remains the same as previously outlined.
3. Logic Gates Interactive Display:
HTML Structure: Similar to the previous plan.
SASS Integration:
Create SASS files for styling, e.g., styles/main.scss.
Utilize SASS for styling buttons, input fields, display area, and the logic gate simulation area.
JavaScript Functionality: Remains the same as previously outlined.
4. Binary/Decimal Calculator:
HTML Structure: Similar to the previous plan.
SASS Integration:
Create SASS files for styling, e.g., styles/main.scss.
Utilize SASS for styling input fields, buttons, display area, and calculator components.
JavaScript Functionality: Remains the same as previously outlined.
Steps to integrate SASS:
Create SASS File Structure: Set up a folder structure for SASS files.
Write SASS Styles: Utilize SASS features to style HTML elements and components.
Compile SASS to CSS: Use npm scripts or build tools to compile SASS files into CSS.
Link Compiled CSS in HTML/JavaScript: Link the compiled CSS file in your HTML file or import it into your JavaScript components.
Considerations:
SASS Organization: Organize SASS files using partials, mixins, and variables for better maintainability.
Compile Workflow: Ensure that SASS compilation is part of your development workflow.
File Structure: Keep the SASS file structure consistent and aligned with your JavaScript components for easier management.
By integrating SASS into your JavaScript project, you can leverage its capabilities to improve the styling aspects of your tools while keeping the JavaScript functionalities intact.

## Binary and How It Works
Input Values (A, B): Binary input values are represented by 'A' and 'B', each consisting of 0s and 1s.

Logic Gates:

AND Gate: Produces an output of 1 only if both inputs (A and B) are 1; otherwise, the output is 0.
OR Gate: Produces an output of 1 if at least one input (A or B) is 1; the output is 0 only if both inputs are 0.
NOT Gate: Inverts the input; if input A is 1, the output is 0, and vice versa.
Output (Result): The output of the logic gates (AND, OR, NOT) generates the result based on the input values and the function performed.
For an AND gate:
If A = 1 and B = 1, the output is 1.
If A = 1 and B = 0, the output is 0.
If A = 0 and B = 0, the output is 0.
This diagram simplifies the operation of basic binary functions using logic gates, sh

