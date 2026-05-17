# CV Creator

A single-file, browser-based CV editor with live preview and PDF export. No installation, no server, no dependencies — just open `cv-creator.html` and start editing.

## Features

- **Live preview** — changes appear instantly in the CV preview
- **Multilingual UI** — editor interface available in multiple languages
- **Multilingual CV content** — enter skills, hobbies, and other fields in multiple languages; the CV renders in the selected language
- **Sections**: Personal info, Work experience, Education, Skills, Languages, Certifications, Hobbies
- **Photo upload** — drag & drop or click to upload a profile photo with position/size controls
- **Color themes** — choose from preset themes or customize individual colors
- **Font size & spacing controls** — fine-tune typography for each CV section
- **JSON export / import** — save your CV data to a `.json` file and reload it later
- **PDF export** — print-ready layout via the browser's print dialog

## Usage

1. Open `cv-creator.html` in any modern browser (Chrome, Edge, Firefox)
2. Edit your details in the left panel
3. Preview updates in real time on the right
4. Export as PDF via **Print → Save as PDF**, or save your data with **Export JSON**

## Data Format

CV data is stored as a structured JSON file (see `max_mustermann_cv.json` for an example). The file can be imported back into the editor at any time.

```json
{
  "version": 2,
  "language": "de",
  "cv": {
    "personal": { ... },
    "skills": { ... },
    "languages": [ ... ],
    "certifications": [ ... ],
    "hobbies": { ... },
    "experience": [ ... ],
    "education": [ ... ]
  }
}
```

## Files

| File | Description |
|------|-------------|
| `cv-creator.html` | The full application — editor + preview + export |
| `max_mustermann_cv.json` | Example CV data (Max Mustermann) |

## Browser Support

Works in any modern browser. PDF export relies on the browser's native print-to-PDF — no plugins required.
