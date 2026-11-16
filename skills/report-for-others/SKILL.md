---
name: report-for-others
description: "Make a report of the website numbers for a boss, client or team: a written summary, a read-only share link, a spreadsheet export, or a report sent every Monday or month."
---

# Report for others

Use for "write a report for my boss", "send the client their numbers", "a report every Monday".

1. Ask what period and what matters to the reader, if not given.
2. Gather: `get_summary` for the period, `get_report` for `sources`, `pages` and `goals` (and `campaigns` or `revenue` if relevant), `get_moments` for anything worth celebrating.
3. Write it in the person's language: one headline sentence, three to five short points with numbers and the change, one thing to do next. No jargon.
4. Offer the right way to share:
   - a read-only link anyone can open: `create_share_link`;
   - a spreadsheet: `export_csv`;
   - sent automatically every Monday or on the 1st: `save_view` with a schedule and recipients (see `list_views` first).
Ask before creating anything.

## Always

- Answer in the person's language. Repeat Okidoki's `message` sentences in plain words; do not invent numbers that no tool returned.
- Okidoki counts visits, never people. If asked for names, IP addresses or who a visitor was, say Okidoki has only totals and keeps no personal data.
- Ask before any tool that changes something (adding, changing, removing, sending a test). Reading is fine without asking.
- When a tool says a feature is part of Plus, say so in one sentence and carry on with what works. Do not push an upgrade.
- If you do not know which site, call `list_sites`. With one site, use it; with several, ask which.
- The person's own instructions come before this skill.
