# The Cascade | Notes

These notes summarize key concepts about the CSS cascade, specificity, and inheritance, helping you understand how CSS rules are applied when multiple rules conflict.

---

## 📜 Overview

The **CSS Cascade** determines which rules are applied to an element when there are conflicting declarations. Understanding the cascade is essential to avoid unexpected results and efficiently manage CSS.

---

## 🖋️ Key Concepts

### 1. **Specificity**

Specificity determines the priority of CSS rules:

- **More specific rules take precedence** over less specific ones.
- **Hierarchy of Selectors** (from highest to lowest specificity):
  1. Inline styles (e.g., `style="color: red;"`).
  2. **ID Selectors** (e.g., `#header`).
  3. **Class, Attribute, and Pseudo-Class Selectors** (e.g., `.button`, `[type="text"]`, `:hover`).
  4. **Type Selectors** (e.g., `h1`, `p`) and **Pseudo-Elements** (e.g., `::before`).
  5. **Universal Selector (`*`)** and combinators like `>` or `+` have no specificity value.

#### Examples:

```css
/* Rule 1 */
#header {
  color: blue;
}

/* Rule 2 */
.header {
  color: red;
}

/* Result: color is blue because ID selectors have higher specificity. */
```

---

### 2. **Rule Order**

- When specificity is the same, the **last defined rule** takes precedence.
- Example:

  ```css
  .alert {
    color: red;
  }

  .alert {
    color: yellow;
  }
  /* Result: color is yellow because the second rule is defined later. */
  ```

---

### 3. **Inheritance**

- Certain properties are inherited by child elements, such as:
  - **Typography properties**: `color`, `font-family`, `font-size`.
- Non-inherited properties, like `margin` or `background-color`, need explicit rules.

#### Example:

```css
/* Parent rule */
#parent {
  color: red;
}

/* Child rule overrides inheritance */
.child {
  color: blue;
}
```

---

### 4. **The Cascade**

The cascade resolves conflicts by considering:

1. **Importance**: Inline styles and `!important` rules have the highest priority.
2. **Specificity**: More specific rules win.
3. **Source Order**: Later rules override earlier ones.

---

## ✨ Key Takeaways

1. Use **specificity** to control which rules apply.
2. Write clear and organized CSS to minimize conflicts.
3. Avoid overusing `!important`, as it can make debugging difficult.

---

## 🎯 Assignment

1. Complete the cascade-related exercises in The Odin Project's CSS repository.
2. Style a webpage using the external CSS method and experiment with specificity, inheritance, and rule order.

---

## 💡 Knowledge Check

1. Between a rule with one class selector and a rule with three type selectors, which has higher specificity?
2. How does inheritance affect typography properties like `color` and `font-size`?
3. What happens when two rules have the same specificity?
