---
name: ig-lead-finder
description: Search Instagram for ideal-client businesses, filter their profiles and posts for fit and visible marketing gaps, and build a scored prospect list. Use when the user says "leads dhundo", "clients dhundo", "post filter karo", or before DM outreach.
---

# Lead finder

## Where to look (browser, public pages only)
- Keyword + city search: "[industry] [city]" (salon, clinic, gym, cafe, real estate, coaching, boutique, D2C brand…) from the ICP.
- Location tags and local hashtags.
- Followers/commenters of local business pages and of own posts (people already engaging = warmest).
- People who liked/commented on own posts, story viewers who replied.

## Filter — keep only if
- Business/creator account that is clearly the ICP, active in last 30 days.
- Roughly 300-50k followers (owner still reads DMs).
- Has a real product/service and can plausibly pay.
- Not already with an obvious agency, not in `do-not-contact`, not already in `leads.csv`.

## Spot the gap (this becomes the DM opener)
Check their last 9 posts and bio and note one or two *specific, true* observations:
- no reels / reels with low views vs followers
- weak bio, no link/CTA, no highlights
- inconsistent posting, poor creatives, no captions
- good product but no ads/website/Google presence
- something they do well (use this as the compliment)

## Score (0-10)
ICP match 0-4 · visible gap we can fix 0-3 · activity/ability to pay 0-2 · warm signal (engaged with us) 0-1. Contact only ≥6.

## Output
Append rows to `data/leads.csv` (status `new`) with the observation in `pain_point_observed`. Report top prospects to the user. Collect only what is public and needed for outreach — no personal phone numbers or private details scraped into files.

Next: `ig-outbound-commenter` (warm up) → `ig-dm-outreach`.
