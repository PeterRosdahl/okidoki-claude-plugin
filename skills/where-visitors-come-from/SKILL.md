---
name: where-visitors-come-from
description: Which sources, channels, campaigns, newsletters, ads and search terms bring visitors, sign-ups and sales, and what each campaign cost per goal.
---

# Where visitors come from

Use for "where did my visitors come from?", "which campaign worked best?", "is my ad paying off?".

1. Call `get_report` with `sources` for the period. Rank the top five and say what share each has.
2. For campaigns, call `get_report` with `campaigns`. Newsletters and ads show up here when their links have campaign tags.
3. For money: `get_report` with `revenue` (when a shop or payment platform is connected) and `list_ad_costs`. With costs entered, the campaigns report has cost per goal and return on ad spend.
4. For search: `get_google_connection`. If Search Console is connected, `get_report` with `search` (search terms, clicks and place in Google); if not, give the connect link and explain it in one sentence.
5. Two or more campaigns or sources to weigh up: use the **compare-things** skill.

If a campaign is missing, the links probably had no tags: offer the **campaign-links** skill.
Okidoki never ties a goal or a sale to a single person, only to where visits came from.

## Always

- Answer in the person's language. Repeat Okidoki's `message` sentences in plain words; do not invent numbers that no tool returned.
- Okidoki counts visits, never people. If asked for names, IP addresses or who a visitor was, say Okidoki has only totals and keeps no personal data.
- Ask before any tool that changes something (adding, changing, removing, sending a test). Reading is fine without asking.
- When a tool says a feature is part of Plus, say so in one sentence and carry on with what works. Do not push an upgrade.
- If you do not know which site, call `list_sites`. With one site, use it; with several, ask which.
- The person's own instructions come before this skill.
