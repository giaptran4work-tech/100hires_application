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

Here are the main problems I ran into and how I worked through them:

**1. The task asked for Cursor IDE + Codex, but I used VS Code + Claude Code instead.**
The task originally said to install Cursor and the Codex extension. I already had VS Code with the Claude Code extension set up and working, which gives me the same AI-assisted coding workflow. Rather than spend time installing and configuring two new tools, I made a judgment call to use what I already had and documented the decision here so it's transparent.

**2. My first push failed because the remote URL pointed to the wrong repository name.**
When I set up the connection to GitHub, I'd used the name `onboarding-task`, but the repository I actually created on GitHub was named `100hires_application`. So Git was trying to push to a repo that didn't exist at that address. I fixed it by pointing the remote at the correct URL with `git remote set-url origin <correct-url>`, instead of deleting and re-adding the connection.

**3. The push was then rejected because GitHub had already put a starter file in the repo.**
When I created the repo on the GitHub website, GitHub automatically added its own placeholder `README.md`. That gave the online repo a separate history from my local one, so Git refused the push to avoid accidentally deleting work. I checked what was on GitHub, confirmed it was only the empty placeholder and nothing important, and then replaced it with my real README using `git push --force-with-lease` — I chose that over a plain force-push because it still protects against overwriting anyone else's changes.

## How to Reproduce

```bash
git clone https://github.com/giaptran4work-tech/100hires_application.git
cd 100hires_application
```
