# Intro to CSS | Notes

These notes summarize the foundational concepts of CSS from The Odin Project. CSS (Cascading Style Sheets) is used to style HTML, enabling you to control the layout, design, and appearance of web pages.

---

## 📜 Overview

CSS allows you to:

1. Add styles to HTML elements.
2. Target elements using selectors like classes and IDs.
3. Define rules to style multiple elements consistently.

---

## 🖋️ CSS Basics

### CSS Syntax

- A CSS rule has two main parts:
  1. **Selector**: Targets the HTML elements to style.
  2. **Declaration Block**: Contains property–value pairs.
  - Example:
    ```css
    h1 {
      color: blue;
      font-size: 24px;
    }
    ```

---

## 🎯 CSS Selectors

### 1. **Universal Selector**

- Targets all elements.
- Syntax: `* { ... }`

### 2. **Type Selector**

- Targets specific HTML elements.
- Example:
  ```css
  p {
    color: gray;
  }
  ```

### 3. **Class Selector**

- Targets elements with a specific class attribute.
- Syntax: `.class-name { ... }`
- Example:

  ```css
  <div class="highlight" > Content</div > .highlight {
    color: yellow;
  }
  ```

### 4. **ID Selector**

- Targets an element with a unique ID.
- Syntax: `#id-name { ... }`
- Example:

  ```css
  <div id="header" > Header</div > #header {
    background-color: blue;
  }
  ```

### 5. **Grouping Selectors**

- Combine selectors to share styles.
- Example:
  ```css
  h1,
  h2 {
    color: green;
  }
  ```

### 6. **Chaining Selectors**

- Combine multiple selectors for specific targeting.
- Example:
  ```css
  .subsection.header {
    color: red;
  }
  ```

### 7. **Descendant Combinator**

- Targets nested elements.
- Syntax: `parent child`
- Example:
  ```css
  .menu .item {
    color: white;
  }
  ```

---

## 🎨 Key CSS Properties

1. **Color and Background**

   ```css
   color: red;
   background-color: blue;
   ```

2. **Typography**

   - `font-family`: Specifies fonts.
   - `font-size`: Sets text size.
   - `font-weight`: Adjusts text boldness.
   - `text-align`: Aligns text horizontally.

3. **Image Dimensions**
   - Set height and width while maintaining aspect ratio:
     ```css
     img {
       height: auto;
       width: 500px;
     }
     ```

---

## 🛠️ Adding CSS to HTML

### 1. **External CSS**

- Link a `.css` file in the `<head>` of your HTML.
- Example:
  ```html
  <link rel="stylesheet" href="styles.css" />
  ```

### 2. **Internal CSS**

- Add styles inside `<style>` tags in the `<head>`.
- Example:
  ```html
  <style>
    body {
      background-color: lightgray;
    }
  </style>
  ```

### 3. **Inline CSS**

- Add styles directly to elements using the `style` attribute.
- Example:
  ```html
  <p style="color: blue;">Hello!</p>
  ```

---

## 🎯 Key Takeaways

1. **Selectors**: Allow you to target elements precisely.
2. **Best Practices**:
   - Use external CSS for scalability.
   - Use classes over IDs for reusability.
3. **Image Styling**: Explicitly set height and width to prevent layout shifts.

---

## 📖 Assignment

1. Complete exercises from The Odin Project's CSS repository:
   - CSS methods
   - Class and ID selectors
   - Group and chain selectors
   - Descendant combinator
2. Review the solutions and practice writing your own styles.

---

## 💡 Knowledge Check

1. What is the difference between a class and an ID selector?
2. How do you apply the same rule to multiple selectors?
3. What are the three ways to add CSS to an HTML file?
4. What does the descendant combinator do?

---
