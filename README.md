# Southall Stories

Canonical source repository for the custom Micro.blog theme used at **southallstories.uk**.

## Purpose

This repository is the working source of truth for the Southall Stories site design and Hugo/Micro.blog templates. Changes are developed here first, then copied into the corresponding custom-theme files in Micro.blog.

The separate `davidmarsden/southall` repository is the generated/public-site mirror and should not be used as the primary place to edit the theme.

## Initial source

The initial theme source was exported from Micro.blog on 4 September 2026. The repository is being seeded with the custom templates, configuration and styling that materially define the site. Micro.blog-generated content, newsletters, bookshelves, collections and other account/export data are intentionally excluded from this source repository.

## Main files

- `layouts/index.html` — homepage
- `layouts/_default/baseof.html` — overall page shell
- `layouts/post/single.html` — article pages
- `layouts/partials/` — masthead, navigation and supporting components
- `static/custom.css` — Southall Stories custom overrides
- `static/css/style.css` — theme stylesheet
- `_variables-light.scss` / `_variables-dark.scss` — theme colour/type variables
- `config.json` — exported Micro.blog/Hugo configuration snapshot

## Workflow

1. Make and review changes here.
2. Copy the changed files into the Southall Stories custom theme in Micro.blog.
3. Rebuild and check the live site.
4. Keep GitHub and Micro.blog in sync.

## Redesign direction

The 2026 refresh is intended to move Southall Stories from a chronological-blog presentation toward a stronger independent local-publication identity: lead investigations, clearer editorial sections, better archives and research routes, and a distinct but connected presentation of Ealing Civic Commons.
