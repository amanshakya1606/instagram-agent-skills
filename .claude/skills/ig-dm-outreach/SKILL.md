---
name: ig-dm-outreach
description: Write and send personalised first DMs to qualified prospects for the agency's services, within Instagram guidelines and daily caps, with user approval. Use when the user says "DM karo", "msg bhejo", "outreach", "clients ko message".
---

# DM outreach

Cold DMs are the riskiest action on Instagram. Low volume, high personalisation, approval every time. Read `brand/guidelines.md` sections 3-5 first.

## Before writing
- Prospect is in `data/leads.csv` with score ≥6 and status `new` or `warmed`.
- Prefer prospects warmed up first (liked 2 posts + 1 real comment a day or two earlier, or they engaged with us).
- Today's outbound DM count is under the cap.

## First message formula (3 short lines, ≤45 words)
1. **Specific observation** about their page/post (from `pain_point_observed` or a real compliment).
2. **One useful insight** or reason for reaching out — no pitch.
3. **One easy question** (yes/no or one word).

No link, no price, no "we are a 360 agency offering…", no voice note, no attachments.

### Examples
- "Hi Neha, aapke bridal looks ka kaam bahut clean hai — especially last reel. Ek cheez notice ki: bio me booking link nahi hai. Bookings abhi DM se hi aati hain ya WhatsApp se?"
- "Hello sir, Spice Route ki butter chicken reel dekhi, 40k views 🔥 Aap abhi Instagram se orders track karte ho ya sirf awareness ke liye use ho raha hai?"

## Flow after reply (handled in `ig-dm-inbox`)
Reply → 1-2 questions about their goal → offer free audit / quick tip → share proof → suggest call/WhatsApp. Pitch only after they show interest.

## Follow-up
One only, after 3-4 days, adding new value ("aapke page ke liye 2 quick ideas likhe the, bhej du?"). Then stop.

## Process
0. Read `brand/learnings.md` for openers with the best reply rate; run every draft through `ig-humanizer`.
1. Draft DMs for today's prospects (max per caps). Show the batch: handle, observation used, message.
2. Send approved ones only, 90-180 s apart, different opener each.
3. Update `leads.csv` (status `dm-sent`, date) and the activity log.
4. Stop immediately on any block/warning screen; report.

## Opt-out
"No / not interested / stop" → one polite thank-you, status `do-not-contact`, never again.
