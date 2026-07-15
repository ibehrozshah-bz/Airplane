# AeroDesk — Airplane Management System

A responsive airline operations front-end built with **HTML5, CSS3, and Bootstrap 5**, covering four screens: **Home Dashboard**, **Ticket Management**, **Departures**, and **Arrivals**.

## Live demo
Open `index.html` directly in a browser, or serve the folder with any static server. No build step or backend is required — all data on screen is sample/mock data for demonstration.

## Features
- Fixed, professional sidebar navigation (collapses to an off-canvas menu on tablet/mobile) with active-page highlighting
- Sticky topbar with global search, notification icon, live clock, and profile avatar
- Four full pages:
  - **Home Dashboard** — KPI stat cards, weekly traffic mini-chart, fleet status, recent ticket activity, next departures
  - **Ticket Management** — ticket stats, searchable/filterable table, "New Ticket" modal form
  - **Departures** — live departure board with gate chips, aircraft, scheduled/estimated time, status pills, search + status filter
  - **Arrivals** — live arrivals board with the same interaction pattern as Departures
- Reusable status "pill" components (Confirmed / Pending / Cancelled / On Time / Delayed / Boarding / Landed / Departed)
- Client-side table search and status filtering (`assets/js/script.js`) — no frameworks, plain JavaScript
- Attractive multi-column footer with quick links, contact details, and social icons
- Fully responsive layout (desktop, tablet, mobile) built on the Bootstrap 5 grid plus custom CSS
- Accessible focus states and `prefers-reduced-motion` support

## Tech stack
| Layer      | Choice                                   |
|------------|-------------------------------------------|
| Markup     | Semantic HTML5                            |
| Styling    | Bootstrap 5.3 (CDN) + custom `assets/css/style.css` design system |
| Icons      | Bootstrap Icons (CDN)                     |
| Fonts      | Space Grotesk (display) + Inter (body), Google Fonts |
| Behaviour  | Vanilla JavaScript (`assets/js/script.js`) |

## Folder structure
```
airplane-management-system/
├── index.html          # Home Dashboard
├── tickets.html         # Ticket Management
├── departures.html      # Departures
├── arrivals.html        # Arrivals
├── assets/
│   ├── css/
│   │   └── style.css    # design tokens, sidebar, cards, tables, footer
│   └── js/
│       └── script.js    # sidebar toggle, live clock, search & filters
└── README.md
```

## Running locally
No installation needed.
```bash
# Option 1: just open the file
open index.html          # macOS
start index.html         # Windows

# Option 2: serve it (recommended for consistent relative paths)
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Uploading to GitHub
```bash
cd airplane-management-system
git init
git add .
git commit -m "Airplane Management System — initial submission"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo-name>.git
git push -u origin main
```
Then submit the repository link, e.g. `https://github.com/<your-username>/<your-repo-name>`.

Optional: enable **GitHub Pages** (Settings → Pages → Deploy from branch → `main` / root) to also share a live URL alongside the repo link.

---
Submitted: 15 July 2026
