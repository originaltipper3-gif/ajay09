# AGENTS.md

## Architecture

This is a static, single-file site. All markup, styles and script live in `index.html`. There is no package.json, no bundler and no build step. `netlify.toml` publishes the repository root as-is.

## Key files

- `index.html` — the landing page: header status pill, profile badge, stats grid, countdown card, CTA buttons, feature list, sticky bottom join bar, and the inline countdown/redirect script.
- `netlify.toml` — sets the publish directory to `.`.

## Conventions and decisions

- Styling uses the Tailwind Play CDN with utility classes inline. Custom effects (glow, pulse, shimmer, glass card) are defined in the `<style>` block in the head.
- The Telegram invite URL appears in four places: the `targetTelegramUrl` constant and three anchor `href`s. Keep them in sync.
- The countdown starts at 15 in the markup and in `totalSeconds`. Update both when changing it.
- Don't add a framework or build tooling unless the owner asks for it. The page is intentionally zero-build.
