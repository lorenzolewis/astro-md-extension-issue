# Astro MD Link Issue

There are 2 issues here related to parsing relative links in markdown files and their rendered urls:

1. If the `.md` extension is included in a link FROM a markdown document TO another markdown document, that link results in a 404 as it keeps the `.md` extension in the `a` tag of the source page
2. If the links are relative (i.e. `[app](app.md)` instead of `[app](./app.md)` or `[app](/app.md)`), the source page URL links to the base directory and not relative from that page.
