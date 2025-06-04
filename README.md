# Bash Commands & Git Practice Repository

A curated collection of useful Bash commands, scripts, and Git workflows to boost productivity and streamline project organization. This repository also documents my learning journey with Git branching, file management, and GitHub integration.

---

## Table of Contents

- [About](#about)
- [Bash Commands](#bash-commands)
- [Git Commands](#git-commands)
- [Git Branching Workflow](#git-branching-workflow)
- [Local Project Organization](#local-project-organization)
- [Setting Up a New Repo & Pushing to GitHub](#setting-up-a-new-repo--pushing-to-github)
- [Contributing](#contributing)
- [License](#license)

---

## About

This repository began as a way to practice Bash commands for project setup, file management, and other common shell tasks. Along the way, I learned to use Git branches, commit changes, and manage workflows both locally and remotely.

---

## Bash Commands

### Create Multiple Project Folders with Starter Files

```bash
for i in {1..10}; do
  mkdir "project$i" && touch "project$i/index.html" "project$i/style.css" "project$i/script.js"
done
```
Creates folders named `project1` to `project10`, each containing `index.html`, `style.css`, and `script.js`.

### Move All Files from One Folder to Another

```bash
mv source_folder/* destination_folder/
```

---

## Git Commands

### Viewing Branches

```bash
git branch
```
Lists all local branches. The current branch is marked with an asterisk (`*`).

### Creating and Switching Branches

```bash
git checkout -b branch_name
```
Creates a new branch and switches to it.

```bash
git checkout branch_name
```
Switches to an existing branch.

### Adding Files and Committing Changes

```bash
git add .
```
Stages all changed files.

```bash
git add filename
```
Stages a specific file.

```bash
git commit -m "Your commit message"
```
Commits staged changes with a message.

### Pushing Branches to Remote

```bash
git push -u origin branch_name
```
Pushes the branch to the remote repository and sets it to track the remote branch.

### Linking a Local Repo to a Remote GitHub Repo

```bash
git remote add origin https://github.com/<YOUR-GITHUB-USERNAME>/<REPO-NAME>.git
```
Connects your local repo to a GitHub remote.

### Renaming the Branch to Main

```bash
git branch -M main
```
Renames the current branch to `main`.

---

## Important Notes

- Run Git commands inside your repository folder.
- Only files inside the repo folder are tracked by Git.
- Branches are local to each repo; switching branches changes the visible files/folders.

---

## Git Branching Workflow

Key takeaways:

- Branches belong to the Git repository folder.
- To create and switch to a new branch:
  ```bash
  git checkout -b Bash_Commands
  ```
- To commit changes:
  ```bash
  git commit -m "Your commit message"
  ```
- Always push your branch to remote:
  ```bash
  git push origin Bash_Commands
  ```

---

## Local Project Organization

To keep your Bash commands and scripts organized:

- Create a dedicated folder inside your repo, e.g., `Bash_Commands/`.
- Store your scripts (`.sh` files) and command snippets there.
- Keep a `README.md` inside the folder explaining each script or snippet.

**Example structure:**
```
PROGRAMMING/
└── Bash_Commands/
    ├── README.md
    ├── scripts/
    │   ├── create_projects.sh
    │   └── move_files.sh
    └── snippets.md
```

---

## Setting Up a New Repo & Pushing to GitHub

**Steps:**

1. **Create and navigate to a new folder:**
    ```bash
    mkdir ~/Desktop/my-new-repo
    cd ~/Desktop/my-new-repo
    ```

2. **Initialize Git:**
    ```bash
    git init
    ```

3. **Add your first file:**
    ```bash
    echo "# My New Repo" > README.md
    git add README.md
    git commit -m "Initial commit"
    ```

4. **On GitHub, create a new repository (without README or .gitignore).**

5. **Link your local repo to GitHub and push:**
    ```bash
    git remote add origin https://github.com/<YOUR-GITHUB-USERNAME>/<REPO-NAME>.git
    git branch -M main
    git push -u origin main
    ```

---

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

---

## License

This project is licensed under the MIT License.

