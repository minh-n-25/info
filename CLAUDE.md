# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

A personal CV / portfolio site for Nguyen Do Anh Minh (RPA & Software Developer). Pure static HTML — no build step, no dependencies, no package manager, no tests. Each page is a single self-contained `.html` file with all CSS and JS inlined.

## Running / previewing

Served by XAMPP from `c:\xampp\htdocs\Claude\info`, so it's reachable at `http://localhost/Claude/info/index.html` (and `/cv.html`) when Apache is running. Otherwise just open the `.html` files directly in a browser — nothing requires a server except the PDF download and the local `avt_cv.png` image (both resolve fine over `file://` too).

## The two pages (they are separate, not linked)

- **`index.html`** — the primary "hero" page. Dark cyberpunk/HUD aesthetic (dark navy `#040d1c`, cyan `#00c8e8` accents, Rajdhani/DM Sans/JetBrains Mono fonts from Google Fonts). Single-file SPA with two view states (`#intro` and `#cv`) toggled by `showCV()` / `showIntro()` via CSS `.active`/`.leaving` classes with fade animations. All CV content (skills, languages, experience, stats) lives in **JavaScript data arrays** near the bottom of the `<script>` and is rendered into the DOM by `render*()` functions on load. To change CV content here, edit those arrays — not markup.
- **`cv.html`** — a separate, print-oriented classic CV (light theme, two-column). Content is **hardcoded in the HTML markup**, and every translatable node carries a `data-lang-key`. A `translations` object (`en`/`jp`/`vi`) plus `setLang()` swap text for the EN/JP/VI language buttons; a Print button calls `window.print()`.

## Conventions that matter

- **Bold markers**: both pages use `**text**` inside content strings and convert it to `<strong>` at render time (regex `/\*\*(.*?)\*\*/g`). Keep this syntax when editing CV text.
- **Two sources of truth for CV data**: the same facts (job titles, dates, skills) are duplicated across `index.html`'s JS arrays and `cv.html`'s markup + `translations`. When updating a fact (e.g. a job duration or skill), update **both files**, and in `cv.html` update **all three languages**.
- **PDF asset**: `index.html` links `CV_Nguyen_Do_Anh_Minh_Fullstack_Developer.pdf` via `downloadCV()`. If the CV content changes, regenerate/replace that PDF to keep it in sync.
- `README.md` is effectively empty (UTF-16, just the word "info") — not a source of information.
