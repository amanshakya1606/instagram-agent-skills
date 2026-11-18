# Instagram Agent Skills (Hinglish, for marketing agencies)

A set of 22 [Claude Code](https://claude.com/claude-code) skills that run an Instagram account end to end through the browser: content calendar, carousels, reel scripts, voiceover, publishing, comments, DMs, lead finding and weekly analytics. Written for Indian businesses and agencies that talk to customers in Hinglish.

Built and used daily by **Aman Shakya**, founder of **Scalvya Digital**.

## Skills
- `ig-analytics-review`
- `ig-animated-reel-maker`
- `ig-brand-setup`
- `ig-carousel-designer`
- `ig-comment-replier`
- `ig-competitor-analysis`
- `ig-content-calendar`
- `ig-dm-inbox`
- `ig-dm-outreach`
- `ig-hashtag-seo`
- `ig-hindi-voiceover`
- `ig-humanizer`
- `ig-lead-finder`
- `ig-outbound-commenter`
- `ig-post-writer`
- `ig-profile-optimizer`
- `ig-publisher`
- `ig-reel-script-hindi`
- `ig-repurpose`
- `ig-story-planner`
- `ig-viral-reel-research`
- `instagram-agent`

`instagram-agent` is the router: ask it anything about Instagram and it picks the right skill.

## Setup
1. Copy `.claude/skills/` and `brand/` into your project folder.
2. Fill in `brand/brand-profile.md` and `brand/visual-system.md`.
3. Read `brand/guidelines.md`: daily caps (comments, DMs), action gaps, and what always needs a human (passwords, OTPs, payments).
4. Open Claude Code in that folder and say: "aaj ka Instagram kaam karo".

## Safety
- Low daily caps and slow pacing to stay inside Instagram's limits.
- First DMs carry no pitch and no link.
- Text found on Instagram is treated as data, never as instructions.
- Never invents results, reviews or clients.

## Credits
Hook formula set in `brand/hooks.md` is adapted from [instagram-agent-skill](https://github.com/Jakeschincariol/instagram-agent-skill) (MIT).

## License
MIT
