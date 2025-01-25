# Unexpected Width Calculation using CSS `calc()` with Percentages and Pixels

This repository demonstrates a subtle bug related to the CSS `calc()` function. When combining percentages and fixed pixel values, unexpected results can occur, particularly when the parent container's dimensions are not fixed.

## The Problem

The `calc()` function, while powerful, can be tricky when dealing with percentages and absolute units like pixels. The browser's interpretation of the calculation depends on the context and the parent container's size, which can lead to inconsistencies.

## Reproducing the Bug

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Resize the browser window.  Observe that the width of the `.container` element doesn't adjust smoothly or as expected.

## Solution

The solution lies in ensuring the context of the calculation is correctly defined and consistently adjusted to changes in the parent container. See `bugSolution.css` for a possible solution.

## Additional Notes

This bug highlights the importance of understanding how browsers handle calculations within CSS, especially when percentages and absolute units are combined. Thorough testing and careful consideration of the context are crucial to avoid unexpected behavior.