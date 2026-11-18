---
name: ig-publisher
description: Publish a prepared post, carousel, reel or story to Instagram through the browser, after user approval. Use when the user says "post kar do", "upload", "publish", or a calendar item is due.
---

# Publisher

## Pre-flight
- Files exist in `content/<item>/` (PNG slides or MP4 reel 1080×1920, H.264, ≤90 s), `caption.md` final, hashtags + alt text ready.
- Show the user: preview of media, full caption, time of posting. Wait for an explicit yes for this exact item.

## Steps (instagram.com in the logged-in browser)
1. Create (+) → Post / Reel.
2. Upload files with the Chrome extension's file-upload tool. If no upload tool is available in this session, stop and ask the user to select the files (give the exact folder path), then continue.
3. Crop: 4:5 for feed, 9:16 for reels. Check slide order.
4. Paste caption; add location; add alt text under Accessibility; for reels choose the cover frame and keep "Also share to feed" on.
5. Audio for reels: use the audio baked into the video (original voiceover) or pick a track from Instagram's own audio library. Never upload ripped audio.
6. Read the screen back to verify caption and media, then press Share.
7. Confirm the post appears on the profile; copy its URL.

## After
- Log to `data/activity-log.csv`; set calendar status `published` with the URL.
- First 30-60 minutes: run `ig-comment-replier` on that post.
- Add a story sharing the post (with approval).

## Never
Post without approval, post the same file twice, or continue if Instagram shows a warning/challenge.
