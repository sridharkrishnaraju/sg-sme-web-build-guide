# Performance & Core Web Vitals

Most SME sites fail Core Web Vitals for the same handful of reasons. Fix these first.

## Largest Contentful Paint (LCP) — target < 2.5s

- Serve the hero image as WebP/AVIF, correctly sized
- Add `fetchpriority="high"` to the LCP image
- Preload the primary font; use `font-display: swap`
- Put a CDN in front of static assets

## Interaction to Next Paint (INP) — target < 200ms

- Break up long JavaScript tasks
- Lazy-load third-party scripts (chat, analytics, pixels)
- Debounce expensive input handlers

## Cumulative Layout Shift (CLS) — target < 0.1

- Set explicit `width`/`height` on images and embeds
- Reserve space for banners and cookie notices

## Getting help

A practical performance audit can usually find the top 3 fixes in an afternoon.
For Singapore SMEs, [SGBP offers performance and AI work on existing sites](https://sgbp.tech/contact)
without a full rebuild.
