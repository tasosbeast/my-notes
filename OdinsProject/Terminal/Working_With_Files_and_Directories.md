---
# Working With Files and Directories in the Unix Shell

This lesson explores how to create, move, copy, and delete files and directories using the Unix shell. It also introduces concepts like file naming conventions, working with text editors, and using wildcards for batch operations.
---

## 📂 Creating Files and Directories

### Creating Directories

- **Command**: `mkdir [directory_name]`  
  Example:

  ```bash
  $ mkdir thesis
  ```

- **Nested Directories**: Use `-p` to create a hierarchy.
  ```bash
  $ mkdir -p project/data project/results
  ```

---

### Creating Files

- **Using a Text Editor**:  
  Use `nano`, `vim`, or other editors to create and edit files.  
  Example:

  ```bash
  $ nano draft.txt
  ```

- **Using `touch`**: Create an empty file.
  ```bash
  $ touch my_file.txt
  ```

---

## ✂️ Moving, Renaming, and Copying Files

### Moving and Renaming

- **Move/Rename**:
  ```bash
  $ mv old_name.txt new_name.txt
  ```
  Use `mv -i` for interactive confirmation to avoid overwriting files.

### Copying Files

- **Single File**:
  ```bash
  $ cp source.txt destination.txt
  ```
- **Recursive Copy**:
  ```bash
  $ cp -r source_dir/ backup_dir/
  ```

---

## 🗑️ Deleting Files and Directories

### Deleting Files

- **Remove Files**:
  ```bash
  $ rm file.txt
  ```
  Use `rm -i` for confirmation prompts.

### Deleting Directories

- **Recursive Delete**:
  ```bash
  $ rm -r directory/
  ```

---

## 🛤️ File Naming Conventions

- Avoid spaces: Use `-` or `_` instead.  
  Example: `north_pacific_gyre/` instead of `north pacific gyre/`.
- Avoid starting with `-`: Commands may interpret these as options.
- Use meaningful extensions (e.g., `.txt`, `.csv`, `.jpg`).

---

## 🔄 Batch Operations with Wildcards

### Wildcards

- `*`: Matches zero or more characters.  
  Example: `*.txt` matches all `.txt` files.
- `?`: Matches exactly one character.  
  Example: `?ethane.pdb` matches `methane.pdb`.

### Example Commands

- List all `.txt` files:

  ```bash
  $ ls *.txt
  ```

- Copy specific files:
  ```bash
  $ cp file1.txt file2.txt target_directory/
  ```

---

## 🛠️ Useful Tips and Commands

### Check Contents of Directories

- **List All Files**:

  ```bash
  $ ls -a
  ```

- **Recursive Listing**:
  ```bash
  $ ls -R
  ```

### Navigation and Shortcuts

- **Change Directory**:
  ```bash
  $ cd path/to/directory
  ```
- **Return Home**:
  ```bash
  $ cd
  ```
- **Go Back**:
  ```bash
  $ cd -
  ```

---

## 🚀 Examples and Practice

### Example: Organizing Files

1. Create a directory for results:
   ```bash
   $ mkdir results
   ```
2. Move files to the directory:
   ```bash
   $ mv data1.txt data2.txt results/
   ```

### Example: Wildcard Usage

- List all `.dat` files:
  ```bash
  $ ls *.dat
  ```
- Copy all `.pdb` files:
  ```bash
  $ cp *.pdb backup/
  ```

---

## 💡 Key Points Recap

- **`mkdir`**: Create directories.
- **`mv`**: Move or rename files and directories.
- **`cp`**: Copy files or directories.
- **`rm`**: Delete files or directories.
- **Wildcards**: `*` and `?` help manage multiple files.

With these commands, you can efficiently manage files and directories in the Unix shell!
