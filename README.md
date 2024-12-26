# JavaScript Type Coercion Bug

This repository demonstrates a subtle bug in JavaScript related to type coercion within conditional statements.  The bug arises from implicit type conversions during comparisons, leading to unexpected behavior when handling various data types.

## Bug Description
The `foo` function intends to check if a numeric value `x` is null, negative, or positive. However, due to JavaScript's loose typing and implicit type coercion, the comparison `x < 0` can yield unexpected results when `x` is not a number.  The condition evaluates to `true` under certain circumstances that may not be intended.

## Solution
The solution involves explicit type checking and conversion to ensure that the comparison is performed reliably only on numeric values.  This involves checking for the type of `x` explicitly before the comparison.

## How to reproduce
1. Clone this repository.
2. Open `bug.js` to see the buggy implementation.
3. Run the code using a JavaScript interpreter (e.g., Node.js).
4. Compare the output to the expected behavior of checking for `null`, negative or positive values.
5. View the `bugSolution.js` for the corrected implementation.