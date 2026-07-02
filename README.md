# Awesome List for Grok Connectors [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A directory of the publicly documented connectors and skills in xAI's [Grok Connectors](https://grok.com/connectors) and Grok Skills — 15 connector integrations plus 5 built-in skills plus Bring Your Own MCP, organized by category with descriptions and use cases.

**Version:** v0.1.7 | **Last updated:** July 2, 2026 | **Total connectors:** 15 | **Built-in skills:** 5 | **Categories:** 7 | **BYO MCP:** supported

See [CHANGELOG.md](CHANGELOG.md) for the full release history.

Grok connectors are OAuth-authenticated integrations that let Grok read and write across your everyday tools directly inside the chat — email, calendar, files, CRM, code, and project management — without copy-pasting. They launched May 6, 2026 on Grok Web, iOS, and Android. The same release added Bring Your Own MCP support, making Grok the fourth major assistant (after Claude, ChatGPT, and Gemini) to ship a [Model Context Protocol](https://modelcontextprotocol.io) client surface for custom servers.

[Grok Skills](https://x.ai/news/grok-skills) launched May 18, 2026 as a second primitive: persistent expertise that Grok remembers across every conversation. Each account ships with built-in skills for office documents (Word, PowerPoint, Excel, PDF) plus a Skill Creator for building your own. Skills run on Grok 4.3 across web, iOS, and Android.

> **Scope note:** This list covers connectors and skills explicitly named in xAI's public documentation and launch announcements. xAI's May 11, 2026 follow-up announcement referenced "20+ connectors" — the full catalog (beyond the named built-in set, the named catalog connectors with dedicated setup guides, and the public callouts) requires a logged-in Grok session to enumerate. Additional catalog entries will be folded in as they're publicly documented.

For more information, see the [Connectors Documentation](https://docs.x.ai/grok/connectors), the in-product catalog at grok.com/connectors (linked above), and the [launch announcement](https://x.ai/news/grok-connectors).

Connectors marked with **`X`** are built and maintained by xAI.

This list is maintained weekly. To contribute, see [CONTRIBUTING.md](CONTRIBUTING.md).

> **Disclaimer:** This is a free, public, community-maintained list. Not affiliated with, endorsed by, or sponsored by Grok, xAI Corp, SpaceX, or any Musk-affiliated entity. "Grok" and related marks are the property of xAI Corp. Each connector is the property of its respective owner. No fees, no paid placement, no commercial relationship with any vendor listed.

> [!TIP]
> ### Connector of the Week — July 2, 2026
>
> **X (hosted MCP server)** · *Bring Your Own MCP*
>
> On June 30, 2026, X shipped an official hosted MCP server exposing 200+ X API endpoints — posts, search, users, bookmarks, trends — to any MCP-compatible client, with Grok, Claude, and Cursor named at launch. For Grok users it's the highest-profile public server you can add through the BYO MCP surface (grok.com/connectors → New Connector → Custom); docs live at docs.x.com/mcp. A catalog-grade first-party integration arriving through the custom-connector door rather than the built-in list — exactly the pattern BYO MCP was built for. Details and link in the Bring Your Own MCP section below.

---

## Contents

- [Calendar and Scheduling](#calendar-and-scheduling)
- [Communication](#communication)
- [CRM and Sales](#crm-and-sales)
- [Development Tools](#development-tools)
- [Documents and Files](#documents-and-files)
- [Finance and Trading](#finance-and-trading)
- [Productivity](#productivity)
- [Bring Your Own MCP](#bring-your-own-mcp)
- [Skills](#skills)
- [Beyond the Chat](#beyond-the-chat)
- [Related](#related)

---

## Calendar and Scheduling

- [Google Calendar](https://calendar.google.com) **`X`** - Search, create, and update events in your Google Calendar. *Use case: Checking free/busy time, scheduling meetings inside a chat, RSVPing to invites, surfacing the day's agenda.*
- [Outlook Calendar](https://outlook.live.com/calendar) **`X`** - Manage Microsoft Outlook calendar events with delegated mailbox permissions. *Use case: Drafting calendar invites, finding meeting conflicts across work calendars, triaging accepted vs declined events.*


## Communication

- [Gmail](https://mail.google.com) **`X`** - Search, summarize, draft, and send messages across your Gmail inbox. *Use case: Triaging the inbox, composing context-aware replies, summarizing long threads, finding specific past conversations.*
- [Microsoft Teams](https://www.microsoft.com/microsoft-teams) **`X`** - Read messages, channels, and chats across your Microsoft Teams workspace. *Use case: Searching channel history, pulling thread context into a Grok answer, surfacing what was said about a topic across team chats.*
- [Outlook Mail](https://outlook.live.com) **`X`** - Search and act on Microsoft Outlook email with delegated mailbox permissions. *Use case: Inbox triage, drafting replies in your voice, finding attachments and threads, summarizing newsletters and notifications.*
- [Slack](https://slack.com) - Search and read Slack channels, DMs, and threads connected to your workspace. *Use case: Pulling decision context from past conversations, summarizing channel activity, finding specific files or links shared in chat.*


## CRM and Sales

- [HubSpot](https://www.hubspot.com) - Read-only access to HubSpot CRM data including contacts, companies, deals, and tickets via the [xAI MCP setup guide](https://docs.x.ai/integrations/hubspot-mcp-setup). *Use case: Summarizing open deals over a threshold, surfacing account activity, ranking pipeline by stage, drafting outreach from deal context.*
- [Salesforce](https://www.salesforce.com) **`X`** - Explore Salesforce objects, query records, and create or update CRM data. *Use case: Pulling account history, updating opportunity stages from chat, querying custom objects, generating call-prep briefs.*


## Development Tools

- [GitHub](https://github.com) - Connect repositories, issues, and pull requests for code search, PR review, and development workflow context. *Use case: Summarizing pull requests, reviewing diffs, searching across code, drafting issue descriptions, triaging backlog.*
- [Linear](https://linear.app) - Connect Linear workspace to bring tasks, issues, roadmaps, and projects into Grok. *Use case: Searching the backlog, summarizing sprint progress, drafting status updates, creating new issues from chat.*


## Documents and Files

- [Google Drive](https://drive.google.com) **`X`** - Search, read, create, and manage files across personal and shared Google Drive. *Use case: Analyzing spreadsheets without leaving chat, drafting and writing Google Docs, organizing folders, uploading Grok-generated artifacts to Drive.*
- [OneDrive](https://onedrive.live.com) **`X`** - Access personal and shared files in Microsoft OneDrive. *Use case: Reading and analyzing OneDrive spreadsheets, presentations, and reports, surfacing relevant files for a given task.*
- [SharePoint](https://www.microsoft.com/microsoft-365/sharepoint) **`X`** - Search, read, synthesize, and (with write permissions) edit files, lists, and pages across SharePoint sites. *Use case: Organization-wide document search, editing pages and lists, surfacing the latest version of policies, generating reports from SharePoint data.*


## Finance and Trading

- [Interactive Brokers](https://www.interactivebrokers.com) - Link an existing IBKR account to analyze your portfolio, model exposures, research markets, and generate reviewable order instructions across equities, ETFs, options, and futures in natural language. No new account, no passwords or API keys shared. *Use case: Surfacing portfolio exposures and concentration, scenario-modeling sector and region risk, drafting hedges and options strategies as order instructions held in an AI Instructions tab for your approval before execution.*


## Productivity

- [Notion](https://www.notion.so) - Search and edit pages, databases, and wikis across personal or team Notion workspaces. *Use case: Querying the team wiki, drafting and updating pages, querying structured Notion databases, summarizing project notes.*


## Bring Your Own MCP

Grok supports custom Model Context Protocol servers. Any MCP server reachable over the public internet can be added as a connector via grok.com/connectors → New Connector → Custom. Grok discovers the server's exposed tools and makes them available in conversations alongside built-in and catalog connectors.

For setup, authentication patterns, and local-server tunneling guidance, see the Custom MCP connectors documentation linked from the launch post above.

The highest-profile public server you can add this way: X's official hosted MCP server (launched June 30, 2026), exposing 200+ X API endpoints — posts, search, users, bookmarks, trends — documented at [docs.x.com/mcp](https://docs.x.com/mcp).

Looking for MCP servers to connect? See the awesome-mcp-servers list in the Related section below for a broad community-maintained directory that should work with Grok's BYO MCP surface.


## Skills

Grok Skills are persistent instruction sets that Grok remembers across every conversation. Launched May 18, 2026 on Grok 4.3, they ship as built-in skills out of the box, support custom-skill creation through conversation or file upload, and can be overridden — your version always takes priority. Skills are a separate primitive from connectors: connectors are the I/O layer (where the data lives), skills are the procedural layer (what to do with it).

Skills marked with **`X`** are built and maintained by xAI.

- [Word Documents](https://www.microsoft.com/microsoft-365/word) **`X`** - Create and edit .docx with full formatting — headings, tables, bullet points, and consistent styling. *Use case: Generating polished invoices, contracts, proposals, and resumes from a single chat-side instruction.*
- [Presentations](https://www.microsoft.com/microsoft-365/powerpoint) **`X`** - Build slide decks from scratch with visual hierarchy and speaker notes. *Use case: Pitch decks, quarterly reviews, workshop materials with exercises, frameworks, and takeaways.*
- [Spreadsheets](https://www.microsoft.com/microsoft-365/excel) **`X`** - Generate formatted spreadsheets with formulas, color-coded sections, and clear structure. Analyze data inline. *Use case: Budgets, dashboards, forecasts, and monthly trackers with income/expenses/savings projections.*
- [PDFs](https://www.adobe.com/acrobat/about-adobe-pdf.html) **`X`** - Create, merge, split, and extract from PDFs. Style and format for share-ready output. *Use case: Polished PDF reports, proposals, and research papers formatted for conference or stakeholder submission.*
- [Skill Creator](https://grok.com) **`X`** - Build new custom skills through conversation. *Use case: Capture a perfected workflow once and reuse it across every future chat — describe it, upload a file, or write it from scratch.*


## Beyond the Chat

This list catalogs what Grok can connect *to* inside a conversation. In June and July 2026 xAI also shipped three adjacent integration surfaces that fall outside that scope but are worth knowing.

**Microsoft Office add-ins.** [Grok for Word](https://x.ai/news/introducing-word-addin) (June 18), Grok for PowerPoint (June 16), and Grok for Excel embed Grok *inside* the Office apps as free Microsoft 365 add-ins. They can themselves leverage connectors — for example, drafting from your SharePoint or Google Drive. These are distinct from the chat-side document Skills of the same names listed above: Skills generate files chat-side, add-ins put Grok in the app.

**Grok Build and the Plugin Marketplace.** [Grok Build](https://x.ai/news) is xAI's terminal coding agent; its [Plugin Marketplace](https://x.ai/news/grok-plugin-marketplace) (June 11, open repo `xai-org/plugin-marketplace`) bundles skills, commands, agents, hooks, MCP servers, and LSPs, launching with plugins from MongoDB, Vercel, Sentry, Chrome DevTools, Cloudflare, and Superpowers. That plugin ecosystem is a separate primitive from chat connectors and would belong in a sibling list.

**Voice Agent Builder.** [Voice Agent Builder](https://x.ai/news/grok-voice-agent-builder) (July 1, beta) is xAI's no-code platform for building production voice agents on Grok Voice. It reuses the connector family in a third surface: voice agents can book into Google Calendar or Outlook Calendar, manage Linear and Notion tickets, pull files from Google Drive and OneDrive, and wire to custom APIs and MCP servers — with SIP telephony, knowledge collections, guardrails, and $0.05/min pricing.


## Related

- [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) - Community-maintained directory of MCP servers across all clients.
- [awesome-claude-connectors](https://github.com/rdmgator12/awesome-claude-connectors) - Anthropic Claude connectors directory (500+ entries).
- [awesome-claude-plugins](https://github.com/rdmgator12/awesome-claude-plugins) - Claude Code plugins directory.
- [awesome-perplexity-connectors](https://github.com/rdmgator12/Perplexity-Connectors-awesome-list-) - Perplexity AI connectors directory.
- [awesome-mistral-connectors](https://github.com/rdmgator12/awesome-mistral-connectors) - Mistral Le Chat connectors directory.
- [awesome-lm-studio-connectors](https://github.com/rdmgator12/awesome-lm-studio-connectors) - LM Studio plugins and integrations directory.
- [awesome-chatgpt-apps](https://github.com/rdmgator12/awesome-chatgpt-apps) - OpenAI ChatGPT apps and connectors directory.
- [awesome-gemini-extensions](https://github.com/rdmgator12/Gemini-Awesome-List-) - Google Gemini CLI extensions directory.
- [awesome-microsoft-copilot-connectors](https://github.com/rdmgator12/awesome-microsoft-copilot-connectors) - Microsoft Copilot connectors directory.
- [awesome-lovable-connectors](https://github.com/rdmgator12/awesome-lovable-connectors) - Lovable platform connectors directory.
- [awesome-healthcare-mcp-servers](https://github.com/rdmgator12/awesome-healthcare-mcp-servers) - Healthcare-focused MCP servers directory.
