# Growing and Shrinking | Notes

These notes summarize the use of the `flex` shorthand property in CSS and its components: **flex-grow**, **flex-shrink**, and **flex-basis**. These properties determine how flex items size themselves within their container.

---

## 📜 Overview

The `flex` property in Flexbox is a shorthand for three properties:

1. **`flex-grow`**: Controls how much a flex item can grow.
2. **`flex-shrink`**: Controls how much a flex item can shrink.
3. **`flex-basis`**: Sets the initial size of a flex item before it grows or shrinks.

The shorthand makes it easy to define flexible layouts without writing verbose styles.

---

## 🖋️ Components of the `flex` Property

### **1. flex-grow**

- **Definition**: Specifies how much a flex item will grow relative to others when there is extra space in the container.
- **Default Value**: `flex-grow: 0` (items do not grow by default).
- **Usage**:
  ```css
  .item {
    flex-grow: 1; /* All items grow equally */
  }
  ```
- **Example**:
  - If one item has `flex-grow: 2` and others have `flex-grow: 1`, the first item will grow twice as much as the others.

---

### **2. flex-shrink**

- **Definition**: Specifies how much a flex item will shrink when the container is smaller than the total size of its items.
- **Default Value**: `flex-shrink: 1` (items shrink equally by default).
- **Usage**:
  ```css
  .item {
    flex-shrink: 0; /* Item will not shrink */
  }
  ```
- **Example**:
  - If one item has `flex-shrink: 2` and others have `flex-shrink: 1`, the first item shrinks twice as much as the others.

---

### **3. flex-basis**

- **Definition**: Sets the initial size of a flex item before growth or shrinkage.
- **Default Value in Shorthand**: `flex-basis: 0` (item size is based on content or other rules).
- **Usage**:
  ```css
  .item {
    flex-basis: 200px; /* Starts with a width of 200px */
  }
  ```
- **Key Note**: `flex-basis: auto` considers the item’s width or height before applying flex-grow or flex-shrink.

---

## ✨ The `flex` Shorthand

### **Syntax**:

```css
flex: [flex-grow] [flex-shrink] [flex-basis];
```

### **Common Values**:

1. **`flex: 1`**:

   - Equivalent to `flex: 1 1 0`.
   - Items grow and shrink equally, starting from a base size of `0`.

2. **`flex: auto`**:

   - Equivalent to `flex: 1 1 auto`.
   - Items grow and shrink equally, starting from their default size.

3. **`flex: none`**:
   - Equivalent to `flex: 0 0 auto`.
   - Items do not grow or shrink, and their size is determined by `flex-basis`.

---

## 🛠️ Practical Applications

1. **Equal Growth**:

   - Make items grow equally within a container:
     ```css
     .item {
       flex: 1; /* All items grow equally */
     }
     ```

2. **Prevent Shrinking**:

   - Prevent an item from shrinking while others adjust:
     ```css
     .item {
       flex-shrink: 0;
     }
     ```

3. **Custom Initial Sizes**:
   - Set initial sizes with `flex-basis` and allow proportional growth:
     ```css
     .item {
       flex: 2 1 100px;
     }
     ```

---

## 🎯 Key Takeaways

1. **`flex-grow`** determines how much extra space an item takes.
2. **`flex-shrink`** controls how items shrink when the container is too small.
3. **`flex-basis`** sets the starting size of an item.
4. Use shorthand values (`flex: 1`, `flex: auto`) for common use cases.

---

## 📖 Assignment

1. **Practice**:
   - Experiment with `flex-grow`, `flex-shrink`, and `flex-basis` values on [Scrimba’s Flexbox Demo](https://scrimba.com/learn/flexbox).
2. **Read**:
   - MDN Documentation on [Flex Property](https://developer.mozilla.org/en-US/docs/Web/CSS/flex).

---

## 💡 Knowledge Check

1. What does the `flex` shorthand represent?
2. How do `flex-grow` and `flex-shrink` differ?
3. What happens if you set `flex-basis` to `auto`?
