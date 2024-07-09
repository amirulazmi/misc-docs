# Training Material: Version Control

## Introduction to Version Control

### What is Version Control?

Version Control, also known as source control, is a system that records changes to a file or set of files over time so that you can recall specific versions later. It allows multiple people to collaborate on a project, track changes, and manage versions efficiently.

### Why Use Version Control?

- **Collaboration**: Multiple developers can work on the same project simultaneously without overwriting each other’s work.
- **Backup**: Each version is saved, providing a backup in case of mistakes or data loss.
- **History Tracking**: Keeps a detailed history of changes, making it easy to review and revert to previous versions.
- **Branching and Merging**: Facilitates working on multiple features or fixes concurrently without affecting the main project.

## Key Concepts in Version Control

### Repository (Repo)

A repository is a storage location for software packages, often used to store multiple versions of code and related files. It can be hosted on a local machine or a remote server.

### Commit

A commit is a record of changes made to the files in the repository. Each commit includes a unique ID, a message describing the changes, and the author’s information.

### Branch

A branch is a parallel version of the repository. It allows developers to work on features or fixes independently of the main codebase. Branches can be merged back into the main codebase.

### Merge

Merging is the process of combining changes from different branches into one branch. This is typically done to integrate new features or fixes into the main branch.

### Conflict

A conflict occurs when changes from different branches clash with each other. Conflicts must be resolved manually to proceed with the merge.

## Popular Version Control Systems

### Git

Git is a distributed version control system that allows developers to work on a project from multiple locations. It’s known for its speed, flexibility, and robust branching and merging capabilities.

### Subversion (SVN)

SVN is a centralized version control system. It’s simpler than Git but doesn’t offer the same level of flexibility for branching and merging.

### Mercurial

Mercurial is another distributed version control system similar to Git, known for its simplicity and performance.

## Basic Git Commands

### Setting Up Git

1. **Install Git**:

   - For Windows: Download and install Git from [git-scm.com](https://git-scm.com/).
   - For macOS: Use Homebrew: `brew install git`.
   - For Linux: Use the package manager: `sudo apt-get install git` (Debian/Ubuntu).

2. **Configure Git**:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"
   ```

### Creating a Repository

1. **Initialize a New Repository:**

   ```bash
   git init
   ```

2. **Clone an Existing Repository:**
    ```bash
    git clone <repository-url>
    ```

### Basic Workflow
1. **Check Repository Status:**
    ```bash
    git status
    ```

2. **Add Changes to Staging Area:**
    ```bash
    git add <file>
    git add .
    ```

3. **Commit Changes:**
    ```bash
    git commit -m "Commit message"
    ```

4. **Push Changes to Remote Repository:**
    ```bash
    git push origin <branch-name>
    ```

5. **Pull Changes from Remote Repository:**
    ```bash
    git pull origin <branch-name>
    ```

### Branching and Merging
1. **Create a New Branch:**
    ```bash
    git branch <branch-name>
    ```

2. **Switch to a Branch:**
    ```bash
    git checkout <branch-name>
    ```

3. **Merge a Branch into the Current Branch:**
    ```bash
    git merge <branch-name>
    ```

4. **Delete a Branch:**
    ```bash
    git branch -d <branch-name>
    ```

### Resolving Conflicts
When a conflict occurs during a merge, Git will mark the conflicting files. You need to manually edit these files to resolve the conflicts.

1. **Edit the Conflicted Files to resolve conflicts.**
2. **Add the Resolved Files to the staging area:**
    ```bash
    git add <file>
    ```
3. **Commit the Merge:**
    ```bash
    git commit
    ```

### Best Practices for Version Control
- Commit Frequently: Make small, frequent commits to keep changes manageable.
- Write Meaningful Commit Messages: Clearly describe the changes in each commit.
- Use Branches for Features and Fixes: Keep the main branch clean by developing new features and fixing bugs in separate branches.
- Regularly Sync with the Remote Repository: Pull changes frequently to stay up-to-date with the team’s work.
- Review Code Changes: Use pull requests or code reviews to ensure code quality before merging changes.

### Conclusion
Version control is an essential practice in modern software development. It facilitates collaboration, ensures code quality, and helps manage the complexity of software projects. By mastering version control systems like Git, you can significantly improve your development workflow and productivity.