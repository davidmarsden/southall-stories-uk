# Southall Stories overrides — staging package

**Not installed.** This folder is a candidate Micro.blog plugin, not a replacement for the Microwave theme. Keep the live custom theme unchanged until preview verification.

## Base and ownership

- **Microwave** remains the base theme and owns inherited layouts, Bootstrap, standard scripts and Sass compilation.
- **Southall Stories** owns editorial templates, masthead/navigation, four dedicated stylesheets and the tested hamburger script.
- **Micro.blog** owns content, site settings, uploads and generated config.
- **Other plugins** own Search Space, SocialSpec, Collections, conversations and reply-by-email components.

## Staged files

The four dedicated CSS files and paired mobile navigation HTML/JS are copied from the repository's known source. The existing custom theme remains authoritative until plugin installation is tested. The manifest's `includes` only lists the four dedicated stylesheets; the mobile nav script is loaded by the existing base template, and must be checked on a preview with the plugin enabled.

## Blockers before enabling

1. Compare against pristine upstream Microwave, not only the davidmarsden-test export.
2. Decide whether the site's customised `baseof.html`, `head.html`, homepage, articles, archives and taxonomy layouts should be included as exact overrides. The staging package intentionally does **not** override them yet.
3. Extract Southall-only changes from `static/css/style.css` and `static/custom.css`, preserve light/dark palette, and check CSS load order.
4. Confirm Micro.blog resolves the plugin's `layouts/partials/mobile-nav.html` and `static/js/hamburger.js` as expected.
5. Compare mobile and desktop pages, archive, search, metadata, and both colour schemes before cutover.
6. Remove duplicate custom-theme files only **after** passing preview tests and documenting rollback.

## Rollback

Disable the plugin and rebuild the existing custom theme. Do not delete any live theme overrides during staging.

See [asset inventory](../docs/asset-comparison.md) and [migration checklist](../docs/overrides-migration.md).
