---
name: compare-things
description: Compare campaigns, newsletters, pages, sources, countries, devices, sales days or occasions side by side, and say which did best.
---

# Compare things

Use for "which newsletter worked best?", "mobile or desktop?", "how did Black Friday compare with last year?".

1. Same kind of thing over the same period (campaigns, pages, sources, countries, devices): `compare_side_by_side` with two to four of them.
2. Things the person did at different times (emails, campaigns, notes): `list_results`, then `compare_results` with up to six.
3. Everything at once by one thing (all sources by device, all countries): `explore`.
4. Sales days and holidays: `list_occasions`, then `get_occasion` for one, against a usual stretch and last year.
5. Say which did best and by how much in two or three sentences. Say "too few to tell" when the numbers are small.

## Always

- Answer in the person's language. Repeat Okidoki's `message` sentences in plain words; do not invent numbers that no tool returned.
- Okidoki counts visits, never people. If asked for names, IP addresses or who a visitor was, say Okidoki has only totals and keeps no personal data.
- Ask before any tool that changes something (adding, changing, removing, sending a test). Reading is fine without asking.
- When a tool says a feature is part of Plus, say so in one sentence and carry on with what works. Do not push an upgrade.
- If you do not know which site, call `list_sites`. With one site, use it; with several, ask which.
- The person's own instructions come before this skill.
