---
name: ig-outbound-commenter
description: Find relevant posts from ideal clients and niche creators and write thoughtful, non-promotional comments that earn profile visits. Use when the user says "dusre accounts pe comment karo", "engagement karo", or in the daily routine.
---

# Outbound commenter

A good comment is visible to the poster and their audience. A spammy one gets the account restricted. Quality over count.

## Targets (pick 5-10 per session, within caps)
- Recent posts (<24 h) from ICP business owners in `data/leads.csv` — warms them before any DM.
- Posts from mid-size creators the ICP follows (business, local city pages, industry pages).
- Not competitors' client-hunting posts, not giveaway/viral meme posts, not sensitive topics (politics, religion, tragedy).

## Writing rules
- Read the caption and look at the media first. The comment must prove it.
- 8-25 words. Add something: a specific compliment, an experience, a useful tip, or a genuine question.
- Same language as the post.
- Never: "Nice post", "DM us", service pitches, links, hashtags, own handle, emojis only.
- Never the same comment twice; never more than one comment per account per day.

## Nine comment types (choose by what the post says)
1. **Add a datum** — post makes a claim; back it with a number you actually have.
2. **Add the missing case** — right but incomplete; name the condition where it holds.
3. **Respectful disagree** — say what you agree with first, then where you differ.
4. **Extend one line** — quote-reference their strongest line and build on it.
5. **Ask the real question** — they skipped the hard part; ask one specific question.
6. **The receipt** — you have done what they describe; say what happened, briefly.
7. **The correction** — factual error; be brief, kind and certain.
8. **The reframe** — facts right, framing off; offer another reading.
9. **The one-liner** — nothing to add; under 10 words, funny or true.

Draft two options of different types per post and recommend one. Comment early on fresh posts. Run every draft through `ig-humanizer`.

## Examples
- Cafe owner's new menu reel → "Cold coffee wala shot kamaal hai — ye reel lunch time pe post karoge to walk-ins aur badhenge. Location tag bhi add kar do 👌"
- Business coach post on pricing → "Point 2 sabse underrated hai. Humne dekha hai discount hatane ke baad bhi clients rukte hain agar result dikhe."

## Process
1. Collect target posts (URL, handle, what the post is about).
2. Draft one comment each; show the batch for approval.
3. Post approved ones 60-120 s apart, like the post too. Stop on any block warning.
4. Log each. If the owner replies, continue the thread via `ig-comment-replier` and raise the lead's fit score.
