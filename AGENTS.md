# AGENTS.md

## Cursor Cloud specific instructions

This is a static HTML site (`index.html`) with no build step, no package manager, and no runtime dependencies.

- **Run locally:** `python3 -m http.server 8000` from the repo root, then open `http://localhost:8000/`.
- **Lint / test / build:** There are no lint, test, or build commands. The project has no `package.json`, no CSS/JS preprocessors, and no CI checks beyond the GitHub Pages deployment workflow.
- **Deployment:** Handled automatically by `.github/workflows/pages.yml` on push to `main`. See `README.md` for GitHub Pages configuration details.
