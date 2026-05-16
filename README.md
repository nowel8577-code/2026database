# 2026database

Classroom tool workspace connected to Firebase Firestore.

## Current Setup

- Workspace: `G:\我的雲端硬碟\2026database`
- Firebase project: `teacherstudy-38c15`
- Firestore rules: `firestore.rules`
- Firebase config: `firebase.json`
- Default writable collection: `wordcloud_words`

## Firestore

The current rules allow public read/write access only to `wordcloud_words` and deny all other collections.

Deploy rules with:

```powershell
npx.cmd -y firebase-tools@latest deploy --only firestore:rules
```

## Project Files

- `AGENTS.md`: Codex project working instructions
- `README.md`: project overview
- `.gitignore`: local and secret file exclusions
- `firebase.json`: Firebase deployment config
- `.firebaserc`: default Firebase project
- `firestore.rules`: Firestore security rules
