# Block and Inline | Notes

These notes summarize the differences between block and inline elements in CSS, their behavior, and the use of generic containers like `<div>` and `<span>`.

---

## 📜 Overview

CSS elements are categorized as **block** or **inline**, which determines how they behave within a document’s layout. Understanding these categories helps in structuring and styling web pages effectively.

---

## 🖋️ Block vs. Inline Elements

### 1. **Block Elements**

- Default display style: `display: block`.
- Take up the full width of their container by default.
- Start on a new line.
- Common block elements: `<div>`, `<p>`, `<h1>` to `<h6>`, `<section>`.
- Example:
  ```html
  <p>This is a block element.</p>
  ```

### 2. **Inline Elements**

- Default display style: `display: inline`.
- Occupy only as much width as their content.
- Do not start on a new line.
- Common inline elements: `<span>`, `<a>`, `<strong>`, `<em>`.
- Example:
  ```html
  <a href="#">This is an inline element.</a>
  ```

### 3. **Inline-Block Elements**

- Behave like inline elements but can have block-level padding and margins.
- Commonly used for layout purposes.
- Example:
  ```css
  .box {
    display: inline-block;
    width: 100px;
    height: 50px;
  }
  ```

---

## 🌟 Divs and Spans

### `<div>` (Block-Level)

- A generic container used to group related elements.
- Commonly used for structuring and applying styles or layouts to sections.
- Example:
  ```html
  <div class="container">
    <h1>Header</h1>
    <p>Paragraph inside a div.</p>
  </div>
  ```

### `<span>` (Inline-Level)

- A generic inline container used for grouping text or inline elements for styling.
- Best used when no semantic element is appropriate.
- Example:
  ```html
  <p>
    The word <span class="highlight">highlight</span> is styled differently.
  </p>
  ```

---

## 🎯 Key Differences Between Inline, Block, and Inline-Block

| Feature                | Block   | Inline  | Inline-Block |
| ---------------------- | ------- | ------- | ------------ |
| Starts on new line?    | Yes     | No      | No           |
| Takes full width?      | Yes     | No      | No           |
| Allows padding/margin? | Yes     | Limited | Yes          |
| Example                | `<div>` | `<a>`   | `<img>`      |

---

## ✨ Use Cases and Best Practices

1. **Use Block Elements**:

   - For major structural components (e.g., sections, headers, footers).
   - Example: `<div>`, `<section>`.

2. **Use Inline Elements**:

   - For styling parts of a text (e.g., highlighting, links).
   - Example: `<span>`, `<strong>`.

3. **Use Inline-Block**:
   - For aligning boxes side by side while maintaining block-like padding and margins.

---

## 🛠️ Assignments

1. **Read**:

   - MDN’s article on [Normal Flow](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flow_Layout/Normal_Flow).
   - W3Schools' guide on [Block and Inline Elements](https://www.w3schools.com/html/html_blocks.asp).

2. **Practice**:
   - Complete exercises in The Odin Project’s [CSS exercises repository](https://github.com/TheOdinProject/css-exercises) under the `foundations/block-and-inline` directory.

---

## 💡 Knowledge Check

1. What is the difference between a block element and an inline element?
2. When should you use `<div>` vs. `<span>`?
3. How does `display: inline-block` differ from `display: block`?

---
