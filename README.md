# Eagle Word Tester

A kid‑friendly webpage for practicing English words from `full_eagle_word.js`.

## How to use (GitHub Pages)

1. Create a new GitHub repo (e.g., `eagle-word-tester`).
2. Upload **index.html** and **full_eagle_word.js** to the repo root (or just upload the provided ZIP contents).
3. In *Settings → Pages*, set **Branch: main** and **/ (root)**. Save.
4. Open the Pages URL after it builds. You should see the app.
5. Use the left panel to pick Week/Section and start a session.

### Data format

`full_eagle_word.js` must define `window.wordData` with the structure:

```js
window.wordData = [
  {
    week: 1,
    sections: [
      { type: "Reading Plus", story: "Mike's New Airplane", words: [
        { en: "airplane", zh: "飛機" },
        // ...
      ]}
    ]
  }
];
```

### Features

- Spelling, Multiple‑choice, Dictation (TTS), Flashcards
- Spelling tolerance (0/1/2 chars off still count)
- Wrong‑answer recycling and simple localStorage history
- Keyboard shortcuts: **Enter** submit, **Tab** next, **Ctrl/Cmd+.** speak

---

© 2025 Eagle Words
