# Inconsistent Width Calculation with CSS calc()

This repository demonstrates an uncommon issue encountered when using the `calc()` function in CSS to calculate widths involving percentages and fixed lengths. The problem stems from the browser's interpretation of the calculation in the presence of elements with borders or padding, resulting in discrepancies from the expected values.

## Problem Description
The provided CSS code aims to set the width of an inner element to be 20px less than its parent container.  However, due to the interaction between percentages, lengths, and the parent's border, the calculated width may be inaccurate in certain browsers.

## Solution
The solution involves adjusting the calculation within `calc()` to explicitly account for the border width, ensuring consistent and accurate width calculation across different browsers.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` (or view the example in this README) in a web browser.
3. Observe the inconsistent width of the blue inner element across different browsers.
4. Compare with `bugSolution.html` for the corrected behavior.