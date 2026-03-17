# 🎲 Group Allocator

A lightweight, self-contained web app for randomly allocating students (or any list of names/items) into groups. Built for classroom use — no installation, no login, no internet connection required after the page loads.

---

## Features

- **Manual name entry** — type names one at a time and add with Enter
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

1. Download `group-allocator.html`
2. Open it in any modern browser — no server or installation needed
3. Add names manually or import a CSV file
4. Set your group size and remainder preference
5. Click **Allocate Groups**
6. Optionally collapse the sidebar for display purposes

---

## CSV Format

The app accepts:

- One name per line
- Comma-separated names on a single line
- A mix of both
- A header row containing the word "name" (this will be automatically skipped)

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

1. Add `group-allocator.html` to your GitHub repository
2. Enable GitHub Pages in your repo settings (Settings → Pages → Deploy from branch → `main`)
3. Access it at `https://<your-username>.github.io/<your-repo>/group-allocator.html`

---

## Part of the Teacher Toolkit

This app was built alongside the [Score Tracker](./index.html) — a classroom score tracking tool. More tools may be added over time.

---

## Tech

Pure HTML, CSS, and vanilla JavaScript. No frameworks, no build step, no dependencies. The font ([DM Sans](https://fonts.google.com/specimen/DM+Sans) / [DM Serif Display](https://fonts.google.com/specimen/DM+Serif+Display)) is loaded from Google Fonts — the app still works offline, just with a fallback font.
