---
name: dig-deeper
description: Hard questions on the website numbers that need many numbers at once: one thing cut by another (sources by device, countries by reading, weekday by hour), patterns that go together, segments, saved views and custom queries.
---

# Dig deeper

Use when the person wants more than the standard reports: "where do my mobile visitors come from?", "which countries read the most?", "when in the week do people buy?", "save this view", "count visits to /blog from Sweden on mobile".

1. One thing cut by another: `explore` with one or two of page, source, channel, campaign, country, device, browser, language, weekday, hour or day, and a goal when the cut is place, device or time. The card shows bars or a heat map and the person can switch the measure. Call it two or three times from different angles for a hard question, then say in a few sentences what stands out and where the numbers are too small to tell. Give it a short `title` in the person's language.
2. Filters on the usual tools (`get_summary`, `get_report` take source, country, device, page and more).
3. Things that go together: `get_patterns` (over 90 days, each with the numbers behind it).
4. A group of visits to reuse: `add_segment` (never a person, only filters); `list_segments` first.
5. A view to come back to: `save_view`; `list_views` for saved ones.
6. Anything else: `run_sql` with one SELECT on the site's own events (Plus). Explain the result in words, not the query.
7. Questions worth asking right now: `suggest_questions`.

## Always

- Answer in the person's language. Repeat Okidoki's `message` sentences in plain words; do not invent numbers that no tool returned.
- Okidoki counts visits, never people. If asked for names, IP addresses or who a visitor was, say Okidoki has only totals and keeps no personal data.
- Ask before any tool that changes something (adding, changing, removing, sending a test). Reading is fine without asking.
- When a tool says a feature is part of Plus, say so in one sentence and carry on with what works. Do not push an upgrade.
- If you do not know which site, call `list_sites`. With one site, use it; with several, ask which.
- The person's own instructions come before this skill.
