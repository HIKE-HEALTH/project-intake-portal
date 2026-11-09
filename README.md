# Project Intake Portal

A single-page portal that runs a project intake & prioritization process:

Business Leader (SBAR) → EPMO completeness review → SBAR Committee (project required?) → Project Manager (business case) → Project Governance (approve + weighted score) → Portfolio roadmap.

## Run it

Open `index.html` in a browser, or enable GitHub Pages (Settings → Pages → Deploy from branch → `main` / root) and visit the published URL.

## Storage

When hosted on claude.ai as an Artifact, requests are stored in a shared database so every role sees the same queue.
When hosted anywhere else (GitHub Pages, a local file), the page falls back to the browser's local storage, so each person sees only the requests created in their own browser. To share data outside claude.ai you would add a small backend (e.g. Firebase, Supabase) in place of the `db` calls in `index.html`.
