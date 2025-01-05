# HTML Boilerplate | Notes

These notes summarize the "HTML Boilerplate" lesson from The Odin Project, explaining the basic structure of an HTML document and its essential components.

---

## 📜 Overview

An HTML document follows a basic structure called the **boilerplate**, which serves as the foundation for building webpages. Understanding its parts is crucial for creating functional and well-structured websites.

---

## 🖋️ Key Components of HTML Boilerplate

### 1. **Doctype Declaration**

- **Purpose**: Tells the browser which version of HTML to use.
- **Syntax**:
  ```html
  <!DOCTYPE html>
  ```

### 2. **HTML Element**

- Represents the root element of the document.
- Encloses all other elements.
- **Syntax**:
  ```html
  <html lang="en"></html>
  ```
  - **`lang` Attribute**: Specifies the language of the content for accessibility (e.g., screen readers).

### 3. **Head Element**

- Contains metadata and resources required for rendering the page.
- Does not display content on the webpage.
- **Common Elements in the `<head>`**:
  - **`<meta charset="UTF-8">`**: Ensures proper encoding of text, allowing special characters.
  - **`<title>`**: Sets the title of the webpage (visible in the browser tab).
- **Syntax**:
  ```html
  <head>
    <meta charset="UTF-8" />
    <title>My First Webpage</title>
  </head>
  ```

### 4. **Body Element**

- Contains all visible content, such as text, images, and links.
- Placed below the `<head>` element.
- **Syntax**:
  ```html
  <body>
    <h1>Hello World!</h1>
  </body>
  ```

---

## 🛠️ Creating an HTML File

1. Create a folder (e.g., `html-boilerplate`).
2. Inside the folder, create a file named `index.html`.
3. Add the boilerplate:
   ```html
   <!DOCTYPE html>
   <html lang="en">
     <head>
       <meta charset="UTF-8" />
       <title>My First Webpage</title>
     </head>
     <body>
       <h1>Hello World!</h1>
     </body>
   </html>
   ```

---

## 🌐 Viewing HTML in a Browser

- **Methods**:
  - Drag and drop the file into the browser.
  - Double-click the file in your file explorer.
  - Use a terminal command:
    - **Ubuntu**: `google-chrome index.html`
    - **macOS**: `open ./index.html`
    - **WSL**: `explorer.exe index.html`

---

## 🚀 VS Code Boilerplate Shortcut

1. Open an `.html` file.
2. Type `!` and press `Enter`.
3. The boilerplate will be automatically populated.

---

## 🎯 Key Takeaways

1. **Doctype**: Ensures proper rendering of the page in the browser.
2. **Root Element**: `<html>` encloses all elements in the document.
3. **Metadata**: `<head>` includes the title and encoding settings.
4. **Content**: `<body>` contains all visible elements.

---

## 📖 Assignment and Resources

- Watch *[*Kevin Powell’s Building Your First Web Page](https://www.youtube.com/watch?v=V8UAEoOvqFg&t=93s)\*\* video.
- Practice writing the boilerplate from memory multiple times.
- Validate your HTML with the [W3 HTML Validator](https://validator.w3.org/).

---

## 💡 Knowledge Check

1. What is the purpose of the doctype declaration?
2. What does the `<html>` element do?
3. Why is the `<meta charset="UTF-8">` tag important?
4. What does the `<title>` element do?

Use these notes as a reference to build a solid foundation for working with HTML!
