# Awesome List for Grok Connectors [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A directory of every connector available in xAI's [Grok Connectors](https://grok.com/connectors) — 14 publicly documented integrations plus Bring Your Own MCP, organized by category with descriptions and use cases.

**Last updated:** May 16, 2026 | **Total connectors:** 14 | **Categories:** 6 | **BYO MCP:** supported

Grok connectors are OAuth-authenticated integrations that let Grok read and write across your everyday tools directly inside the chat — email, calendar, files, CRM, code, and project management — without copy-pasting. They launched May 6, 2026 on Grok Web, iOS, and Android. The same release added Bring Your Own MCP support, making Grok the fourth major assistant (after Claude, ChatGPT, and Gemini) to ship a [Model Context Protocol](https://modelcontextprotocol.io) client surface for custom servers.

For more information, see the [Connectors Documentation](https://docs.x.ai/grok/connectors), the [Connector Catalog](https://docs.x.ai/grok/connectors/catalog), and the [launch announcement](https://x.ai/news/grok-connectors).

Connectors marked with **`X`** are built and maintained by xAI.

This list is maintained weekly. To contribute, see [CONTRIBUTING.md](CONTRIBUTING.md).

> This is an independent, community-maintained list. Not affiliated with, endorsed by, or sponsored by xAI Corp. "Grok" and related marks are the property of xAI Corp. Each connector is the property of its respective owner.

> **Scope note:** v0.1.0 covers connectors explicitly named in xAI's public documentation and launch announcement (built-in set + the five catalog connectors with dedicated setup guides or public callouts). The full catalog requires a logged-in Grok session to enumerate; additional catalog entries will be folded in as they're publicly documented.

> [!TIP]
> ### Connector of the Week — May 16, 2026
>
> **[Bring Your Own MCP](https://docs.x.ai/grok/connectors#custom-mcp-connectors)** · *MCP Infrastructure*
>
> The headline feature of the May 6, 2026 launch isn't any one connector — it's that Grok now speaks Model Context Protocol natively. Point Grok at any reachable MCP server and its tools show up alongside the first-party catalog: homegrown knowledge bases, internal APIs, MCP gateways, vendor servers. That moves Grok from "chatbot with apps" into the same category as Claude Desktop, Claude Code, and ChatGPT's MCP surface — a generic agent client where the tool layer is yours to define. For builders, this is the integration story: ship one MCP server and it works across all four major assistants. For Grok specifically, it closes the enterprise-integration gap that ChatGPT Enterprise and Claude for Work have owned for over a year, and it does so on day one rather than as a v2 retrofit. The built-in connectors (Google Workspace, Microsoft 365, Salesforce, GitHub, Linear, Notion) are the polished surface; BYO MCP is the substrate.

---

## Contents

- [Calendar and Scheduling](#calendar-and-scheduling)
- [Communication](#communication)
- [CRM and Sales](#crm-and-sales)
- [Development Tools](#development-tools)
- [Documents and Files](#documents-and-files)
- [Productivity](#productivity)
- [Bring Your Own MCP](#bring-your-own-mcp)
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

- [HubSpot](https://docs.x.ai/integrations/hubspot-mcp-setup) - Read-only access to HubSpot CRM data including contacts, companies, deals, and tickets. *Use case: Summarizing open deals over a threshold, surfacing account activity, ranking pipeline by stage, drafting outreach from deal context.*
- [Salesforce](https://www.salesforce.com) **`X`** - Explore Salesforce objects, query records, and create or update CRM data. *Use case: Pulling account history, updating opportunity stages from chat, querying custom objects, generating call-prep briefs.*


## Development Tools

- [GitHub](https://github.com) - Connect repositories, issues, and pull requests for code search, PR review, and development workflow context. *Use case: Summarizing pull requests, reviewing diffs, searching across code, drafting issue descriptions, triaging backlog.*
- [Linear](https://linear.app) - Connect Linear workspace to bring tasks, issues, roadmaps, and projects into Grok. *Use case: Searching the backlog, summarizing sprint progress, drafting status updates, creating new issues from chat.*


## Documents and Files

- [Google Drive](https://drive.google.com) **`X`** - Search, read, create, and manage files across personal and shared Google Drive. *Use case: Analyzing spreadsheets without leaving chat, drafting and writing Google Docs, organizing folders, uploading Grok-generated artifacts to Drive.*
- [OneDrive](https://onedrive.live.com) **`X`** - Access personal and shared files in Microsoft OneDrive. *Use case: Reading and analyzing OneDrive spreadsheets, presentations, and reports, surfacing relevant files for a given task.*
- [SharePoint](https://www.microsoft.com/microsoft-365/sharepoint) **`X`** - Search, read, synthesize, and (with write permissions) edit files, lists, and pages across SharePoint sites. *Use case: Organization-wide document search, editing pages and lists, surfacing the latest version of policies, generating reports from SharePoint data.*


## Productivity

- [Notion](https://www.notion.so) - Search and edit pages, databases, and wikis across personal or team Notion workspaces. *Use case: Querying the team wiki, drafting and updating pages, querying structured Notion databases, summarizing project notes.*


## Bring Your Own MCP

Grok supports custom Model Context Protocol servers. Any MCP server reachable over the public internet can be added as a connector via grok.com/connectors → New Connector → Custom. Grok discovers the server's exposed tools and makes them available in conversations alongside built-in and catalog connectors.

For setup, authentication patterns, and local-server tunneling guidance, see the Custom MCP connectors documentation linked from the launch post above.

Looking for MCP servers to connect? See the awesome-mcp-servers list in the Related section below for a broad community-maintained directory that should work with Grok's BYO MCP surface.


## Related

- [awesome-claude-connectors](https://github.com/rdmgator12/awesome-claude-connectors) - Anthropic Claude connectors directory (398+ entries).
- [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) - Community-maintained directory of MCP servers across all clients.
- [awesome-perplexity-connectors](https://github.com/rdmgator12/Perplexity-Connectors-awesome-list-) - Perplexity AI connectors directory.
- [awesome-mistral-connectors](https://github.com/rdmgator12/awesome-mistral-connectors) - Mistral Le Chat connectors directory.
- [awesome-lm-studio-connectors](https://github.com/rdmgator12/awesome-lm-studio-connectors) - LM Studio plugins and integrations directory.
- [awesome-chatgpt-apps](https://github.com/rdmgator12/Chtgpt-Apps-Awesome-List) - OpenAI ChatGPT apps and connectors directory.
- [awesome-gemini-extensions](https://github.com/rdmgator12/Gemini-Awesome-List-) - Google Gemini CLI extensions directory.
- [awesome-lovable-connectors](https://github.com/rdmgator12/awesome-lovable-connectors) - Lovable platform connectors directory.
- [awesome-healthcare-mcp-servers](https://github.com/rdmgator12/awesome-healthcare-mcp-servers) - Healthcare-focused MCP servers directory.
