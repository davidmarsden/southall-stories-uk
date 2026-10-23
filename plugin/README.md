# Southall Stories overrides — integration candidate

This directory is the **plugin package root** (its `plugin.json` belongs at the root of an installed plugin, not in the parent repository root). It is not yet installed or validated on Micro.blog.

## Ownership and dependencies

Microwave remains the base theme. This plugin owns the customised editorial layouts (`index.html`, `post/single.html`, `_default/single.html`, `_default/taxonomy.html`, archive layouts), the overall `baseof.html`, Southall `head.html`, mobile navigation, supporting partials, branding stylesheets, and legacy `style.css` / `custom.css` retained for visual fidelity. `_variables-light.scss` preserves the original light-mode Sass configuration. `search.js` and standard Microwave assets are expected to come from the installed base theme unless explicitly overridden.

The Southall `head.html` already links the four Southall stylesheets. Therefore the manifest has `includes: []` to avoid duplicate CSS requests. The Southall `baseof.html` references `js/hamburger.js`, and the paired mobile-nav partial is packaged alongside it.

**Excluded:** site `config.json`, generated content, Micro.blog account data, SocialSpec, Search Space, Collections and other independently managed plugin files.

## Dependencies still to verify before installing

1. Confirm the installed Microwave version and exact upstream layout/asset resolution, including inherited `sidebar`, `sidemeta`, `social-icons`, standard JavaScript and Bootstrap styles.
2. Confirm Micro.blog accepts an installed plugin with `baseof.html` and `head.html` overrides while keeping Microwave as the base theme.
3. Check whether the plugin's light-mode Sass variable override compiles as expected; if not, move the palette into explicit CSS.
4. Compare `style.css` and `custom.css` with pristine upstream Microwave and reduce duplicated inherited code after visual parity is established.
5. Verify homepage, articles, categories, archive, search, social previews, navigation, colour schemes and third-party plugin integrations on a test site.

## Deployment / rollback

Install the contents of **this directory** as a Micro.blog plugin on a test site first. Do not install the repository root as a plugin. Keep the existing custom theme and export intact. On failure, disable the plugin, restore the original theme configuration and rebuild.

See `../docs/asset-comparison.md` and `../docs/overrides-migration.md`.
