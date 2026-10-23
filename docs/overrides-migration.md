# Overrides migration acceptance checklist

- [ ] Confirm upstream Microwave version and file-level baseline.
- [ ] Record exact file ownership: Southall, Microwave, or independent Micro.blog plugin.
- [ ] Audit and minimise changes to `baseof.html`, `head.html`, `style.css`, `custom.css` and `search.js`.
- [ ] Verify menu opens, closes, follows links, Escape works and ARIA state matches.
- [ ] Verify homepage, post pages, categories, archive and support pages at mobile and desktop widths.
- [ ] Verify search, OpenGraph metadata, images, newsletter and plugin features.
- [ ] Verify light and dark palettes, fonts, links and contrast.
- [ ] Install on a test Micro.blog site; inspect generated HTML and asset load order.
- [ ] Document any differences and fix them before changing the production theme.
- [ ] Keep current Micro.blog theme export as rollback snapshot.
- [ ] Only after acceptance, enable on Southall Stories and remove duplicate custom-theme overrides incrementally.
