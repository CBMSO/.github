# CBMSO/.github

This repository holds organisation-wide content for
[CBMS — Computational Biomedical Systems](https://github.com/cbmso).

## What lives here

| Path             | Purpose                                                                 |
| :--------------- | :----------------------------------------------------------------------- |
| `profile/README.md` | The public organisation profile rendered on the [org page](https://github.com/cbmso). Edit **this** file to change how the lab presents itself. |
| `profile/cbms-logo.svg` | The lab logo used by the profile. Same artwork as `src/app/icon.svg` in the website repo (identical `viewBox`, `d` and `fill`), plus explicit `width`/`height` — see below. |

Nothing here is built or released. The website is deployed separately from its own
repository — see [cbmslabs.pages.dev](https://cbmslabs.pages.dev).

## Notes for maintainers

- The profile logo is a real SVG (`profile/cbms-logo.svg`), versioned here rather than
  hot-linked, so it can never be served as a raster. When the website's
  `src/app/icon.svg` changes, copy it over to keep the two in sync.
- **Do not put `width`/`height` on the `<img>` tag** in `profile/README.md`.
  GitHub responds to a sized markdown image by adding `js-gh-image-fallback`,
  which paints `background-color: var(--bgColor-muted)` with a `6px` radius —
  a grey tile that reads as a box around the mark. Inline `style` and
  `<style>` blocks are both stripped, so it cannot be overridden. Leave the
  `<img>` unsized and let the SVG's own `width`/`height` set the size.
- Keep the profile's research tracks and capabilities consistent with the website
  copy; they currently mirror `src/lib/research-tracks.ts` and the services page.