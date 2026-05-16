# Onboarding Task

This repository documents the setup and onboarding task I was assigned.

## Tools Installed

- **Visual Studio Code** — primary code editor.
- **Claude Code extension** (for VS Code) — AI coding assistant, installed from the
  Extensions marketplace and signed in with my Claude account.
- **Git** (v2.54.0, Windows) — version control, used for committing and pushing this repo.

> **Note on the original task:** The task originally listed *Cursor IDE* with the
> *Claude Code* and *Codex* extensions. To complete the task faster I used my
> existing **VS Code + Claude Code** setup instead, which provides the same core
> AI-assisted workflow. Cursor and Codex were not installed.

## Steps Completed

1. Confirmed VS Code was installed and working.
2. Installed the **Claude Code** extension in VS Code (Extensions → search
   "Claude Code" → Install) and logged in with my Claude account.
3. Verified Git was installed (`git --version` → 2.54.0).
4. Created a **public** repository on GitHub via the GitHub website.
5. Opened the project folder in VS Code.
6. Created this `README.md` describing the tools, steps, and issues.
7. Initialized a local Git repository, committed the work, and pushed it to GitHub.

## Issues Encountered & Solutions

| Issue | Solution |
|-------|----------|
| Task specified Cursor IDE + Codex, but installing two new tools would be slow. | Used existing **VS Code + Claude Code**, which covers the same AI-coding workflow. |
| GitHub CLI (`gh`) was not installed, so the repo couldn't be created from the terminal. | Created the public repository through the **GitHub website** (github.com/new) instead. |
| No global Git identity (`user.name` / `user.email`) was configured, so commits would fail. | Set the identity **locally** for this repository with `git config user.name` / `user.email`. |

## How to Reproduce

```bash
git clone https://github.com/<your-username>/onboarding-task.git
cd onboarding-task
```
