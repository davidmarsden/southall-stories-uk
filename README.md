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
- `static/css/southall-refresh.css` — homepage/article refresh styles
- `static/css/southall-browse.css` — archive/category styles
- `static/css/southall-pages.css` — supporting page styles
- `static/custom.css` — older Southall Stories overrides still in use
- `static/css/style.css` — inherited theme stylesheet
- `_variables-light.scss` / `_variables-dark.scss` — theme colour/type variables
- `config.json` — exported Micro.blog/Hugo configuration snapshot
- `docs/about-page.md` — canonical refreshed About page copy for Micro.blog

## Workflow

1. Make and review changes here.
2. Copy the changed files into the Southall Stories custom theme in Micro.blog.
3. Rebuild and check the live site.
4. Keep GitHub and Micro.blog in sync.

## 2026 redesign status

The refresh is moving Southall Stories from a chronological-blog presentation toward a stronger independent local-publication identity.

Completed first-pass work:

- Editorial homepage with lead investigation, latest stories, reporting beats and Civic Commons feature.
- Compact publication masthead and clearer navigation.
- Publication-style article pages with improved typography, metadata, sharing, support and conversation routes.
- Category pages with visual story cards.
- Year-by-year archive with jump navigation and category links.
- First-pass styling for supporting publication pages.
- Decision to retire the overlapping `Read Me` page and consolidate trust/start-here information into a stronger `About Southall Stories` page. Preserve `/read-me/` with a Micro.blog redirect to `/about/`.
- Refreshed About page copy stored in `docs/about-page.md`.

## Polish backlog

Keep these for later refinement rather than interrupting the structural redesign:

- Fine-tune homepage left-rail spacing/alignment.
- Revisit lead-story image/copy balance after more real-world use.
- Consider curated/featured lead-story selection instead of always using the newest post.
- Reduce visual noise from very long category/tag strings in archive rows.
- Improve card rhythm where portrait/tall images create uneven category-page layouts.
- Continue softening the article left rail on very long reads if it still feels visually dominant.
- Continue styling the Micro.blog conversation form so it feels more native to the publication design.
- Review mobile/tablet behaviour of the floating topic/category control.
- Review About page copy after it has been live for a while, including the final preferred contact address.
- Develop the fuller Southall Stories identity system later: compact mark, favicon, social card, horizontal wordmark and possible simplification/removal of the old quill motif.

## Redesign direction

Southall Stories should feel like an independent local investigative publication: lead investigations, clearer editorial sections, strong archives and research routes, accessible supporting pages, and a distinct but connected presentation of Ealing Civic Commons. The yellow, real Southall photography and slightly irreverent character should remain part of the identity rather than being polished into a generic news-site look.
