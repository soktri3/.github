# Bolt Performance Journal

## 2025-05-06 - Reducing HTTP Redirects in Documentation
**Learning:** Canonicalizing URLs in documentation (e.g., from `modelcontextprotocol.io` to `modelcontextprotocol.io/docs/getting-started/intro`) eliminates unnecessary network round trips (301/302/308 redirects), providing a faster experience for users.
**Action:** Always audit documentation links for redirects and update to canonical destinations.

## 2025-05-06 - SVG Asset Optimization for GitHub Profiles
**Learning:** Minifying SVG logos in the `profile/assets/` directory using SVGO can reduce asset size. While the savings per file might be small in this specific repo (~2-5%), it is a best practice to ensure fast profile loading and reduced bandwidth.
**Action:** Run `npx svgo` on all new SVG assets with `--multipass --precision 1`.
