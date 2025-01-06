## Meet the Team - A Git Introduction

Welcome! This activity will introduce you to Git, a powerful version control system used by developers worldwide. We'll be creating personal introduction files and practicing a typical Git workflow, including creating branches, commits, and pull requests.

**What is Git?**

Git helps track changes to files, allowing multiple people to collaborate on projects efficiently. It keeps a history of every change, making it easy to revert to previous versions if needed.

**Our Goal:**

Each of you will create a short introduction about yourself and use Git to add it to a shared repository. This will give you hands-on experience with the basic Git workflow.

**Setup:**

*   Make sure you have a terminal or command prompt available on your computer.
*   You'll need a GitHub account. **Please share this with your trainer via email (charles.jester@revature.com) to be added to our Organization on GitHub to allow pushing of your file.**

**Steps:**

1.  **Cloning the Repository:**
    *   Open your terminal/command prompt.
    *   The `git clone` command downloads a copy of a repository to your local machine.
    *   Use the following command, to clone the remote repository as a local repository:

        ```bash
        git clone https://github.com/2164-ServiceNow/meet-the-team.git
        ```

    *   This will create a folder named `meet-the-team` in your current directory.
    *   Navigate into this folder using the `cd` (change directory) command:

        ```bash
        cd meet-the-team
        ```

2.  **Creating a Branch:**
    *   Branches allow you to work on changes without affecting the main project.
    *   The `git checkout -b <branch-name>` command creates and switches to a new branch.
    *   Create a branch with your name (e.g., `john-doe`):

        ```bash
        git checkout -b your-name
        ```

3.  **Creating and Committing a File:**
    *   Create a new text file named `introduction-your-name.txt` (e.g., `introduction-john-doe.txt`). You can do this using a text editor or from the command line (e.g., `touch introduction-your-name.txt` on macOS/Linux or `type nul > introduction-your-name.txt` on Windows). [Example: introduction-charles-jester.txt](https://github.com/2164-ServiceNow/meet-the-team/blob/main/introduction-charles-jester.txt)
    *   Write a short introduction about yourself in the file (name, where are you from, a fun fact, etc.).
    *   The `git add <file>` command stages changes for commit. To add your new file, use:

        ```bash
        git add introduction-your-name.txt
        ```

        Or to add all changes use:

        ```bash
        git add .
        ```

    *   The `git commit -m "Your commit message"` command saves your changes with a descriptive message:

        ```bash
        git commit -m "Add introduction file"
        ```

4.  **Pushing the Branch:**
    *   The `git push` command uploads your branch to the remote repository on GitHub:

        ```bash
        git push
        ```

5.  **Creating a Pull Request (PR):**
    *   Go to the `meet-the-team` repository on GitHub in your web browser.
    *   You should see a prompt to compare and create a pull request for your branch. Click it.
    *   Write a short description for your PR (e.g., "Adding my introduction").
    *   **Important:** Request a review from at least one other participant. This simulates a real-world code review process. (This will be available once GitHub accounts have been shared & added to organization)

6.  **(Challenge) Reviewing and Merging (If time allows):**
    *   Switch roles and review each other's pull requests.
    *   Leave comments on the PR if you have any feedback.
    *   Once a review is received, your trainer will merge it into the `main` branch by clicking the "Merge pull request" button on GitHub.

**Troubleshooting:**

If you encounter any errors, don't hesitate to ask your instructor for assistance.

Have fun and welcome to the team!
