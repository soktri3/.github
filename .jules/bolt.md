## 2025-04-22 - Logo Asset Optimization

**Learning:** Replacing large, static PNG assets with theme-aware SVGs significantly reduces repository weight and improves initial page load for organization profiles. SVGs (approx. 3KB) are >90% smaller than high-resolution PNGs (46KB) and maintain clarity at all sizes.

**Action:** Always prefer SVGs for logos and simple graphics. Use the `<picture>` tag with `prefers-color-scheme` media queries to support dark and light modes on GitHub READMEs. Always specify `width` and `height` on images to prevent Cumulative Layout Shift (CLS).
