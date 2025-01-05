# Commit Messages | Notes

These notes summarize key practices and rules for writing effective commit messages in Git, including **The Odin Project** and **cbea.ms** best practices, as well as examples of when to include a commit message body.

---

## 📜 Overview

Commit messages are critical for:

1. **Collaboration**: Helping team members understand changes and decisions.
2. **Debugging**: Identifying when and why changes were made.
3. **Maintenance**: Revisiting code after a break or debugging legacy systems.

A good commit message answers **what** changed and **why**, leaving out unnecessary details about **how** (the code provides that).

---

## 🖋️ The Anatomy of a Good Commit Message

### 1. Subject Line

- A concise summary (50 characters or less).
- Written in **imperative mood** (e.g., "Fix typo in README").
- No trailing punctuation.
- Example:
  ```plaintext
  feat: add basic structure for the hero section
  ```

### 2. Body (Optional)

- Provides detailed context about the changes.
- Wrap text at 72 characters per line for readability.
- Separates the **what** and **why** from the **how**.
- Example:

  ```
  Improve loading speed for large datasets.

  Previously, queries with over 10k results would cause delays due to
  inefficient indexing. This change adds lazy-loading for results.

  Fixes #123.
  ```

---

## 🔑 When and Why to Add a Commit Message Body

### When to Include a Body

1. **If the Subject Alone is Insufficient**:
   - When the subject doesn’t fully explain the purpose of the commit.
2. **To Document Context**:
   - Explain why the change was made (e.g., a bug fix or client request).
3. **To Highlight Side Effects**:
   - Describe additional impacts or decisions related to the change.

### Examples

1. **Adding Placeholder Content**:

   - **Commit**:

     ```plaintext
     feat: add placeholder content to the hero section

     Added temporary text and image placeholders to outline the layout.
     The final content will be added once assets are received from the
     client. This ensures the layout can be styled and tested in the meantime.
     ```

2. **Responsive Design Improvements**:

   - **Commit**:

     ```plaintext
     style: improve responsive design for navigation bar

     Reduced padding and font size in the navigation bar for screens
     under 768px width. This prevents text overflow issues and ensures
     the layout remains clean on smaller devices.
     ```

### Why it Matters

- **Context for Future Developers**:
  - Explains decisions that might not be obvious from the code.
- **Debugging**:
  - Provides clues about intent, making it easier to trace and fix bugs.
- **Collaboration**:
  - Helps teammates quickly understand changes and their rationale.

---

## 🔑 Best Practices for Commit Messages

### The Seven Rules (from cbea.ms)

1. **Separate the subject from the body with a blank line.**
2. **Limit the subject line to 50 characters.**
3. **Capitalize the subject line.**
4. **Do not end the subject line with a period.**
5. **Use the imperative mood in the subject line.**
6. **Wrap the body at 72 characters.**
7. **Explain what and why in the body, not how.**

---

## ⏳ When to Commit

- After meaningful changes, such as:

  1. Implementing a new feature.
  2. Fixing a bug.
  3. Updating documentation.

- Think of commits as **snapshots** of your progress. Frequent commits help trace issues and revert changes when necessary.

---

## 🎯 Assignment

1. Write five commits for a simple HTML/CSS project, following these rules.
2. Read the full article ["How to Write a Git Commit Message"](https://cbea.ms/git-commit/) for additional insights.

---

## 📖 Additional Resources

- [Conventional Commits](https://www.conventionalcommits.org/): Explore standardized commit message formats.
- **Pro Git**: A free online book for mastering Git.
