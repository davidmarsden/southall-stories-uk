# Asset comparison — Southall Stories vs davidmarsden-test

Source: Micro.blog exports supplied 23 October 2026. The reference is Microwave-derived, **not verified pristine upstream Microwave**. The original detailed inventory is retained in the conversation as `southall-asset-comparison.txt`; this document records the migration decisions.

| Class | Identical | Modified | Southall-only |
| --- | ---: | ---: | ---: |
| CSS and JavaScript | 8 | 7 | 9 |

## CSS

- Identical: `static/css/hamburgers.css`, `loader.css`, `photoswipe.css` — inherit.
- Near-identical: `bootstrap-light.css`, `bootstrap-dark.css` — inherit only after verifying palette and Sass effects.
- Modified: `static/css/style.css` (729 vs 471 lines) and `static/custom.css` (145 vs 220 lines) — extract intentional Southall rules; do not replace wholesale without visual checks.
- Southall-only: `static/css/southall-refresh.css`, `southall-browse.css`, `southall-pages.css`, `southall-identity.css` — plugin-owned.
- `static/css/collections.css` — leave to Collections.

## JavaScript

- Identical: `archive.js`, `lastfm.js`, `lightbox.js`, `masonry.js` — inherit.
- Modified: `hamburger.js` (working mobile navigation) — plugin-owned together with HTML partial.
- Modified: `search.js` (187 vs 153 lines) — preserve defensive changes pending ownership audit.
- Southall-only: `studio.js`, `search-space/application.js`, `search-space/minisearch.js` — third-party ownership; exclude.

## Sass and configuration

- `_variables-dark.scss`, `theme.toml` identical — inherit.
- `_variables-light.scss` modified: brand colours, page background, fonts and rounded corners — preserve visual effects with targeted CSS if feasible.
- `config.json` is generated/site-specific — exclude.
- Exported `plugin.json` describes SocialSpec on Southall and Microwave on the reference — **do not reuse either**.

## Risk and constraints

CSS load order, Hugo template precedence, duplicate plugin-provided layouts, and inherited theme updates are unresolved. Do not install the staging package on the live site until validated.
