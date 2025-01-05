# Links and Images | Notes

These notes summarize the "Links and Images" lesson from The Odin Project, covering how to create and manage links, display images, and utilize the `<picture>` tag for responsive images in HTML.

---

## 📜 Overview

- **Links**: Connect web pages to other resources.
- **Images**: Embed visual content to enhance web pages.
- **Responsive Images**: Use the `<picture>` tag to serve different images based on the browser or device.

---

## 🖋️ Links in HTML

### Creating Links

- Use the `<a>` tag to create hyperlinks.
- The `href` attribute specifies the destination.
- Example:
  ```html
  <a href="https://example.com">Visit Example</a>
  ```

### Types of Links

1. **Absolute Links**:
   - Include the full URL (e.g., `https://example.com/page`).
2. **Relative Links**:
   - Refer to pages within the same website (e.g., `about.html`).

### Opening Links in New Tabs

- Use the `target="_blank"` attribute to open links in a new tab.
- Add `rel="noopener noreferrer"` for security:
  ```html
  <a href="https://example.com" target="_blank" rel="noopener noreferrer"
    >Open in New Tab</a
  >
  ```

---

## 🖼️ Images in HTML

### Displaying Images

- Use the `<img>` tag to embed images.
- The `src` attribute specifies the image path.
- The `alt` attribute provides a description for accessibility.
- Example:
  ```html
  <img src="image.jpg" alt="Description of the image" />
  ```

### Relative Paths for Images

- Use relative paths to reference images within the same project:
  ```html
  <img src="./images/photo.jpg" alt="Photo" />
  ```

### Parent Directory Access

- Use `../` to move up one level in the directory:
  ```html
  <img src="../images/photo.jpg" alt="Photo" />
  ```

---

## 🌟 Responsive Images with `<picture>` Tag

The `<picture>` tag allows you to serve different images based on browser capabilities or device size:

- **Structure**:  
  The `<picture>` element contains multiple `<source>` elements with different formats or resolutions.
- **Fallback**:  
  The `<img>` tag inside the `<picture>` acts as a fallback for browsers that don’t support `<picture>`.

### Example:

```html
<picture>
  <source srcset="image.avif" type="image/avif" />
  <source srcset="image.webp" type="image/webp" />
  <img src="image.jpg" alt="Description of the image" />
</picture>
```

- **How It Works**:
  1. The browser checks the `<source>` elements in order.
  2. If AVIF is supported, it loads `image.avif`.
  3. If AVIF isn’t supported, it falls back to WebP (`image.webp`).
  4. If neither AVIF nor WebP is supported, it defaults to the `<img>` tag (`image.jpg`).

---

## 🔄 Key Concepts

1. **Attributes**:
   - Add additional information to elements (e.g., `href`, `src`, `alt`).
2. **Absolute vs. Relative Links**:
   - Absolute: Full URL.
   - Relative: Local paths within the project.
3. **Alt Attribute**:
   - Describes the image for accessibility and acts as fallback text.
4. **Picture Tag**:
   - Enables responsive images and supports modern formats like AVIF and WebP.

---

## 🛠️ Best Practices

1. Always include `alt` text for images.
2. Use relative paths for easier file management.
3. Add `noopener noreferrer` when using `target="_blank"` for security.
4. Use the `<picture>` tag to optimize images for performance and compatibility.

---

## 🎯 Assignment

- Practice creating links and embedding images in an HTML project.
- Add alt attributes and relative paths to improve accessibility and organization.
- Use the `<picture>` tag to implement responsive images.
- Watch Kevin Powell’s videos on HTML links and images.

---

## 💡 Knowledge Check

1. How do you create a hyperlink in HTML?
2. What is the purpose of the `alt` attribute in images?
3. How do you access a parent directory in a file path?
4. How does the `<picture>` tag help with responsive images?
5. What are the benefits of using relative links in a project?

Use these notes to confidently work with links, images, and responsive design in your HTML projects!
