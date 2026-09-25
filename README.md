# Chao turns 40 ✦ Hong Kong · Shenzhen · Taipei

A fun, mobile-friendly itinerary site for a 40th birthday trip — 18 friends, 6 countries,
Oct–Nov 2026. Live countdown, the crew, an interactive map of everyone flying in, and the full
day-by-day plan.

> **To update the trip, edit [`data/itinerary.json`](data/itinerary.json) and push.**
> The rest of the site renders from it. See [`PROJECT.md`](PROJECT.md) for the full guide.

## Develop in VS Code
Open the folder in VS Code (`File → Open Folder…`, or `code .` from the terminal). On first open
it offers the recommended extensions in `.vscode/` — accept them. Then run the site any of these ways:

- **Live Server (easiest):** install the recommended *Live Server* extension, then click
  **Go Live** in the status bar (or right-click `index.html` → *Open with Live Server*). Opens at
  `http://localhost:5500`.
- **Run + debug:** press **F5** ("Run site (Chrome)") — starts a local server and opens Chrome with
  breakpoints enabled in `assets/app.js`.
- **Task only:** **Cmd+Shift+B** ("Serve site") starts `http://localhost:8000`; open it in any browser.

A local server is required (not just opening the file) because the page `fetch`es the JSON data.

If `code .` isn't recognised, in VS Code run **Cmd+Shift+P → "Shell Command: Install 'code' command in PATH"**.

## Run locally (no editor)
```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy (GitHub Pages)
1. Push to `main`.
2. Repo → **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main` / `/ (root)`.
3. Site goes live at the URL shown there. (Pages on a private repo needs GitHub Pro/Team/Enterprise;
   otherwise make the repo public to publish.)

## Stack
Static HTML/CSS/vanilla JS · [Leaflet](https://leafletjs.com) map · no build step.
