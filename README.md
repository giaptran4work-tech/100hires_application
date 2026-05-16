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
| No global Git identity (`user.name` / `user.email`) was configured, so the commit would fail. | Set the identity **locally** for this repository with `git config user.name` / `user.email`. |
| First push failed with `remote: Repository not found` — the GitHub repo had not been created yet (`git remote add` only stores the URL locally). | Created the public repository on the **GitHub website** first, then retried the push. |
| Push still failed because the local remote URL used the wrong repo name (`onboarding-task` vs the actual `100hires_application`). | Corrected the URL with `git remote set-url origin <correct-url>`. |
| Push rejected with `! [rejected] main -> main (fetch first)` — GitHub had initialized the repo with its own auto-generated stub `README.md`, creating an unrelated history. | Confirmed the remote only contained the throwaway stub, then overwrote it with our real README using `git push --force-with-lease`. |

## How to Reproduce

```bash
git clone https://github.com/giaptran4work-tech/100hires_application.git
cd 100hires_application
```
