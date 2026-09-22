# Local Text Anonymizer & De-ID Tool

A zero-dependency, single-file local web application for de-identifying support tickets, technical documentation, and internal communications. Fully privacy-compliant—all text processing runs 100% client-side in your browser with no server requests or data transmission.

## ✨ Features

- **Privacy-First & Offline Ready:** Completely standalone HTML/JS application. No backend required.
- **Multiple Anonymization Modes:**
  - **Partial Initials Mode (`-p`):** Replaces names with clean initials (e.g., `Alex Miller` -> `A.M.`). Adds a deterministic 3-character hash suffix only when collisions occur (e.g., `A.M._a1f`).
  - **Standard Mode:** Replaces identities with sequential tokens (e.g., `[User_1]`, `[User_2]`).
- **Smart Grammar & Formatting Support:**
  - Handles case-insensitivity and irregular spacing.
  - Automatically handles possessives (e.g., `Alex's` -> `A.M.'s`).
  - Matches single first/last name occurrences across the text to the same mapped entity.
- **Live Visual Highlighting:**
  - Highlights detected names in the Input box in real time.
  - Highlights replaced anonymized tokens in the Output box.
- **Synchronized Split Views:**
  - Simultaneous bi-directional vertical and horizontal scrolling.
  - Synchronized selection across input and output fields.
  - Toggleable Horizontal (side-by-side) and Vertical (stacked) layouts with a draggable resizable splitter.
- **Audit & Reversal Mapping:** Generates a real-time JSON mapping table for compliance tracking and potential de-anonymization audits.
- **Quick Controls & Customization:**
  - Integrated utility tools: Copy, Paste, Clear, Undo, Redo.
  - Customizable editor typography (Font Family & Font Size selection, featuring JetBrains Mono by default).
  - Collapsible header dictionary input saved locally via `localStorage`.

## 🚀 Quick Start

1. Download or clone `index.html`.
2. Double-click `index.html` to open it in any modern web browser.
3. Paste your text into the **Input Text** pane to see immediate anonymization results!

## 📄 License

MIT License
