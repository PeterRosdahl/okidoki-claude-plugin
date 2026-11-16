---
name: explain-a-change
description: Find out why visitors, page views, goals or sales went up or down: which source, page, campaign or day the change came from, and what happened then.
---

# Explain a change

Use for "why did traffic drop?", "where did this spike come from?", "anything I should know?".

1. Call `get_summary` for the period the person means (default: last 7 days against the 7 before) to confirm the size of the change.
2. Call `get_insights` for what changed more than usual.
3. Narrow it down with `get_report`: `sources` first, then `pages` and `campaigns`. Look for the one or two rows that make up most of the change.
4. For the days around the change, call `get_report` with `calendar` (holidays, paydays, weather, downtime), `find_occasions` and `list_occasion_notes` (a sale, a newsletter, a holiday) and `list_findings` (what Okidoki's morning agent noticed).
5. Say in plain words: how big the change is, where it came from, and the most likely reason. Say "not sure" when the numbers do not show it; never guess a cause as fact.
6. Offer one useful next step, for example an alert rule (**watch-what-matters**) or a note of the occasion with `add_occasion_note`.

Small numbers (a few dozen visitors) move a lot by chance; say so.

## Always

- Answer in the person's language. Repeat Okidoki's `message` sentences in plain words; do not invent numbers that no tool returned.
- Okidoki counts visits, never people. If asked for names, IP addresses or who a visitor was, say Okidoki has only totals and keeps no personal data.
- Ask before any tool that changes something (adding, changing, removing, sending a test). Reading is fine without asking.
- When a tool says a feature is part of Plus, say so in one sentence and carry on with what works. Do not push an upgrade.
- If you do not know which site, call `list_sites`. With one site, use it; with several, ask which.
- The person's own instructions come before this skill.
