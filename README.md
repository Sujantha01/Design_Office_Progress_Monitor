[README.md](https://github.com/user-attachments/files/35418585/README.md)
# DESIGN OFFICE PROGRESS MONITOR — TV dashboard prototype
By Amila Sujantha

This standalone preview is NOT an integrated V3.04 update. All displayed numbers and workers are synthetic. The V3.04 ZIP was unavailable, so the precise columns, overview charts, filtering and data calculations are not verified. No database is accessed or modified.

## Preview
Open index.html directly, or run START_PREVIEW.cmd with Python available in PATH. Use F11 or Full screen. Overview and board alternate every 30 seconds. Board pages advance every 5 seconds; for large datasets multiple rotations may be needed. The prototype currently resets the page on each board visit, so more than six pages require a pagination improvement before production. A very long row may also exceed the viewport. Test at actual TV resolution and viewing distance.

## GitHub
Upload index.html, style.css, config.js, app.js, and .nojekyll to a GitHub repository. Configure GitHub Pages to deploy from the chosen branch and root. Do not publish confidential data, credentials, database files or real snapshots. The demo is safe for public preview. No repository has been created or deployed by this package.

## Private integration
Use an approved private HTTPS service or host this frontend on an internal office server. GitHub Pages cannot open a Windows network share or SQLite database, and HTTPS pages may block HTTP LAN requests. Set demo:false and dataUrl to an approved authenticated endpoint; for cross-origin use configure appropriate CORS and authentication (the included fetch only sends same-origin credentials). Prefer same-origin private hosting. Do not expose the database to the internet. The bridge must call the existing V3.04 overview and board data providers, using the same filters and ordering and no independent calculations. Export an atomic JSON snapshot with the structure in snapshot.schema.example.json. Verify against both desktop views. The bridge is not included because the application source/schema was unavailable.
