# Copilot instructions

## Project overview

- This is a static, Spanish-language Día de Muertos information site. The entry point is `index.html`; it links directly to the single stylesheet, `style.css`.
- The page is organized as a single document: the navigation links to section IDs such as `#que-es`, `#elementos-imagenes`, and `#raices`. Keep those IDs and their matching links in sync when changing page sections.
- Images are local files in the repository root, referenced from HTML with relative paths. Preserve their exact filenames, including spaces, accents where present, and letter case.
- Most visual rules are shared through element selectors in `style.css`; `.menu` provides navigation-specific styling, and media queries at 768px and 400px adjust the layout for narrower screens. The final `.menu` rule overrides its earlier positioning, so inspect the cascade before changing menu behavior.

## Build, test, and lint

- There are no package manifests or configured build, test, or lint commands.
- To preview the site, open `index.html` in a browser. Check navigation anchors, local image loading, and the responsive layout at desktop and narrow viewport widths.
- No automated or single-test command is configured.

## Content and styling conventions

- Keep page copy and navigation labels in Spanish.
- Use semantic HTML sections with stable IDs for in-page navigation; use descriptive `alt` text for content images.
- Keep asset references relative to `index.html`; there is no asset bundler or framework pipeline.
- Add styles to the existing `style.css` and account for its shared element-level rules, responsive breakpoints, and later cascade overrides.
