---
name: goals-and-funnels
description: Track what visitors should do on the site, like sign-ups, purchases, contact forms or downloads, and see where people drop off on the way.
---

# Goals and funnels

Use for "track sign-ups", "how many reach the thank-you page?", "where do people drop off?".

1. Call `list_goals` to see what is tracked.
2. For ideas, call `suggest_goals` (from what visitors did) or `get_measurement_plan`.
3. Add a goal with `add_goal` only after the person agrees: a page (like /thanks), an event (form, download, outbound, email, phone, app) or engagement (read to the end, stayed a while).
4. Results: `get_report` with `goals`, for the period and compared with the one before.
5. Drop-off: `get_report` with `paths` and a page shows where people went right after it. `get_funnel_ideas` for funnels from real paths, `list_funnels` for saved ones and `get_report` with `funnels` for their numbers. Save one with `add_funnel` when the person wants it.
6. Say which step loses the most people and one idea to try on that page.

## Always

- Answer in the person's language. Repeat Okidoki's `message` sentences in plain words; do not invent numbers that no tool returned.
- Okidoki counts visits, never people. If asked for names, IP addresses or who a visitor was, say Okidoki has only totals and keeps no personal data.
- Ask before any tool that changes something (adding, changing, removing, sending a test). Reading is fine without asking.
- When a tool says a feature is part of Plus, say so in one sentence and carry on with what works. Do not push an upgrade.
- If you do not know which site, call `list_sites`. With one site, use it; with several, ask which.
- The person's own instructions come before this skill.
