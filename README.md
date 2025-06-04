# Bash Commands & Git Practice Repository

This repository is a collection of useful Bash commands, scripts, and Git workflows aimed at improving productivity and project organization. It also documents my learning process with Git branching, file management, and GitHub integration.

---

## Table of Contents

- [About](#about)
- [Bash Commands](#bash-commands)
- [Git Commands I Learned and Found Useful](#git-commands-i-learned-and-found-useful)
- [Git Branching Workflow](#git-branching-workflow)
- [Local Project Organization](#local-project-organization)
- [Setting Up a New Repo & Pushing to GitHub](#setting-up-a-new-repo--pushing-to-github)
- [Contributing](#contributing)
- [License](#license)

---

## About

This repo started as a way to practice Bash commands for project setup (creating folders/files), moving files, and other common shell tasks. Along the way, I learned to better use Git branches, commit changes, and manage multiple workflows locally and remotely.

---

## Bash Commands

Here’s a handy Bash snippet to quickly create multiple project folders, each with starter files:

```bash
for i in {1..10}; do
  mkdir "project$i" && touch "project$i/index.html" "project$i/style.css" "project$i/script.js"
done
