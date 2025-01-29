# CSS Specificity Bug: Unexpected Behavior with Complex Selectors

This repository demonstrates a subtle bug related to CSS specificity when combining ID selectors, class selectors, and element selectors in a cascaded manner.  Some browsers might not correctly interpret the specificity and produce unexpected results.

The bug involves using selectors with high specificity that could lead to unexpected rendering behavior across different browsers.  The solution showcases how to solve the issue by carefully revisiting the selectors and potentially simplifying the CSS rules.

## How to reproduce:

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe the text color.  The expected color is purple, but you might see a different color depending on the browser and its CSS engine implementation.

## Solution:

The solution provided in `bugSolution.css` addresses the issue by making sure the selector that takes precedence is well defined and that there are no ambiguous rules that are dependent on the order.