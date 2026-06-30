# Forge — JSON, shaped.

A single-file, no-build JSON formatter/validator/viewer. Works entirely in the
browser — nothing is sent to a server, so it's safe to use on private data.

## Features

- **Paste, upload, or fetch** — paste JSON directly, drag a `.json` file onto
  the input panel, or fetch one from a URL (subject to that server's CORS
  policy).
- **Live validation** — errors are reported with the exact line and column.
- **Formatted view** — syntax-highlighted, line-numbered, with colored
  nesting-depth guides on the left edge so deep structures stay readable.
- **Tree view** — collapsible, expand/collapse all, click any key to copy its
  JSON path (e.g. `root.owner.contact`).
- **Stats view** — file size, line count, total keys, max depth, and a
  breakdown of value types.
- **Controls** — 2/4-space or tab indent, minify, sort keys alphabetically,
  unescape a JSON-as-string payload, and a live search that filters the tree
  and highlights matching lines in the formatted view.
- **Copy & download** — one click to copy the formatted text or download it
  as `formatted.json`.
- **Light/dark theme**, keyboard shortcuts (`Ctrl/Cmd+Enter` to reformat,
  `Ctrl/Cmd+S` to download, `Esc` to clear search), and a responsive layout
  that stacks on mobile.

## Deploy to GitHub Pages

1. Create a new repository (or use an existing one) and add `index.html` to
   the root — e.g. for a project page, or to the root of a repo named
   `<username>.github.io` for a user/org page.
2. Commit and push:
   ```bash
   git add index.html
   git commit -m "Add Forge JSON formatter"
   git push
   ```
3. In the repo, go to **Settings → Pages**, set **Source** to "Deploy from a
   branch", pick `main` and `/ (root)`, then save.
4. Your formatter will be live at `https://<username>.github.io/<repo>/`
   (or `https://<username>.github.io/` for a user/org page) within a minute
   or two.

No build step, no dependencies to install — it's a static file.
