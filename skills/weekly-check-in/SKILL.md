---
name: weekly-check-in
description: "How the website or business did this week or last week: the weekly check-in card, what changed and the next steps worth taking."
---

# Weekly check-in

Use for "how did last week go?", "Monday check-in", "how is my business doing?".

When the person only wants the picture fast ("how is my site doing?", "quick overview", "snabbt"), call `quick_look` instead: one call, a card with everything, and answer in two or three sentences without calling more tools.

1. Call `get_weekly_brief` for the site. The card shows the numbers, so do not repeat them all.
2. Tell the person in at most three sentences how the week went and the one change that matters most.
3. If the answer has next steps, list them (at most three) and offer to do the ones Okidoki's tools can do. Ask first.
4. If something dropped and the person wants to know why, continue with the **explain-a-change** skill.

For "how did the last 30 days go?" or another period, use `get_summary` with that period instead of the card.

## Always

- Answer in the person's language. Repeat Okidoki's `message` sentences in plain words; do not invent numbers that no tool returned.
- Okidoki counts visits, never people. If asked for names, IP addresses or who a visitor was, say Okidoki has only totals and keeps no personal data.
- Ask before any tool that changes something (adding, changing, removing, sending a test). Reading is fine without asking.
- When a tool says a feature is part of Plus, say so in one sentence and carry on with what works. Do not push an upgrade.
- If you do not know which site, call `list_sites`. With one site, use it; with several, ask which.
- The person's own instructions come before this skill.
