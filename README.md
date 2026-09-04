# Southall Stories

Canonical source repository for the custom Micro.blog theme used at **southallstories.uk**.

## Purpose

This repository is the working source of truth for the Southall Stories site design and Hugo/Micro.blog templates. Changes are developed here first, then copied into the corresponding custom-theme files in Micro.blog.

The separate `davidmarsden/southall` repository is the generated/public-site mirror and should not be used as the primary place to edit the theme.

## Initial source

The initial theme source was exported from Micro.blog on 4 September 2026. The repository is being seeded with the custom templates, configuration and styling that materially define the site. Micro.blog-generated content, newsletters, bookshelves, collections and other account/export data are intentionally excluded from this source repository.

## Main files

- `layouts/index.html` — editorial homepage
- `layouts/_default/baseof.html` — overall page shell
- `layouts/_default/single.html` — supporting publication pages
- `layouts/_default/taxonomy.html` — category pages
- `layouts/list.archivehtml.html` / `layouts/_default/list.archivehtml.html` — archive
- `layouts/post/single.html` — article pages
- `layouts/partials/` — masthead, navigation and supporting components
- `layouts/partials/head.html` — metadata, favicon and social-preview defaults
- `static/css/southall-refresh.css` — homepage/article refresh styles
- `static/css/southall-browse.css` — archive/category styles plus cross-site polish
- `static/css/southall-pages.css` — supporting page styles
- `static/css/southall-identity.css` — final identity-system refinements
- `static/custom.css` — older Southall Stories overrides still in use
- `static/css/style.css` — inherited theme stylesheet
- `_variables-light.scss` / `_variables-dark.scss` — theme colour/type variables
- `docs/about-page.md` — canonical refreshed About page copy for Micro.blog
- `docs/campaigns-page.md` — canonical Campaigns/resources copy
- `docs/search-page.md` — Search Space greeting copy
- `docs/subscribe-page.md` — refreshed Subscribe copy
- `docs/local-links-page.md` — Local links & resources page copy
- `docs/identity-system.md` — agreed identity rules and usage notes

## Workflow

1. Make and review changes here.
2. Copy the changed files into the Southall Stories custom theme in Micro.blog.
3. Rebuild and check the live site.
4. Keep GitHub and Micro.blog in sync.

## 2026 redesign status

The refresh has moved Southall Stories from a chronological-blog presentation toward a stronger independent local-publication identity.

Completed work includes:

- Editorial homepage with lead investigation, latest stories, reporting beats and Civic Commons feature.
- Compact publication masthead and clearer navigation.
- Publication-style article pages with improved typography, metadata, sharing, support and conversation routes.
- Category pages with visual story cards.
- Year-by-year archive with jump navigation and cleaner category metadata.
- Supporting publication pages refreshed and restyled: About, Campaigns, Search, Subscribe and Local links & resources.
- `Read Me` retired in favour of About, with `/read-me/` preserved via Micro.blog redirect.
- Global site credits for Micro.blog, Search Space by Sven Dahlstrand and the Microwave theme by Josh Dawson.
- Second-pass polish to sidebar rhythm, homepage lead balance, article heading spacing, conversation form styling, archive tag noise, mobile topic control and image-less category cards.
- Final identity system agreed and wired into the theme.

## Identity system

- Masthead: yellow/black **SOUTHALL STORIES**.
- Descriptor: **Independent local journalism**.
- Main strapline: **Recording what happens to Southall — and who is responsible.**
- Short line: **Local people. Local questions.**
- Character line: **Digging the dirt, unearthing the truth.**
- Easter egg: **As read by Ealing Council’s Press Office**.
- Favicon/site icon: original Southall Gasworks **No unauthorised access** image.
- Default social-preview image: the same original Gasworks sign image; article pages override it with their own lead image where available.
- No `SS` monogram.
- Old quill motif retired from the core identity.

## Remaining polish backlog

Keep these for later review rather than changing things just for the sake of it:

- Consider curated/featured lead-story selection instead of always using the newest post.
- Review homepage lead proportions again after more real-world use.
- Review About copy after it has been live for a while.
- Check category-card image crops on a wider sample of older posts and adjust individual source images only where necessary.
- Revisit the mobile/tablet topic drawer after using the site on phones for a while.

## Redesign direction

Southall Stories should feel like an independent local investigative publication: lead investigations, clearer editorial sections, strong archives and research routes, accessible supporting pages, and a distinct but connected presentation of Ealing Civic Commons. The yellow, real Southall photography and slightly irreverent character should remain part of the identity rather than being polished into a generic news-site look.
