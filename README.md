# Inconsistent Calculations with CSS calc() and Percentage or Viewport Units

This repository demonstrates an uncommon CSS bug related to the `calc()` function and its interaction with percentages, `em`, `rem`, `vh`, and `vw` units.  The issue arises from inconsistencies in the calculation order and how the browser handles unit conversions within the `calc()` function. This can result in unexpected element dimensions that differ from the expected calculated values.

## Description

The `calc()` function is powerful for dynamic CSS, but combining it with percentage or viewport-relative units can lead to subtle errors.  These discrepancies are often due to rounding errors or the order of calculations performed by the browser.

## Reproducing the Bug

The `bug.css` file contains CSS code illustrating the problem. Observe the actual dimensions of the affected elements to see the discrepancy compared to the expected values calculated from the CSS code.

## Solution

The `bugSolution.css` file provides a possible workaround or alternative approach that can help to mitigate this issue, demonstrating better practices for handling such calculations in CSS.  In many instances, using a JavaScript solution might provide more accuracy.