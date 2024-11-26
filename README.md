# Detailed Documentation: Git and GitHub

---

## Table of Contents

1. [Introduction to Git](#introduction-to-git)  
2. [Installing Git](#installing-git)  
3. [Basic Git Commands](#basic-git-commands)  
4. [Introduction to GitHub](#introduction-to-github)  
5. [Working with GitHub](#working-with-github)  
6. [Advanced Git and GitHub Concepts](#advanced-git-and-github-concepts)  

---

## Introduction to Git

Git is a **distributed version control system** that helps track changes in files and coordinate work on those files among multiple people. 

### Why Use Git?

- **Version Control:** Maintain a history of file changes.  
- **Collaboration:** Work seamlessly in teams.  
- **Branching:** Experiment in isolated environments.  

---

## Installing Git

### Windows

1. Download Git from the [official website](https://git-scm.com/downloads).  
2. Run the installer and follow the prompts.  
3. Verify installation:  
   ```
   git --version
   ```

### macOS

- Use Homebrew:  
  ```
  brew install git
  ```
- Verify installation:  
  ```
  git --version
  ```

### Linux

- Use your package manager:  
  ```
  sudo apt update  
  sudo apt install git
  ```
- Verify installation:  
  ```
  git --version
  ```

---

## Basic Git Commands

<details>
<summary>Setting Up Git</summary>

```
# Configure Git with your name and email
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

</details>

<details>
<summary>Initializing a Repository</summary>

```
# Create a new Git repository
git init
```

</details>

<details>
<summary>Adding Files</summary>

```
# Add files to staging area
git add <file_name>
git add .
```

</details>

<details>
<summary>Committing Changes</summary>

```
# Save changes to the repository
git commit -m "Commit message"
```

</details>

<details>
<summary>Checking Status</summary>

```
# View the state of your working directory
git status
```

</details>

<details>
<summary>Viewing History</summary>

```
# View commit history
git log
```

</details>

---

## Introduction to GitHub

GitHub is a web-based platform for hosting Git repositories. It provides tools for collaboration, version control, and code sharing.

### Why Use GitHub?

- **Centralized Hosting:** Store your Git repositories online.  
- **Collaboration Tools:** Pull requests, code reviews, and discussions.  
- **CI/CD Integration:** Automate testing and deployment.  

---

## Working with GitHub

### Creating a Repository

1. Go to [GitHub](https://github.com).  
2. Log in and click on **New Repository**.  
3. Fill in repository details and click **Create Repository**.

### Connecting a Local Repo to GitHub

```
# Add remote URL
git remote add origin <repo_url>

# Push changes to GitHub
git push -u origin main
```

### Cloning a Repository

```
# Clone a repository from GitHub
git clone <repo_url>
```

### Branching and Pull Requests

<details>
<summary>Creating a Branch</summary>

```
# Create a new branch
git branch <branch_name>

# Switch to the new branch
git checkout <branch_name>
```

</details>

<details>
<summary>Creating a Pull Request</summary>

1. Push your branch to GitHub:  
   ```
   git push origin <branch_name>
   ```  
2. Go to your GitHub repository.  
3. Click **Pull Requests** > **New Pull Request**.  
4. Review and submit the pull request.

</details>

---

## Advanced Git and GitHub Concepts

<details>
<summary>Stashing Changes</summary>

```
# Save changes without committing
git stash

# Reapply stashed changes
git stash apply
```

</details>

<details>
<summary>Rebasing</summary>

```
# Rebase your branch onto another branch
git rebase <branch_name>
```

</details>

<details>
<summary>Resolving Merge Conflicts</summary>

- Open the conflicting file.  
- Edit the file to resolve conflicts.  
- Add and commit the resolved file.  

```
git add <file_name>
git commit
```

</details>

<details>
<summary>Using SSH for GitHub</summary>

1. Generate an SSH key:  
   ```
   ssh-keygen -t ed25519 -C "you@example.com"
   ```  
2. Add the key to your GitHub account.  
3. Clone or push using SSH:  
   ```
   git clone git@github.com:username/repository.git
   ```

</details>

---

This documentation serves as a beginner-friendly guide to Git and GitHub. For more advanced topics, consult the [official Git documentation](https://git-scm.com/doc) or [GitHub Docs](https://docs.github.com).
