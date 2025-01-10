# Alignment

## Overview

This lesson covers how to align flex items inside a flex container both horizontally (using `justify-content`) and vertically (using `align-items`). It also introduces the `gap` property for spacing between flex items.

---

## Key Concepts

### Justify-Content

- Aligns items along the **main axis**.
- Common values:
  - `flex-start`: Items align at the start.
  - `center`: Items are centered.
  - `space-between`: Items are spaced evenly with no gaps at the edges.
  - `space-around`: Items have equal space around them.
  - `space-evenly`: Equal space between and around items.
- Example:
  ```css
  .container {
    justify-content: space-between;
  }
  ```

### Align-Items

- Aligns items along the **cross axis**.
- Common values:
  - `flex-start`: Items align at the start of the cross axis.
  - `center`: Items are centered along the cross axis.
  - `flex-end`: Items align at the end of the cross axis.
  - `stretch`: Items stretch to fill the container.
- Example:
  ```css
  .container {
    align-items: center;
  }
  ```

---

## Gap Property

- **Definition**: Adds space between flex items.
- Eliminates the need to manually add margins to individual items.
- Supported in all modern browsers.
- Example:
  ```css
  .container {
    gap: 10px;
  }
  ```

---

## Behavior with Flex-Direction

- The behavior of `justify-content` and `align-items` depends on the **main** and **cross** axes:
  - Default (`flex-direction: row`):
    - Main axis: horizontal.
    - Cross axis: vertical.
  - With `flex-direction: column`:
    - Main axis: vertical.
    - Cross axis: horizontal.

---

## Practical Applications

1. **Centering an Element**:
   - Use both `justify-content` and `align-items`:
     ```css
     .container {
       display: flex;
       justify-content: center;
       align-items: center;
     }
     ```
2. **Spacing Between Items**:
   - Use `gap` for consistent spacing:
     ```css
     .container {
       display: flex;
       gap: 20px;
     }
     ```

---

## Knowledge Check

1. What is the difference between `justify-content` and `align-items`?
2. How does `gap` simplify adding space between flex items?
3. How does the behavior of `justify-content` and `align-items` change with `flex-direction: column`?

---

## Additional Resources

- [CSS Tricks Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [Flexbox Froggy Game](https://flexboxfroggy.com/)
- [MDN Aligning Items in Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Aligning_Items_in_a_Flex_Container)
