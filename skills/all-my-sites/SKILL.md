---
name: all-my-sites
description: For agencies and people with many websites: every site at a glance, which ones need a look, and what to do first.
---

# All my sites

Use for "how are all my clients doing?", "which sites need attention?".

1. Call `get_portfolio` for the last 7 days (or the period asked).
2. Say in two sentences how the sites did together.
3. Go through the sites worth a look: for a drop, `get_insights` on that site; for a quiet site or one with no visits, `check_install`.
4. End with at most three things to do, the most urgent first. Ask before changing anything.

For one client's report, continue with **report-for-others**.

## Always

- Answer in the person's language. Repeat Okidoki's `message` sentences in plain words; do not invent numbers that no tool returned.
- Okidoki counts visits, never people. If asked for names, IP addresses or who a visitor was, say Okidoki has only totals and keeps no personal data.
- Ask before any tool that changes something (adding, changing, removing, sending a test). Reading is fine without asking.
- When a tool says a feature is part of Plus, say so in one sentence and carry on with what works. Do not push an upgrade.
- If you do not know which site, call `list_sites`. With one site, use it; with several, ask which.
- The person's own instructions come before this skill.
