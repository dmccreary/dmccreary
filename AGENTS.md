# Repository Guidelines

## Project Structure & Module Organization
- `docs/` holds the MkDocs content (Markdown pages referenced by `mkdocs.yml`).
- `mkdocs.yml` is the site configuration and navigation.
- `site/` is the generated static site output (do not hand-edit).
- `slides/`, `podcasts/`, and `old-resumes/` contain supporting assets and archives.
- Root-level PDFs and `.pptx` files are source materials referenced from docs.

## Build, Test, and Development Commands
- `mkdocs serve` starts a local dev server with live reload.
- `mkdocs build` generates the static site into `site/`.
- `mkdocs build --strict` fails on broken links or invalid references (use before publishing).

## Coding Style & Naming Conventions
- Markdown is the primary format; prefer clear headings and short paragraphs.
- Use sentence case for headings and keep line lengths reasonable for readability.
- In `mkdocs.yml`, use 2-space indentation and keep navigation ordered and explicit.
- File names are lowercase with hyphens (e.g., `robot-labs.md`).

## Testing Guidelines
- No automated tests are defined in this repository.
- Use `mkdocs build --strict` as a basic validation step for docs changes.

## Commit & Pull Request Guidelines
- Commit history uses short, direct messages (e.g., "updating content"); keep messages concise.
- PRs should include a brief summary and note any navigation or content changes.
- Include screenshots for visible content/layout changes to the generated site.

## Security & Configuration Tips
- Avoid committing secrets or private data to `docs/` or asset folders.
- Keep `site/` in sync only via `mkdocs build` to avoid stale output.
