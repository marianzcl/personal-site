# AGENTS.md

This file applies to the entire repository for Marian's personal website. [PRODUCT.md](PRODUCT.md) describes the current site's content and features. [design.md](design.md) is the primary visual design specification. [design-exploration.md](design-exploration.md) records the earlier design candidates and decisions.

## Branches and Delivery

- Explore the redesign on `design-exploration`, using the `v1.0-before-redesign` tag on `main` as the baseline.
- The current phase covers documentation only. Get Marian's approval before implementing page changes, merging into `main`, or deploying.
- Commit and push only as authorized by the task. Preserve existing changes and keep credentials, private materials, and `.DS_Store` out of Git.

## Site Maintenance

- `index.html` contains the site's HTML, CSS, vanilla JavaScript, data, and embedded assets. `.nojekyll` lets GitHub Pages serve the static files directly. Use relative paths for new local assets so they work under the repository subpath.
- Once Marian approves page implementation, reuse the existing structure, style variables, and rendering logic wherever possible. Leave unrelated embedded images and map geometry untouched.
- Preserve direct access, reloads, and browser back and forward navigation for `#travel-map`, `#interest-timeline`, and `#personal-life`. When changing navigation, check the page title, active navigation item, and focus.
- English is the default language. Keep `.en` and `.zh` content, `[English, Chinese]` data, and any applicable titles, alternative text, control labels, and status messages in sync. Keep `lang` and `data-language` aligned when switching languages.
- Prefer semantic HTML and support keyboard navigation, visible focus, and touch input. Preserve the travel map's marker buttons and text index, and respect reduced-motion preferences.
- Use `[longitude, latitude]` for place coordinates and `approximate: true` for approximate locations. Each selectable country must have a valid region, a map view, and at least one place record. Use numeric years for interest entries and `null` when the year is unknown.
- Rely on information Marian supplies or confirms. Preserve empty states for missing photos, coffee shop entries, or dates. Use only assets cleared for public use, and check photos for privacy concerns and geolocation metadata before publishing. Store audio that visitors select in their own browsers.

## Verification

- For documentation changes, check relative links and factual claims. Before delivery, run `git status --short` and `git diff --check`, and review any new files.
- For page changes, run `python3 -m http.server 8000 --bind 127.0.0.1` from the repository root and open `http://127.0.0.1:8000/` to verify locally.
- As relevant to the change, check English and Chinese language switching, desktop and narrow layouts, keyboard focus, hash navigation, map and text index synchronization, the interest timeline, and empty states. For asset or player changes, check asset URLs under the repository subpath, the lightbox, reduced-motion preferences, or playback fallback as applicable.
