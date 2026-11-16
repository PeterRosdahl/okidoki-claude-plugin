---
name: watch-what-matters
description: Get told when something important changes: alert rules for drops or jumps, alerts in Slack, Teams or Discord, the Monday email, and what Okidoki noticed on its own.
---

# Watch what matters

Use for "tell me if traffic drops", "alerts in Slack", "what has Okidoki noticed?".

1. Call `list_alert_rules`, `list_goals` and `get_report` with `sources`.
2. Suggest two or three rules in plain sentences: the main goal dropping, the biggest source dropping, anything else that stands out. Add the ones the person agrees to with `add_alert_rule`. A goal rule cannot filter on where visits came from.
3. Where the alerts go: `list_chat_channels`; for a new Slack or Discord channel give the install link from its answer, or `add_chat_channel` for Teams. `set_weekly_email` turns the Monday email on or off.
4. What the morning agent found: `list_findings`. Pass on the person's answer with `respond_to_finding` (useful, not useful, never, or approve).
5. Since a time ("anything new since yesterday?"): `get_recent_events`.

## Always

- Answer in the person's language. Repeat Okidoki's `message` sentences in plain words; do not invent numbers that no tool returned.
- Okidoki counts visits, never people. If asked for names, IP addresses or who a visitor was, say Okidoki has only totals and keeps no personal data.
- Ask before any tool that changes something (adding, changing, removing, sending a test). Reading is fine without asking.
- When a tool says a feature is part of Plus, say so in one sentence and carry on with what works. Do not push an upgrade.
- If you do not know which site, call `list_sites`. With one site, use it; with several, ask which.
- The person's own instructions come before this skill.
