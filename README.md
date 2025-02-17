# CSS Specificity Issue with !important and Inheritance

This repository demonstrates an uncommon CSS bug related to specificity and the `!important` flag.  The bug showcases how the `!important` flag can unexpectedly override inherited styles even with more specific selectors.

## Bug Description

A common understanding of CSS specificity is that more specific selectors override less specific ones.  However, the `!important` flag can disrupt this expectation.  This example highlights a scenario where a less specific selector with `!important` overrides a more specific selector that does not.

## How to Reproduce
1. Clone this repository.
2. Open `bug.css` and `bugSolution.css`.
3. Observe the unintended styling in `bug.css` and the corrected styling in `bugSolution.css`.

## Solution
The solution involves removing the unnecessary `!important` flag and relying on the proper specificity of CSS selectors.  Always avoid using `!important` unless absolutely necessary.  Consider using a more specific selector or a different styling approach to achieve the desired result without using `!important`. 