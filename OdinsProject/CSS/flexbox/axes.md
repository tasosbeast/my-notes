# Axes

## Overview

Flexbox operates along two axes:

1. **Main Axis**: Defined by the `flex-direction` property.
   - Default is `row` (horizontal, left-to-right).
2. **Cross Axis**: Perpendicular to the main axis.
   - Adjusts based on the `flex-direction`.

---

## Key Concepts

### 1. Changing Axes

- **`flex-direction: row`** (default):
  - Main axis is horizontal.
- **`flex-direction: column`**:
  - Main axis becomes vertical.
  ```css
  .flex-container {
    flex-direction: column;
  }
  ```

### 2. Impact on `flex-basis`

- **Row Direction**: `flex-basis` controls **width**.
- **Column Direction**: `flex-basis` controls **height**.

### 3. Common Issues and Fixes

- **Empty Flex Items Collapse**:
  - Occurs when using `flex: 1`, as `flex-basis` defaults to `0`.
  - Solutions:
    - Use `flex: 1 1 auto`.
    - Define a height for the parent container.
    - Use `flex-grow: 1` directly.

---

## Practical Insights

- **Block-Level Elements**: Default to full parent width, making horizontal layouts straightforward.
- **Column Flex Containers**: Require explicit heights for items to avoid collapsing due to the default height of `content`.

---

## Knowledge Check

1. How do you make flex items arrange vertically instead of horizontally?
2. What does `flex-basis` refer to in a column flex-container?
3. Why do `flex-basis` behaviors differ for rows and columns?

---

## Additional Resources

- [Flexbox Visual Cheatsheet](https://css-tricks.com/snippets/css/a-guide-to-flexbox/).
- [Interactive Demo on Flexbox Axes](https://scrimba.com/learn/flexbox).
