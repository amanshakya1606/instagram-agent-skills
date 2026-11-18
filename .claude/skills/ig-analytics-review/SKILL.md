---
name: ig-analytics-review
description: Weekly review of Instagram performance — reach, views, sends, saves, follows, profile visits, DMs, leads — with a diagnosis of each post and decisions for next week. Use when the user asks "kaisa chal raha hai", for a weekly report, or before making the next calendar.
---

# Analytics review

## Collect (Professional dashboard / Insights in the browser, plus the logs)
Account: followers Δ, accounts reached (followers vs non-followers), profile visits, link taps.
Per post this week: views, likes, comments, saves, sends/shares, follows from post; for reels also average watch time / retention where shown.
Pipeline from `data/leads.csv`: DMs sent, replies, qualified, calls, won. From `activity-log.csv`: comments made, replies.

If Insights are not visible on web, ask the user for screenshots from the app.

## Read the numbers
- **Sends ÷ reach** — best signal for reaching new people.
- **Saves ÷ reach** — usefulness.
- **Follows ÷ profile visits** — profile clarity (low → run `ig-profile-optimizer`).
- **Reply rate on DMs** — below ~10% means targeting or opener is off.
Compare posts with each other, not with outside benchmarks.

## Diagnose a weak reel (in order)
1. Looked reposted / unoriginal? 2. Drop before 3 s → hook. 3. Watched but not sent → payoff/CTA. 4. Views but no follows → topic unclear or off-ICP. 5. Caption/keywords missing.

## Rank by outlier, not raw views
For each post: views ÷ the account's median views of the last 20 posts = outlier multiple. Sort by that and by sends ÷ reach. A 2× post on a small account teaches more than a big raw number.

## Learning loop
After every review, update `brand/learnings.md`: winning hooks (with formula number), flops, best format/length/time, DM opener reply rates, comment styles that got replies. Dated, one line each. Remove entries the new data contradicts. Every writing skill reads that file, so the agent improves week by week.

## Output — `reports/YYYY-Www.md`
- 5-line summary in plain Hinglish.
- Table of posts with the metrics.
- Top 2 winners and why; bottom 2 and why.
- **Keep / Stop / Try** for next week (3 each).
- Outreach funnel numbers and one change to test.
- Whether caps can be raised (only after 2 clean weeks with no warnings).
