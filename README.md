# Correspondence Register (Daftar Persuratan)

A lightweight tracker for government correspondence — **minutes, memos, and letters**. Built as a single, self-contained HTML page with no build step and no server.

## Features

- **Register table**, grouped by **month** (earliest → latest), with columns:
  Month · Title · From · To · Date · Attachments · Document · Reference · Drafted By · Category
- **Inline editing** — click any cell to edit. Month, Document, Drafted By, and Category are dropdowns; dates use a date picker.
- **Reference & Slogan control panel** — track the last reference used, the next reference, the current slogan, and the next slogan (all editable, auto-saved).
- **Filters & search** — by category (BSP / RBA / BDIS / EAP), month, document type, and free-text search.
- **Summary by category** — record counts per category.
- **Drafter tags** — RS (pink), MH (green), RJ (orange).
- **Light / dark theme** toggle.
- **New Entry** form, and per-row delete.

## Data storage

All data is saved in the **browser's `localStorage`** on the device you use — nothing is sent to a server. This makes it free and private, but it means the register is **per-device and per-browser**: it does not sync between people or machines. Clearing site data will erase the records.

To share one register across several officers, the app would need a small backend or hosted database — see "Next steps" below.

## Running it

Just open `index.html` in any modern browser, or visit the published GitHub Pages site.

## Next steps (optional)

- Export / import records as a JSON or CSV file (backup & transfer).
- A shared backend so multiple users see the same register.
- Printable / PDF view of a month's entries.
