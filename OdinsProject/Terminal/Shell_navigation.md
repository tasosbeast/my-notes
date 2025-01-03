# 📂 Unix Shell Navigation Guide

# Mastering the Unix Shell: Navigating Files and Directories

Understanding how to navigate and manage files and directories is a fundamental skill for using the Unix shell effectively. This guide covers essential commands and concepts for working with the filesystem.

---

## 📂 Introduction to the Filesystem

The filesystem is a hierarchical structure that organizes data on a computer. At the top is the root directory (`/`), and below it are various directories containing files and subdirectories.

- **Files**: Store data, such as text, images, or executable programs.
- **Directories**: Containers for files or other directories, forming a tree-like structure.

---

## 🔍 Key Commands for Navigation

### 1. **Print Working Directory (`pwd`)**

- Displays the current location in the filesystem.
- Example:
  ```bash
  $ pwd
  /Users/nelle
  ```

---

### 2. **List Directory Contents (`ls`)**

- Shows the files and directories in the current directory.
- Options:
  - `-F`: Classifies files and directories.
  - `-a`: Includes hidden files (those starting with `.`).
- Example:
  ```bash
  $ ls -F
  Documents/ Desktop/ Pictures/
  ```

### 3. **Change Directory (`cd`)**

- Moves to a specified directory.
- Shortcuts:
  - `..`: Move up one level.
  - `~`: Go to the home directory.
  - `-`: Return to the previous directory.
- Example:
  ```bash
  $ cd Desktop
  $ pwd
  /Users/nelle/Desktop
  ```

---

## 🛤️ Paths: Absolute vs. Relative

### Absolute Path

- Specifies a location from the root (`/`).
- Always starts with `/`.
- Example:
  ```bash
  /Users/nelle/Desktop
  ```

### Relative Path

- Specifies a location relative to the current directory.
- Does not start with `/`.
- Example:
  ```bash
  Desktop/shell-data
  ```

---

## 🚪 Navigating the Filesystem

### Moving to a Directory

- Use `cd` followed by the directory name.
  ```bash
  $ cd Documents
  ```

### Going Up a Level

- Use `cd ..` to move to the parent directory.
  ```bash
  $ cd ..
  ```

### Returning to Home

- Use `cd` or `cd ~`.
  ```bash
  $ cd
  ```

### Viewing Directory Contents

- Use `ls` with optional arguments.
  ```bash
  $ ls -a -F
  ```

---

## 🌟 Useful Features

### Tab Completion

- Press `Tab` to autocomplete file or directory names.
- Example:
  ```bash
  $ cd Des
  # Press Tab
  $ cd Desktop
  ```

### Hidden Files

- Files starting with `.` are hidden by default.
- View them using `ls -a`.
  ```bash
  $ ls -a
  .bash_profile  Documents  .hidden_file
  ```

---

## 🛠️ Combining Commands and Options

- Combine multiple options for tailored outputs.

  ```bash
  $ ls -l -h
  ```

- Use `man` or `--help` for command documentation.
  ```bash
  $ man ls
  $ ls --help
  ```

---

## 🚀 Example Workflow

### Navigating to a Directory

```bash
$ cd ~/Desktop/shell-lesson-data
```

### Listing Contents

```bash
$ ls -F
exercise-data/ north-pacific-gyre/
```

### Moving Between Directories

```bash
$ cd exercise-data
$ pwd
/Users/nelle/Desktop/shell-lesson-data/exercise-data
```

### Returning to Previous Directory

```bash
$ cd -
```

---

## 💡 Key Points Recap

- **`pwd`**: Shows the current directory.
- **`ls`**: Lists files and directories.
- **`cd`**: Navigates between directories.
- Absolute paths start at `/`, while relative paths are based on the current location.
- Use `..` to move up and `~` to return home.
- Hidden files start with `.` and require `ls -a` to view.

With these tools and techniques, you'll navigate the Unix shell like a pro!
