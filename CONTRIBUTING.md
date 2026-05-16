# Contributing

This list tracks every connector available in [Grok](https://grok.com/connectors) — xAI's built-in connectors, the third-party Connector Catalog, and the Bring Your Own MCP developer story. Contributions welcome.

> **Disclaimer:** This is a free, public, community-maintained project. Not affiliated with, endorsed by, or sponsored by Grok, xAI Corp, SpaceX, or any Musk-affiliated entity. No fees, no paid placement, no commercial relationship with any vendor listed.

## What You Can Contribute

### New Connectors
When xAI adds new connectors to the built-in set or the catalog, submit a PR adding them to the appropriate section with a description and use case.

### Improved Descriptions
If a description or use case is missing detail or could be more helpful, submit a PR with a better one.

### Category Corrections
If a connector is in the wrong category, submit a PR moving it.

### Field Reports
Tested a connector and have real-world notes? Add a brief field report below the connector entry:

```markdown
- [Connector Name](https://link) — Description. *Use case: ...*
  > **Field report:** One paragraph on what worked, what didn't, what surprised you. Be specific.
```

## Guidelines

- One PR per change unless closely related.
- Keep descriptions concise — one sentence for the description, one for the use case.
- Use cases should be specific and practical, not marketing copy.
- Only add connectors that are publicly available in Grok (built-in, catalog, or documented at [docs.x.ai/grok/connectors](https://docs.x.ai/grok/connectors)). For general MCP servers not yet in Grok, see [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers).
- Maintain alphabetical order within categories.
- Mark connectors maintained by xAI itself with **`X`** after the connector link, before the description separator (e.g., `[Connector](https://link) **\`X\`** — Description.`).

## Weekly Updates

This list is updated weekly to stay in sync with the official Grok Connectors set. If you notice the catalog has added connectors that aren't listed here, please open an issue or PR.
