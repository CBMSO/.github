# CBMSO/.github

This repository holds organisation-wide content for
[CBMS — Computational Biomedical Systems](https://github.com/cbmso).

## What lives here

| Path             | Purpose                                                                 |
| :--------------- | :----------------------------------------------------------------------- |
| `profile/README.md` | The public organisation profile rendered on the [org page](https://github.com/cbmso). Edit **this** file to change how the lab presents itself. |
| `profile/logo.svg` | The lab logo used by the profile. Byte-identical to `src/app/icon.svg` in the website repo. |

Nothing here is built or released. The website is deployed separately from its own
repository — see [cbmslabs.pages.dev](https://cbmslabs.pages.dev).

## Notes for maintainers

- The profile logo is a real SVG (`profile/logo.svg`), versioned here rather than
  hot-linked, so it can never be served as a raster. When the website's
  `src/app/icon.svg` changes, copy it over to keep the two in sync.
- Keep the profile's research tracks and capabilities consistent with the website
  copy; they currently mirror `src/lib/research-tracks.ts` and the services page.