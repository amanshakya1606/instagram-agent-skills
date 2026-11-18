---
name: ig-post-writer
description: Write Instagram post copy — captions, hooks, carousel slide text, CTAs — in the brand's Hinglish voice for a marketing agency audience. Use when the user asks to write a post, caption, carousel copy, or says "post likho".
---

# Post writer

Read `brand/brand-profile.md` and the calendar item first.

## Caption structure
1. **Hook (first 125 characters — before "more")**: contains the search keyword and a reason to keep reading.
2. **Body**: short lines, one idea per line, concrete example or number, 3-6 lines.
3. **CTA**: one action only. Prefer save / send ("Apne us dost ko bhejo jiska business online nahi chal raha") or DM keyword ("DM 'AUDIT'").
4. **Hashtags**: 3-5 relevant ones from `ig-hashtag-seo`, at the end.

## Hook formulas (rotate, do not repeat within a week)
- Mistake: "90% local businesses Instagram pe ye galti karte hain"
- Number: "3 cheezein jo aapke ads ka paisa barbaad kar rahi hain"
- Contrarian: "Followers badhane se sales nahi badhti. Ye badhata hai:"
- Before/after: "₹X spend → Y leads. Kya badla?" (real numbers only)
- Question: "Aapka competitor aapse zyada kyu dikh raha hai?"
- Story: "Ek client ne kaha 'Instagram hamare liye kaam nahi karta'..."

## Carousel copy (7-9 slides)
Slide 1 hook (≤8 words) → 2 problem → 3-7 one point per slide (≤25 words) → 8 recap → 9 CTA. Each slide must make sense alone and pull to the next.

More formulas: `brand/hooks.md` (26). Past winners/flops: `brand/learnings.md`. Missing numbers become `{aapka number}` placeholders, never invented.

## Quality check before showing
- Run the draft through `ig-humanizer`.
- Would the ICP stop scrolling? Is the first line specific?
- No jargon without explanation; no fake claims; no "guaranteed".
- Reads naturally aloud in Hinglish (Roman script unless the user wants Devanagari).

## Output
Give 2 hook options + 1 full caption + alt text. Save to `content/YYYY-MM-DD-slug/caption.md`. Publishing happens only through `ig-publisher` after approval.
