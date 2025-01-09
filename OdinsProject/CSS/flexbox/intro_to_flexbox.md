# Introduction to Flexbox | Notes

These notes summarize the foundational concepts of Flexbox, a powerful CSS layout tool for arranging items in rows or columns and creating responsive layouts.

---

## 📜 Overview

Flexbox is a modern CSS layout system that provides an efficient way to align and distribute space among items in a container. It is particularly useful for creating responsive designs and flexible layouts.

---

## 🖋️ Key Concepts

### 1. **Flex Containers**

- A **flex container** is any element with `display: flex`.
- It serves as the parent element, controlling the layout of its direct children.
- Example:
  ```css
  .flex-container {
    display: flex;
  }
  ```

### 2. **Flex Items**

- **Flex items** are the direct children of a flex container.
- They adapt their size and position based on the container's rules.
- Example:
  ```html
  <div class="flex-container">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
  </div>
  ```

### 3. **Flexbox Behavior**

- Flexbox aligns items horizontally (row) or vertically (column) by default.
- Items can grow, shrink, or be evenly distributed based on flex properties.

---

## 🎯 Core Flexbox Properties

### **For Flex Containers**

1. **`flex-direction`**: Defines the direction of items.

   - Options: `row` (default), `column`, `row-reverse`, `column-reverse`.
   - Example:
     ```css
     .flex-container {
       flex-direction: column;
     }
     ```

2. **`justify-content`**: Aligns items along the main axis.

   - Options: `flex-start`, `center`, `space-between`, `space-around`, `space-evenly`.
   - Example:
     ```css
     .flex-container {
       justify-content: center;
     }
     ```

3. **`align-items`**: Aligns items along the cross axis.

   - Options: `flex-start`, `center`, `flex-end`, `stretch`.
   - Example:
     ```css
     .flex-container {
       align-items: stretch;
     }
     ```

4. **`flex-wrap`**: Allows items to wrap onto new lines if needed.
   - Options: `nowrap` (default), `wrap`, `wrap-reverse`.
   - Example:
     ```css
     .flex-container {
       flex-wrap: wrap;
     }
     ```

---

### **For Flex Items**

1. **`flex`**: A shorthand for setting `flex-grow`, `flex-shrink`, and `flex-basis`.

   - Example:
     ```css
     .flex-item {
       flex: 1 1 auto;
     }
     ```

2. **`align-self`**: Overrides `align-items` for individual items.
   - Example:
     ```css
     .flex-item {
       align-self: center;
     }
     ```

---

## 🛠️ Tips and Best Practices

1. Use **developer tools** to inspect and debug flexbox layouts.
2. Experiment with code examples to understand how flex properties work together.
3. Combine flexbox with other layout techniques for complex designs.

---

## 🎨 Flexbox Use Cases

1. Centering content vertically and horizontally.
2. Creating responsive navigation bars.
3. Building complex layouts with nested flex containers.

---

## 📖 Assignment

1. **Practice**:
   - Experiment with interactive flexbox examples on [Flexbox Froggy](https://flexboxfroggy.com/).
2. **Resources**:
   - [CSS Tricks Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/).
   - [Learn Flexbox in 8 Minutes](https://www.youtube.com/watch?v=fYq5PXgSsbE).

---

## 💡 Knowledge Check

1. What is the difference between a flex container and a flex item?
2. How do `justify-content` and `align-items` differ?
3. What is the purpose of `flex-wrap` in a flex container?
