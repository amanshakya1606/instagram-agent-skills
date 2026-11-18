---
name: ig-dm-inbox
description: Handle the Instagram inbox — replies from prospects, service inquiries, message requests, story replies — qualify leads, answer objections and move them to a call or WhatsApp. Use when the user says "inbox dekho", "DM ka reply karo", or in the daily routine.
---

# DM inbox

## Steps
1. Open Messages (Primary, General, Requests). List threads whose last message is from the other person.
2. Skip: bare reel forwards with no text, spam, collaboration scams, anything asking for login/OTP/payment (flag to user).
3. Classify and draft:
   - **Inquiry ("price?", "services?")** → thank, ask 2 qualifying questions (business type, goal/budget range) before quoting; share starting price only if it is in the brand profile.
   - **Reply to our outreach** → answer what they said, give one specific idea for their page, offer the free audit.
   - **Interested** → propose next step: call slot or WhatsApp; one link max.
   - **Objection** → use the honest answers in `brand/brand-profile.md`:
     - "Mehenga hai" → break down what is included, offer a smaller starting package if one exists.
     - "Sochke batata hu" → fine; ask what would help decide; offer to send a short plan.
     - "Pehle agency se result nahi mila" → ask what went wrong; explain process and reporting; no promises of guaranteed results.
   - **Not interested** → polite close, `do-not-contact`.
   - **Existing client / complaint** → empathetic, no sales, flag to the user right away.
4. Drafts: 1-3 short lines, their language, one question at the end, no walls of text.
5. Show the batch (their message → our reply) for approval; send approved ones 30-60 s apart.
6. Update `data/leads.csv` status: `replied → qualified → call-booked → won / lost`, with notes.

## Rules
- Never share prices, discounts, timelines or guarantees that are not in the brand profile — ask the user.
- Never ask for or accept payment details in DM.
- If asked "bot ho?" → honest: AI-assisted, team member can join.
- Anything unusual, legal, or angry → hand to the user, do not improvise.
