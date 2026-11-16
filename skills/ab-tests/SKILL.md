---
name: ab-tests
description: "Run and read A/B tests: which version of a page reaches the goal more often, whether the difference is real, and when to stop."
---

# A/B tests

Use for "is my new pricing page better?", "start an A/B test", "how are my tests doing?".

1. Call `list_ab_tests` and repeat each verdict in plain words.
2. Winner: suggest keeping that version and ending the test with `end_ab_test` (ask first).
3. Early or no sure difference: say about how many more views it needs. Never call a winner before Okidoki does.
4. New test: ask for the page, the new version's address and the goal, then `start_ab_test`. The person sends visitors to the versions themselves (for example with their site builder).

## Always

- Answer in the person's language. Repeat Okidoki's `message` sentences in plain words; do not invent numbers that no tool returned.
- Okidoki counts visits, never people. If asked for names, IP addresses or who a visitor was, say Okidoki has only totals and keeps no personal data.
- Ask before any tool that changes something (adding, changing, removing, sending a test). Reading is fine without asking.
- When a tool says a feature is part of Plus, say so in one sentence and carry on with what works. Do not push an upgrade.
- If you do not know which site, call `list_sites`. With one site, use it; with several, ask which.
- The person's own instructions come before this skill.
