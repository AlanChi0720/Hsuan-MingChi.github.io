# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a static personal portfolio website for Hsuan-Ming Chi, built on the "Massively" template by HTML5 UP. It is deployed as a GitHub Pages site (`Hsuan-MingChi.github.io`). There is no build system, package manager, or server-side code.

## Serving Locally

Open any `.html` file directly in a browser, or use any static file server. For example:

```bash
python -m http.server 8080
```

## Site Structure

| File | Purpose |
|---|---|
| `index.html` | Home page — project gallery with featured and grid post layout |
| `generic.html` | Resume page |
| `elements.html` | "Outside of Work" personal page |

## Styling

CSS lives in `assets/css/main.css` and `assets/css/noscript.css`. The source SCSS is in `assets/sass/` (structured as `base/`, `components/`, `layout/`, `libs/`). The compiled CSS is already committed — if you edit SCSS, you need to recompile manually with a Sass tool (e.g., `sass assets/sass/main.scss assets/css/main.css`). There is no watch script configured.

## JavaScript

All JS in `assets/js/` is third-party (jQuery, Scrollex, Scrolly, browser.min, breakpoints.min, util). The only custom logic is in `assets/js/main.js`.

## Adding a New Project Card

Projects are `<article>` elements inside `<section class="posts">` in `index.html`. Featured projects use `<article class="post featured">` above that section. Each card follows this pattern:

```html
<article>
    <header>
        <h2><a href="GITHUB_URL">Project Title<br /></a></h2>
    </header>
    <a href="#" class="image fit"><img src="images/your-image.jpg" alt="" /></a>
    <p>Short description.</p>
    <ul class="actions special">
        <li><a href="GITHUB_URL" class="button">Full Story</a></li>
    </ul>
</article>
```

## Images

Project images are stored directly in `images/`. Use descriptive filenames. Always use forward slashes in image paths (e.g., `images/file.jpg`) — backslashes break on GitHub Pages.

## Skills

The `frontend-design` skill is installed for this project. Use `/frontend-design` when building or redesigning UI components, pages, or sections to get production-grade, distinctive frontend output.
