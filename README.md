# Okidoki Analytics for Claude

![Okidoki Analytics](assets/icon.png)

Okidoki is website analytics anyone can understand, without cookies and without personal data about your
visitors. This plugin connects Claude to your Okidoki account and adds skills that teach Claude how to answer
the questions people actually ask about their website: how is my site doing, where do visitors come from,
which campaigns and newsletters worked, and which pages lead to sign-ups or sales.

## What you get

- **The Okidoki connector** (`https://okidoki.sh/mcp`). You sign in with your Okidoki account and choose
  read only, or read and change.
- **14 skills** for the most common goals: a weekly check-in, explaining why the numbers changed, where
  visitors come from, setting up a new site, goals and funnels, campaign links with UTM tags, reports for a
  boss or client, alerts, all your sites at once, A/B tests, comparisons, site health, deeper questions, and
  a short get-started skill.

## Use it

1. Add the plugin from the directory in Claude, open its **Connectors** tab and connect Okidoki. You need an Okidoki account; the free
   plan works.
2. Ask in your own words, for example:
   - "How is my website doing this week?"
   - "Give me my weekly check-in."
   - "Where did my visitors come from this month?"
   - "Why did visitors drop last week?"
   - "Make a campaign link for our newsletter to /pricing."
   - "Add a goal for people who reach /thanks."

Claude reads freely, and asks you before anything that changes your account, such as adding a goal, a
webhook or a new site. Each connection gets its own key in Okidoki, under Settings → Integrations, where you can turn it off at any time.

In Claude Code you can also install it from this repository:

```bash
/plugin install okidoki-analytics --marketplace PeterRosdahl/okidoki-claude-plugin
```

Then run `/mcp`, pick okidoki and sign in.

## Data

The plugin itself is only instructions (Markdown) and the connector's address. It runs no code on your
computer and stores nothing.

When you use it, Claude sends your questions as tool calls to Okidoki's server at `okidoki.sh`, run by
Adrbl AB in Sweden. Okidoki answers with the statistics of the websites in your own account: totals such as
visitors, page views, sources, pages, campaigns, goals and revenue. Okidoki never collects who your visitors
are, so there are no names, IP addresses or cookies to send. The plugin does not read your chat history,
memory or files, and sends nothing to anyone else.

- Privacy policy: https://okidoki.sh/privacy
- Terms: https://okidoki.sh/terms
- Documentation: https://docs.okidoki.sh/mcp
- Support: hello@okidoki.sh

## License

MIT, see [LICENSE](LICENSE). The Okidoki service itself is covered by its own terms.
