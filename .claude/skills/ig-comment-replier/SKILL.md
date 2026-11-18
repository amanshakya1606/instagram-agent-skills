---
name: ig-comment-replier
description: Read new comments on the account's own posts and reels and draft personal replies that continue the conversation and move interested people to DM. Use when the user says "comments ka reply karo", after publishing, or in the daily routine.
---

# Comment replier

## Steps
1. Check caps in `brand/guidelines.md` and today's log.
2. Open the notifications/activity view and the last 5 posts; collect unreplied comments (handle, text, post URL).
3. Classify each:
   - **Question / interest** ("price?", "kaise?", "details") → helpful short answer + invite to DM. Mark as warm lead in `data/leads.csv`.
   - **Praise** → thank by name + a question back.
   - **Disagreement** → acknowledge, add one fact, stay polite. No arguments.
   - **Spam / bots / abuse** → no reply; list for the user to delete/hide.
   - **Complaint from a client** → empathetic, move to DM, flag to the user.
   **Reply order** (stop when the value runs out; state the counts first): KEYWORD (the word we asked people to comment — reply and deliver what was promised) → LEAD (describes a problem we solve — answer fully in public, close with one line offering help) → SUBSTANCE (adds data or disagrees — longest reply) → QUESTION (shared by many — answer, and flag as a reel idea using hook formula 16) → SUPPORT (praise/emoji — like + 3-8 words) → NOISE (spam/bait — skip). Critics: concede the valid part, hold the position, never delete, never reply twice in one thread.
4. Draft replies (then run `ig-humanizer`): 1-2 lines, same language as the commenter, specific to their words, no links, no copy-paste repeats, emoji sparingly.
5. Show the batch (comment → reply) for approval. Post only approved ones, 45-120 s apart, waiting at least 2 minutes after the comment appeared.
6. Like the comment when replying. Log every reply.

## Good examples
- "Price kya hai?" → "Depends on kya chahiye — ads, social ya full package. DM me 'PLAN' bhejo, 2 min me options bata dete hain 🙌"
- "Nice info" → "Thanks Rohit! Aap abhi apne business ke liye kaunsa platform use kar rahe ho?"

If someone asks whether a bot is replying, say honestly that the team uses AI assistance and a human is available.
