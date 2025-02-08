# CSS calc() Unexpected Behavior in Flexbox

This repository demonstrates an uncommon issue with the CSS `calc()` function when used within a flexbox context.  The `calc()` function's evaluation order can lead to unexpected results if the parent container's size is not definitively determined before `calc()` is processed.

The `bug.css` file shows the problematic code, while `bugSolution.css` provides a solution using alternative techniques.

**Problem:**  `calc(100% - 10px)` within a flexbox item may not subtract 10px correctly if the parent's size isn't fixed.

**Solution:** Use techniques that ensure the parent's size is determined before the calculation or use a different approach that avoids the dependency on `calc()` within a flexbox layout.