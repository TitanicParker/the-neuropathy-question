# The Neuropathy Question

A zero-build GitHub Pages manuscript reader following the TitanicParker publication format.

## Repository structure

This publication uses three top-level files:

- `index.html` — landing page, cover art, Markdown renderer, listening controls, sharing, counters, and reading/listening progress.
- `manuscript.md` — the manuscript content.
- `README.md` — maintenance and publication notes.

## Manuscript workflow

Replace the contents of `manuscript.md` when the manuscript is ready.

The reader fetches `./manuscript.md` from the same repository at runtime, converts it from Markdown to HTML, sanitizes it, and builds narration blocks from rendered headings, paragraphs, and list items.

Recommended structure:

```md
# The Neuropathy Question

## Chapter or major section

Normal prose paragraph.

### Subheading

More prose.
```

The first `#` heading becomes the visible title and browser title.

## Hosting

The site is static and ready for GitHub Pages from the repository root on the `main` branch.

No package install, build step, server, or database is required.
