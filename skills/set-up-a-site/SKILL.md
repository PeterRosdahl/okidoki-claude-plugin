---
name: set-up-a-site
description: "Add a new website to Okidoki, install it on the site, check that visits are counted, and pick the goals worth tracking."
---

# Set up a site

Use for "add my website", "install Okidoki", "is Okidoki working on my site?".

1. Ask for the address if you do not have it. Call `add_site`.
2. Install: the answer has one sentence to paste into the site builder (Lovable, Bolt, v0, Replit, Wix, WordPress and others) and the script tag. Give the person the one that fits how their site is built; ask if you do not know. `get_install_instructions` gives them again later.
3. When the person says it is done, call `check_install`. If it does not count yet, repeat what the answer says to fix.
4. Call `make_measurement_plan` (it reads the public site; the first plan is free) or `get_measurement_plan` if one exists. Offer the two or three goals that matter most and add the ones the person picks with `add_goal`.
5. Optional, offer once: counting visitors with ad blockers (`get_ad_blocker_setup`) and a line for the privacy policy from the install answer.

Never claim the install works before `check_install` says so.

## Always

- Answer in the person's language. Repeat Okidoki's `message` sentences in plain words; do not invent numbers that no tool returned.
- Okidoki counts visits, never people. If asked for names, IP addresses or who a visitor was, say Okidoki has only totals and keeps no personal data.
- Ask before any tool that changes something (adding, changing, removing, sending a test). Reading is fine without asking.
- When a tool says a feature is part of Plus, say so in one sentence and carry on with what works. Do not push an upgrade.
- If you do not know which site, call `list_sites`. With one site, use it; with several, ask which.
- The person's own instructions come before this skill.
