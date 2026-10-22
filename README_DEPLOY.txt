AnyGameRenderer showcase site — static deploy package (2026-10-22)

Contents: index.html (single page) + media/ (videos/posters) + fonts/ (local TTFs).
Fully static, no build step, no external requests. Deploy = serve this directory as-is
(nginx / any static host). Root document: index.html.

Notes:
- Videos are served with HTTP Range requests by any standard static server (needed for
  smooth seeking/looping; nginx/apache/CDN all do this out of the box).
- The Technical report button under the title still has
  placeholder href="#" — fill in the real links in index.html when available.
- favicon: media/favicon.png, referenced from <head>.
