# 🎲 Group Allocator

A lightweight, self-contained web app for randomly allocating students (or any list of names/items) into groups. Built for classroom use — no installation, no login, no internet connection required after the page loads.

**[Open Group Allocator →](https://ironstamp.github.io/group-picker)**

---

## Features

- **Manual name entry** — type names one at a time and add with Enter
- **Load sample** — fill in a set of example names to try it out
- **CSV import** — upload a `.csv` or plain text file, or drag and drop it onto the upload area
- **Flexible group settings** — set a target group size, or specify an exact number of groups
- **Remainder handling** — choose what happens when names don't divide evenly:
  - Spread remainders into existing groups (uneven sizes)
  - Create a separate smaller group
  - Leave remainders unallocated (listed separately)
- **Reveal mode** — hide all names after allocating, then click to reveal one at a time — great for dramatic effect in class
- **Re-shuffle** — re-randomise instantly with the same settings
- **Copy to clipboard** — paste the full group list into an email, Teams message, or document
- **Collapsible settings panel** — slide the sidebar away after setup for a clean full-screen group display

---

## Usage

1. Open the [live page](https://ironstamp.github.io/group-picker), or download `index.html` and open it in any modern browser — no server or installation needed
2. Add names manually or import a CSV file
3. Set your group size and remainder preference
4. Click **Allocate Groups**
5. Optionally collapse the sidebar for display purposes

---

## CSV Format

The app accepts:

- One name per line
- Comma- or semicolon-separated names on a single line
- A mix of both
- A header row containing the word "name" (this will be automatically skipped)

Duplicate names are skipped, so importing the same list twice won't double anyone up.

**Example:**
```
Name
Alice
Ben
Chloe, Daniel, Emma
Finn
```

---

## Deployment (GitHub Pages)

This is a single `.html` file with no dependencies beyond a Google Fonts stylesheet (loaded from the web). To host it:

1. Fork this repository (the app is `index.html`)
2. Enable GitHub Pages in your repo settings (Settings → Pages → Deploy from branch → `main`)
3. Access it at `https://<your-username>.github.io/group-picker/`

---

## Tech

Pure HTML, CSS, and vanilla JavaScript. No frameworks, no build step, no dependencies. The font ([DM Sans](https://fonts.google.com/specimen/DM+Sans) / [DM Serif Display](https://fonts.google.com/specimen/DM+Serif+Display)) is loaded from Google Fonts — the app still works offline, just with a fallback font.

---

## More classroom tools

- [Classroom Manager](https://ironstamp.github.io/classroom-tool): post, schedule and copy Google Classroom courses
- [Score Tracker](https://ironstamp.github.io/scoretracker): live projected scores with a countdown timer
- [Tarsia Puzzle Generator](https://ironstamp.github.io/tarsia-generator): printable triangle-matching puzzles
- [Domino Chain Puzzle Generator](https://ironstamp.github.io/domino-puzzle-generator): printable domino-chain matching cards

---

*Made by Paul Carter, mathematics teacher, New Zealand.*
