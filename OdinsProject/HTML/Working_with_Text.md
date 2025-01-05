# Working with Text | Notes

These notes summarize the "Working with Text" lesson from The Odin Project, explaining how to structure and style text using HTML.

---

## 📜 Overview

Text is a fundamental part of web content. This lesson covers essential HTML elements for text formatting, relationships between elements, and how to create HTML comments.

---

## 🖋️ HTML Text Elements

### 1. **Paragraphs**

- Use the `<p>` tag to create paragraphs.
- Adds a new line after each paragraph.
- Example:
  ```html
  <p>This is a paragraph of text.</p>
  ```

### 2. **Headings**

- Six levels of headings: `<h1>` to `<h6>`.
- `<h1>` is the largest and most important, `<h6>` is the smallest.
- Defines the content hierarchy.
- Example:
  ```html
  <h1>Main Heading</h1>
  <h2>Subheading</h2>
  ```

### 3. **Bold Text**

- **`<strong>`**: Makes text bold and semantically important for screen readers.
- Example:
  ```html
  <strong>This is important text.</strong>
  ```

### 4. **Italicized Text**

- **`<em>`**: Makes text italicized and semantically emphasized for screen readers.
- Example:
  ```html
  <em>This text has emphasis.</em>
  ```

---

## 🔄 Relationships and Nesting

- **Parent and Child**: When one element is nested within another, the outer element is the parent, and the inner element is the child.

  ```html
  <body>
    <p>This is a child of the body.</p>
  </body>
  ```

- **Siblings**: Elements at the same nesting level are siblings.

  ```html
  <body>
    <p>First paragraph (sibling 1).</p>
    <p>Second paragraph (sibling 2).</p>
  </body>
  ```

- **Indentation**: Use consistent indentation to improve readability.

---

## 💡 HTML Comments

- Use comments to leave notes or explanations in the code.
- Comments are not visible on the webpage.
- Syntax:
  ```html
  <!-- This is an HTML comment -->
  ```

---

## 🛠️ Tips and Tools

- **VS Code Comment Shortcut**:

  - **Mac**: `Cmd + /`
  - **Windows/Linux**: `Ctrl + /`

- Use Lorem Ipsum for dummy text:
  - In VS Code, type `lorem` and press Enter.

---

## 🎯 Key Takeaways

1. **Paragraphs**: Use `<p>` to structure text into readable sections.
2. **Headings**: Establish a content hierarchy with `<h1>` to `<h6>`.
3. **Bold/Italicized Text**: Use `<strong>` and `<em>` for semantic emphasis.
4. **Relationships**: Parent, child, and sibling relationships affect styling and behavior.
5. **Comments**: Annotate code with `<!-- -->` for clarity.

---

## 📖 Assignment and Resources

- Watch:
  - Kevin Powell’s **HTML Paragraph and Headings Video**.
  - Kevin Powell’s **HTML Bold and Italic Text Video**.
- Practice:
  - Create a simple blog article using headings, paragraphs, bold, and italicized text.
  - Validate your code with the [W3 HTML Validator](https://validator.w3.org/).

---

## 💡 Knowledge Check

1. How do you create a paragraph in HTML?
2. What are the six levels of headings, and how are they different?
3. How do `<strong>` and `<em>` tags differ semantically?
4. What is the relationship between parent and child elements?
5. How do you create comments in HTML?

Use these notes as a reference for structuring and formatting text in HTML!
