# Unexpected Behavior with CSS calc() function

This repository demonstrates an uncommon error that can occur when using the CSS `calc()` function. Specifically, it highlights issues related to mixing incompatible units and subtracting percentages from percentages within a single `calc()` expression.

## Bug Report
The `bug.css` file contains CSS code that demonstrates the unexpected behavior. The main issues are:

1. **Mixing incompatible units:** Using `calc()` with a mixture of units (e.g., `em` and `px`) without proper unit conversion can lead to unpredictable results.
2. **Subtracting percentages from percentages:** Using `calc()` to directly subtract percentages from percentages can also lead to unexpected results, as percentages are relative to the containing element's size.

## Solution
The `bugSolution.css` file provides a corrected version of the CSS code. It addresses the issues mentioned above by:

1. Using consistent units throughout the `calc()` expression (e.g., converting all units to pixels).
2. Avoiding direct subtraction of percentages. Instead, explicit calculations are made based on the containing element's dimensions.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` (or create your own HTML file with a div that uses the provided CSS) in your web browser.
3. Observe the unexpected behavior of the element with the incorrect `calc()` expression.
4. Replace `bug.css` with `bugSolution.css`.  
5. Refresh the page and observe the corrected behavior.
