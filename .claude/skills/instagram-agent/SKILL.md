---
name: instagram-agent
description: Master Instagram agent for a marketing agency's account. Use for any Instagram request — growth, posting, reels, comments, DMs, leads, calendar, profile, analytics — or when the user says "Instagram chalao", "aaj ka kaam karo", "daily routine". Routes to the right ig-* skill and enforces the safety guidelines.
---

# Instagram Agent (orchestrator)

Works through the browser only — no API, no paid tools.

## Always first
1. Read `brand/guidelines.md` (hard rules) and `brand/brand-profile.md`.
2. If the brand profile still has TODOs that the task needs, run `ig-brand-setup` first.
3. Read `brand/learnings.md` (what has worked on this account) and `brand/hooks.md` when writing.
4. Read today's rows in `data/activity-log.csv` to know remaining daily caps.

## Routing
| User wants | Skill |
|---|---|
| Set up brand, audience, services | `ig-brand-setup` |
| Bio, name, highlights, grid audit | `ig-profile-optimizer` |
| Weekly plan: what + when to post | `ig-content-calendar` |
| Caption / post copy | `ig-post-writer` |
| Carousel or single-image design | `ig-carousel-designer` |
| Hashtags, keywords, search visibility | `ig-hashtag-seo` |
| Upload a post/reel/story | `ig-publisher` |
| Stories plan | `ig-story-planner` |
| Find viral animated reels to learn from | `ig-viral-reel-research` |
| Hindi reel script | `ig-reel-script-hindi` |
| Hindi voiceover audio | `ig-hindi-voiceover` |
| Build the animated reel video | `ig-animated-reel-maker` |
| Reply to comments on own posts | `ig-comment-replier` |
| Comment on other accounts | `ig-outbound-commenter` |
| Find prospects / filter posts | `ig-lead-finder` |
| First DM for services | `ig-dm-outreach` |
| Reply in inbox, handle objections | `ig-dm-inbox` |
| Make any draft sound human (last step before approval) | `ig-humanizer` |
| One piece of own content → a week of posts | `ig-repurpose` |
| Study competitors | `ig-competitor-analysis` |
| Weekly numbers and what to change | `ig-analytics-review` |

## Daily routine ("aaj ka kaam karo")
Run in this order, each with its own approval batch:
1. `ig-comment-replier` — reply to new comments (warmest audience first).
2. `ig-dm-inbox` — answer inbox and message requests.
3. `ig-publisher` — publish today's calendar item if one is ready.
4. `ig-outbound-commenter` — 5-10 thoughtful comments on ICP / peer posts.
5. `ig-lead-finder` → `ig-dm-outreach` — 3-5 new prospects, personalised first DMs.
6. Append everything to the logs and give a 5-line summary: done, pending approval, caps left, anything blocked.

## Weekly routine (Sunday)
`ig-analytics-review` → `ig-viral-reel-research` → `ig-content-calendar` for next week → batch-produce posts and reels.

## Reporting
Say plainly what was actually sent/published vs. only drafted. Never report an action as done unless the page confirmed it.
