# Repository-specific instructions for AI coding agents

This is a small, static portfolio template used for DCDA 40833 student projects. The goal of an AI coding agent here is to be immediately productive with minimal setup.

- **Big picture:** a static site built from plain HTML/CSS with images and example lab pages. No build system, package manager, or server-side code.
- **Primary files:** `index.html`, `css/styles.css`, `images/` (assets), `README.md`, `EDITING_GUIDE.md`.

Key guidance (concise, actionable):

1. Preserve the template structure. Edit page content only; do not remove the navigation or global layout in `index.html`.

2. TODO markers: content insertion points are marked with HTML comments like <!-- TODO: ... -->. Search for the string `TODO` to locate editable regions.

3. Naming & navigation:
   - Page filenames follow predictable names: `ai-evaluation.html`, `tufte-critique.html`, `tableau-visualization.html`, `lab5.html`, `hometown-map.html`.
   - When adding pages, update the site navigation on every page (copy `<nav>` from `index.html`).

4. Assets & paths:
   - Put images in `images/` and reference them with relative paths (e.g., `images/Profile.png`). Filenames are case-sensitive.
   - Embed Folium maps by adding the exported HTML to the repo and referencing via an `<iframe>`.
   - Tableau embeds are external iframes; ensure the published Tableau URL is public.

5. CSS conventions:
   - Theme variables live at the top of `css/styles.css` under `:root` (e.g., `--primary-color`). Prefer changing variables instead of editing many rules.
   - Keep responsiveness and grid classes; most layout is controlled via `styles.css`.

6. Developer workflow (no build/test):
   - Local preview: open `index.html` in a browser (no server required for basic pages). For iframe-embedded HTML files, preview from the repo root in a browser.
   - Git flow: `PULL → EDIT → SAVE → PREVIEW → COMMIT → PUSH`. The README and EDITING_GUIDE document this precisely.
   - Deployment: use GitHub Pages (Settings → Pages → branch: `main` or `master`, folder: `/ (root)`). Allow 1–2 minutes after enabling.

7. What not to do:
   - Do not introduce build tools, bundlers, or frameworks—this repo is intentionally simple.
   - Avoid changing semantic structure (header, nav, main, footer) unless the user asks for a redesign.

8. Helpful examples from this repo:
   - Where to inject content: see `index.html` sections `<!-- TODO: ... -->`.
   - CSS variables: open `css/styles.css` and edit the `:root` block for color changes.
   - Footer repo link: update the GitHub link in the footer to match the user's repo.

9. When in doubt, follow `EDITING_GUIDE.md` and `README.md` — they contain the user-facing workflow, examples, and deployment steps.

If any section is unclear or you'd like the agent to follow stricter rules (e.g., auto-creating lab pages), tell me what to enforce and I'll update this file.
