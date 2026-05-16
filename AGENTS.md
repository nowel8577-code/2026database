# 2026database AGENTS.md

## Project Context

Project name: 2026database
Project type: Classroom tool workspace with Firebase Firestore
Local workspace: G:\我的雲端硬碟\2026database
GitHub repo: not linked yet
Main branch: main

## Firebase

Firebase project ID: teacherstudy-38c15
Firestore rules file: firestore.rules
Firebase config file: firebase.json
Allowed public collection: wordcloud_words

Current Firestore rule policy:
- Allow public read and write for `wordcloud_words`.
- Deny read and write for all other collections.

## Obsidian

Obsidian vault: not configured yet
Project note path: not configured yet

When Obsidian is configured, keep the project note as the single running project log and link it from this file.

## Sync Workflow

Startup workflow:
- Read this `AGENTS.md`.
- Check Git status.
- Check Firebase configuration files.
- Review the project note if Obsidian is configured.
- Do not pull, commit, or push without an explicit request.

Shutdown workflow:
- Summarize completed work.
- Check Git diff and status.
- Update the Obsidian project note if configured.
- Commit and push only when explicitly requested.

Project initialization workflow:
- Keep `AGENTS.md`, `README.md`, `.gitignore`, Firebase config, and Git settings consistent.
- Keep secrets out of the repository.
- Use `npx.cmd` for Firebase CLI commands on Windows.

## Important Commands

```powershell
git status --short --branch
npx.cmd -y firebase-tools@latest projects:list
npx.cmd -y firebase-tools@latest deploy --only firestore:rules
```

## Safety Rules

- Do not commit `.codex/`, `.claude/`, `.env`, API keys, tokens, service account files, or secrets.
- Do not change Firestore security rules without confirming the target Firebase project.
- Do not overwrite this file blindly; update only the sections that changed.
