---
name: ig-animated-reel-maker
description: Produce an original animated Hindi reel (1080×1920 MP4) from a script and voiceover — motion graphics, kinetic text, captions, music, SFX — free and locally. Use when the user says "reel banao", "animated reel", or a scripted reel needs to be rendered.
---

# Animated reel maker

## Inputs
`content/<item>/script.md`, `voiceover.mp3` + per-scene durations and `.vtt`, brand colours/fonts/logo, the style notes from `ig-viral-reel-research` (style only).

## Build with HyperFrames
Load the `hyperframes` skill first and follow its render contract; use `hyperframes-registry` for ready blocks (kinetic type, captions, transitions) and `media-use` for music/SFX.
1. Scaffold a vertical 1080×1920, 30 fps project in `content/<item>/video/`.
2. One scene per script row; scene length = that scene's voiceover duration + 0.2 s.
3. Scene design:
   - Motion starts on frame 0; something changes every 1.5-2.5 s (cut, zoom, new element).
   - Big on-screen text (≥70px), max 6 words at a time, keyword highlighted in brand colour.
   - Word-by-word captions synced from the `.vtt`, placed in the middle third.
   - Keep text out of the top 220px and bottom 420px (Instagram UI overlays).
   - Simple flat illustrations/icons as SVG, charts, phone mockups; brand palette throughout.
4. Audio mix: voiceover full level, music ducked well under it (about -18 dB relative), SFX on transitions.
5. End card 2 s: CTA + @yourbrand + logo.
6. Render MP4 (H.264, AAC). Pull frames at 0 s, 3 s, middle and end and look at them: readable, nothing clipped, first frame is a strong cover.

## Originality
All visuals, script and voice are our own. No reused clips, no watermarks, no ripped audio. A reference reel informs pacing and layout only.

## Output
`content/<item>/reel.mp4`, cover image, caption from `ig-post-writer`. Show the user, then `ig-publisher` after approval.
