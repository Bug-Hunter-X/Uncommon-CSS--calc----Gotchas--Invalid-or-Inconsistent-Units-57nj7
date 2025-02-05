# Uncommon CSS `calc()` Gotchas

This repository demonstrates some less obvious issues that can arise when using the CSS `calc()` function.  Improper usage can lead to unexpected layout problems, particularly when calculations result in negative values or when mixing units inconsistently. 

The `bug.css` file contains examples of these issues. The `bugSolution.css` file offers solutions and best practices to avoid these problems.

## Issues:

1. **Negative Widths:** Using `calc()` to compute a width that results in a negative value will often render as 0, leading to elements disappearing.
2. **Inconsistent Units:** Mixing different units (e.g., percentages and ems) in a `calc()` expression can produce unexpected and inconsistent results across different contexts.

## Solutions:

1. **Conditional Logic:** Use CSS media queries or JavaScript to handle cases where `calc()` might produce negative values, ensuring a safe fallback.
2. **Unit Consistency:** Maintain consistent units within your `calc()` expressions to avoid unexpected behavior.
3. **Thorough Testing:** Test your `calc()` expressions across different screen sizes and font sizes to identify potential issues.