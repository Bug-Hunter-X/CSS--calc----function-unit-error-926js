# CSS `calc()` Function Unit Error

This repository demonstrates a common error encountered when using the `calc()` function in CSS. The issue arises from improperly handling units when subtracting pixel values from percentage values. This can result in unexpected rendering behavior across different browsers.

## Bug Description
The `calc(100% - 50px)` calculation is flawed because it attempts to directly subtract pixels from a percentage without explicitly specifying units for both values.  This often leads to inconsistent or incorrect width calculations.

## Solution
The solution involves ensuring consistent unit handling within the `calc()` function. Both the percentage and pixel values must have their units clearly defined.

## How to reproduce the bug
1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe the unexpected width of the div element.

## How to fix the bug
1. Replace `bug.css` with `bugSolution.css`
2. Reopen `bug.html` in your browser.
3. Observe the corrected width of the div element.