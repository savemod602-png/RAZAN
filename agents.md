# Project Guide

## Architecture

This is a single-page static Netlify site. The complete user experience lives in `index.html`; styles and scripts are intentionally inline to preserve the single-file requirement. `netlify.toml` configures the repository root as the publish directory and adds basic security headers.

## Conventions

- Keep the document Arabic-first with `dir="rtl"`; the display name RAZAN remains left-to-right.
- Preserve the gift-only intro state. Celebration content must remain hidden and inaccessible until the gift button is activated.
- Keep the site dependency-free and backend-free.
- Use CSS custom properties for palette changes and transform/opacity for animation.
- Maintain reduced-motion behavior and visible keyboard focus states.

## Non-obvious decisions

The music is synthesized with the Web Audio API instead of loading an audio asset, keeping the experience self-contained. The age counter uses the visitor's local time and calculates complete years from September 24, 2009.
