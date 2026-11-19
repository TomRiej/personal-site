# Your profile site

Based on template 2 (sidebar). About, Education (as a timeline) and Contact live in the cream sidebar; Experience and Projects are on the main page.

Run locally from Zed's terminal (Ctrl+`), inside this folder:

    python3 -m http.server 8000

then open http://localhost:8000. Save in Zed, refresh the browser.

- Colors: the variables at the top of `style.css`.
- Font: Arial for body text; EB Garamond (Google Fonts) for the blue accent text.
- Add an education entry: copy one `<li>` inside `<ol class="edu-timeline">` in `index.html`. Newest goes first. Give the entry you are still doing `class="current"` (blue border with a small shadow).
- Education icons live in `logos/`. Each timeline entry starts with `<span class="node"><img src="logos/name.svg" alt="..."></span>`; use a small, square-ish icon (crest or emblem), not a full wordmark. Add class `crest` to the span for shields, so they fill more of the box.
- Experience / Projects: two panels side by side in `<div class="slider">`. The big tabs at the top are their titles; clicking one (or the arrow keys, or swiping on a phone) slides to that panel. The URL follows along (`#experience`, `#projects`), so you can link straight to a panel. To add a third panel, add another `<a role="tab">` to `.topnav` and a matching `<section class="panel">` inside `.slider-track`. Slide speed and easing: `--slide` at the top of `style.css`.
