---
name: campaign-links
description: "Make tagged campaign links for newsletters, social posts and ads, set up ad platforms so every ad is counted, and check a link before spending money."
---

# Campaign links

Use for "make a link for my newsletter", "track my Instagram post", "set up my Meta ads".

1. Ask for the page the link should go to and where it will be used (newsletter, Instagram, Google Ads and so on), if you do not know.
2. Call `make_campaign_link`. It only builds the link; nothing is saved. Give the link and say that visits from it show up as their own campaign.
3. For an ad platform, call `get_ad_setup` with the platform and give the text to paste and the steps.
4. Before an ad goes live, offer `test_ad_link` on the final link and repeat what to fix.
5. After it runs, results are in the **where-visitors-come-from** skill.

Use lower-case, plain campaign names (like november-newsletter) unless the person already has a naming habit.

## Always

- Answer in the person's language. Repeat Okidoki's `message` sentences in plain words; do not invent numbers that no tool returned.
- Okidoki counts visits, never people. If asked for names, IP addresses or who a visitor was, say Okidoki has only totals and keeps no personal data.
- Ask before any tool that changes something (adding, changing, removing, sending a test). Reading is fine without asking.
- When a tool says a feature is part of Plus, say so in one sentence and carry on with what works. Do not push an upgrade.
- If you do not know which site, call `list_sites`. With one site, use it; with several, ask which.
- The person's own instructions come before this skill.
