---
name: ig-carousel-designer
description: Design Instagram carousels and single-image posts as HTML and export them to PNG, free and locally. Use when the user asks to make/design a post, carousel, creative, or "post bana do".
---

# Carousel / post designer

## Specs
- Feed portrait: 1080×1350 (4:5). Square 1080×1080 only if asked. Story/reel cover: 1080×1920.
- Safe margins 80px; headline ≥64px, body ≥36px; max ~25 words per slide.
- Brand colours, fonts, logo from `brand/brand-profile.md`. If missing, propose a palette and ask once.

## Build
1. Take slide copy from `ig-post-writer`.
2. Write one HTML file per post in `content/YYYY-MM-DD-slug/slides.html`: each slide a fixed-size `<section>`; system or Google fonts; shapes, gradients, icons as inline SVG. Hindi text needs a Devanagari font (Noto Sans Devanagari / Hind).
3. Export each section to PNG with a headless browser screenshot (Playwright or Chrome `--headless --screenshot`, device scale 1) into `content/.../slide-01.png …`.
4. Open the PNGs and check: no text cut off, contrast OK, logo on first and last slide, swipe cue on slide 1, consistent look across slides.

## Design rules
- Slide 1 is a billboard: big hook, one visual, nothing else.
- One focal point per slide; left-aligned text; generous whitespace.
- Last slide: CTA + handle.
- Use only own graphics, free-licence icons/photos, or generated visuals. No screenshots of other people's content without permission.

## Output
Show the user the slide images, list the file paths, then hand over to `ig-publisher`.
