# SpendWise Dashboard Shell

A responsive financial dashboard layout shell built using modern CSS Grid, Flexbox, and CSS Custom Properties.

## Architectural Summary

1. **Grid Layout:** Used `.dashboard-container` with named `grid-template-areas` to render `header`, `sidebar`, and `main` layout zones without absolute positioning.
2. **Flexbox:** Used inside components (`.header`, `.nav-list`, `.card`) for vertical and horizontal item alignments.
3. **CSS Custom Properties:** Color scheme managed on `:root` with CSS variables (`--brand-color`, `--bg-color`, `--surface-color`, etc.).
4. **Responsive Media Query:** At `<= 768px`, the grid collapses into single-column layout, and vertical sidebar items shift to a horizontal scroll layout.
5. **Card Micro-interactions:** Elevated card states on `:hover` and `:focus-visible` with `transform: translateY(-4px)` and box-shadow updates over a `200ms` transition.
6. **Dark Mode:** `@media (prefers-color-scheme: dark)` overrides `:root` custom properties to support system dark mode.
