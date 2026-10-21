# APEX DEV · Session 3

Static, build-free presentation site for the APEX DEV workshop (Session 3).

## Pages

- `index.html` — landing page, choose a view
- `presenter.html` — presenter view (English notes + slide preview, two-pane layout)
- `broadcast.html` — broadcast view (full-screen slides for projection)

## Notes

- No backend, no database, no build step. Everything (fonts via CDN, images as embedded data) is self-contained in each HTML file.
- The editable site-name fields on the first slide save to the visitor's own browser via `localStorage`; nothing is sent to a server.

## Deploy

Any static host works with zero configuration. For Vercel:

1. Import this GitHub repository in the Vercel dashboard.
2. Framework preset: **Other** (no build command, no output directory needed).
3. Deploy — `index.html` is served at the project's root URL automatically.
