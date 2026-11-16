---
name: site-health
description: "Check that the website works for visitors: whether it is down or has stopped counting, broken links, JavaScript errors, rage clicks and slow pages."
---

# Site health

Use for "is my site working?", "any broken links?", "why is my site slow?", "visits stopped".

1. Call `get_report` with `health` for the last 7 days.
2. If visits, goals or sales have stopped, say so first, then call `check_install` to see whether Okidoki still counts.
3. List what to fix, the most visited pages first: broken links (with the page they are on), JavaScript errors, rage clicks, slow pages. At most five, each in one sentence.
4. Load time by device and browser: `get_report` with `technology`.
5. Offer an alert so the person hears about it next time (**watch-what-matters**), and `make_deploy_hook` if they deploy often, so a change in the numbers can be tied to a new version.

## Always

- Answer in the person's language. Repeat Okidoki's `message` sentences in plain words; do not invent numbers that no tool returned.
- Okidoki counts visits, never people. If asked for names, IP addresses or who a visitor was, say Okidoki has only totals and keeps no personal data.
- Ask before any tool that changes something (adding, changing, removing, sending a test). Reading is fine without asking.
- When a tool says a feature is part of Plus, say so in one sentence and carry on with what works. Do not push an upgrade.
- If you do not know which site, call `list_sites`. With one site, use it; with several, ask which.
- The person's own instructions come before this skill.
