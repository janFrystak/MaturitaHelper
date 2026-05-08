# MaturitaHelper

Local HTML catalogue for maturita study notes. No server, no build step — just open `index.html` in Chrome/Edge.

## Structure

```
Helper/
├── index.html          # Main catalogue
├── practice.html       # Practice / answer drill page
├── manifest.js         # List of note files per subject ← edit this when adding notes
├── note-template.html  # Template for creating new notes
└── notes/
    ├── EKO/            # Ekonomika
    ├── IT/             # Informační technologie
    └── LIT/            # Literatura
```

## Adding a new note

1. Create the note from `note-template.html` — set the three meta tags:
   ```html
   <meta name="mat-subject" content="eko">   <!-- eko | it | lit -->
   <meta name="mat-num"     content="7">
   <meta name="mat-title"   content="Název otázky">
   ```
2. Save it as `NN_Nazev_otazky.html` in the correct subject folder
3. Add the filename to `manifest.js`
4. Reload `index.html` — the note appears automatically

## Features

- Browse notes by subject (EKO / IT / LIT) with a progress bar
- Flag whole notes or individual sections as problematic (stored in `localStorage`)
- Dark mode (synced across catalogue and open notes)
- Practice page — write answers per question, track status (not started / in progress / done)
- Custom practice questions

## Subject totals

| Subject | Questions |
|---------|-----------|
| Ekonomika | 20 |
| Informační technologie | 20 |
| Literatura | 20 |

---

ITE 4.B · Maturita 2025/2026
