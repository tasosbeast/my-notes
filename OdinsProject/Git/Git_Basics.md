
# Git Basics | Notes

These notes summarize key concepts and commands from the Git Basics lesson in The Odin Project. They cover repository setup, managing files, version control workflows, and best practices for using Git effectively.

---

## 📂 Repository Setup

### Creating a Repository on GitHub
1. Go to GitHub and create a new repository.
2. Add a name (e.g., `git_test`) and select "Add a README file."
3. Clone the repository using SSH:
   ```bash
   git clone git@github.com:USER-NAME/REPOSITORY-NAME.git
   ```

4. Check the remote connection:
   ```bash
   git remote -v
   ```

---

## 🔄 Basic Git Workflow

### 1. Check Status
- View the current state of your repository:
  ```bash
  git status
  ```

### 2. Stage Changes
- Add specific files to the staging area:
  ```bash
  git add <file_name>
  ```
- Add all changes:
  ```bash
  git add .
  ```

### 3. Commit Changes
- Commit staged files with a message:
  ```bash
  git commit -m "Descriptive commit message"
  ```

### 4. Push to Remote
- Push committed changes to GitHub:
  ```bash
  git push
  ```

---

## 📜 Managing Files

### Adding and Editing Files
1. Create a new file:
   ```bash
   touch hello_world.txt
   ```
2. Edit the file with a text editor (e.g., `nano` or VS Code).

3. Stage and commit changes:
   ```bash
   git add hello_world.txt
   git commit -m "Add hello_world.txt"
   ```

### Checking Commit History
- View commit log:
  ```bash
  git log
  ```
  Press `q` to exit the log view.

---

## ✏️ Best Practices

### Atomic Commits
- Group changes related to a single feature or task in one commit.
- Benefits:
  - Easier to debug specific changes.
  - Simplifies collaboration and code review.

### Commit Messages
- Write clear and descriptive messages.
- Example:
  ```bash
  git commit -m "Fix bug in login function"
  ```

---

## 🔗 Customizing Git

### Set Default Branch to `main`
```bash
git config --global init.defaultBranch main
```

### Configure VS Code as the Default Editor
```bash
git config --global core.editor "code --wait"
```

---

## 🔧 Git Commands Cheatsheet

### Remote Repository
- Clone a repository:
  ```bash
  git clone git@github.com:USER-NAME/REPOSITORY-NAME.git
  ```
- Push changes:
  ```bash
  git push
  ```

### Workflow Commands
- Stage changes:
  ```bash
  git add .
  ```
- Commit changes:
  ```bash
  git commit -m "Commit message"
  ```

### Status and History
- Check repository status:
  ```bash
  git status
  ```
- View commit log:
  ```bash
  git log
  ```

---

## 🚀 Example Workflow

1. Clone a repository:
   ```bash
   git clone git@github.com:USER-NAME/REPOSITORY-NAME.git
   ```

2. Create or edit files:
   ```bash
   touch hello_world.txt
   echo "Hello Git!" >> hello_world.txt
   ```

3. Stage and commit changes:
   ```bash
   git add .
   git commit -m "Add hello_world.txt"
   ```

4. Push changes to GitHub:
   ```bash
   git push
   ```

---

## 💡 Key Points Recap

- **`git status`**: Check repository state.
- **`git add`**: Stage files for commit.
- **`git commit`**: Save a snapshot of changes.
- **`git push`**: Upload changes to GitHub.
- **Atomic commits**: Focus each commit on one task or feature.

Use these notes as a reference to streamline your Git workflow and keep your projects organized!