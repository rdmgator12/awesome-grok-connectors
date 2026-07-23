# Awesome List for Grok Connectors [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![Last Commit](https://img.shields.io/github/last-commit/rdmgator12/awesome-grok-connectors)](https://github.com/rdmgator12/awesome-grok-connectors/commits/main)

> A directory of the connectors and skills in xAI's [Grok Connectors](https://grok.com/connectors) and Grok Skills — 30 connector integrations plus 5 built-in skills plus Bring Your Own MCP, organized by category with descriptions, use cases, and hosted-MCP server endpoints for catalog connectors.

**Version:** v0.2.0 | **Last updated:** July 23, 2026 | **Total connectors:** 30 | **Built-in skills:** 5 | **Categories:** 10 | **BYO MCP:** supported

See [CHANGELOG.md](CHANGELOG.md) for the full release history.

Grok connectors are OAuth-authenticated integrations that let Grok read and write across your everyday tools directly inside the chat — email, calendar, files, CRM, code, and project management — without copy-pasting. They launched May 6, 2026 on Grok Web, iOS, and Android. The same release added Bring Your Own MCP support, making Grok the fourth major assistant (after Claude, ChatGPT, and Gemini) to ship a [Model Context Protocol](https://modelcontextprotocol.io) client surface for custom servers.

[Grok Skills](https://x.ai/news/grok-skills) launched May 18, 2026 as a second primitive: persistent expertise that Grok remembers across every conversation. Each account ships with built-in skills for office documents (Word, PowerPoint, Excel, PDF) plus a Skill Creator for building your own. Skills run on Grok 4.3 across web, iOS, and Android.

> **Scope note:** As of July 23, 2026 this list covers the full in-app connector catalog — enumerated tile-by-tile from a logged-in grok.com/connectors session (26 catalog tiles, resolving xAI's long-standing "20+ connectors" reference) — plus the xAI-maintained built-ins documented at docs.x.ai. The catalog is MCP-based end to end: third-party tiles are hosted MCP servers whose endpoints the in-app detail view exposes, recorded per entry below. Business and Enterprise connectors (OneDrive, SharePoint, Salesforce) are provisioned by a team admin and may not appear in a consumer session's picker; they remain listed per the official docs. The raw enumeration snapshot lives in [data/grok-catalog-2026-07-23.md](data/grok-catalog-2026-07-23.md).

For more information, see the [Connectors Documentation](https://docs.x.ai/grok/connectors), the in-product catalog at grok.com/connectors (linked above), and the [launch announcement](https://x.ai/news/grok-connectors).

Connectors marked with **`X`** are built and maintained by xAI. Connectors marked with **`C`** are third-party tiles from the in-app connector catalog (enumerated July 23, 2026) — hosted MCP servers that xAI surfaces but does not build or maintain; entries note the server endpoint where the catalog exposes one.

This list is maintained weekly. To contribute, see [CONTRIBUTING.md](CONTRIBUTING.md).

> **Disclaimer:** This is a free, public, community-maintained list. Not affiliated with, endorsed by, or sponsored by Grok, xAI Corp, SpaceX, or any Musk-affiliated entity. "Grok" and related marks are the property of xAI Corp. Each connector is the property of its respective owner. No fees, no paid placement, no commercial relationship with any vendor listed.

> [!TIP]
> ### Connector of the Week — July 23, 2026
>
> **X Ads** · *The catalog cracked open*
>
> First full enumeration of the in-app connector catalog (logged-in session, all 26 tiles — the "20+ connectors" xAI referenced in May, finally itemized): fifteen connectors join the list, and X Ads headlines. It gives Grok access to your X ad campaigns — view campaigns, ad groups, and ads, update creatives, or create new ones with Imagine — with xAI stating it does not train on your Ads data. It lands the same week Grok itself went into X Ads Manager in beta (see Beyond the Chat): xAI is wiring its assistant into its own ads economy from both ends. Also new: Stripe, Figma, Canva, Box, Vercel, Google Cloud BigQuery, S&P Global, Webull, Calendly, Gamma, Excalidraw, Mixpanel, Meltwater, and HyperFrames by HeyGen.

---

## Contents

- [Advertising](#advertising)
- [Analytics](#analytics)
- [Calendar and Scheduling](#calendar-and-scheduling)
- [Communication](#communication)
- [CRM and Sales](#crm-and-sales)
- [Design and Creative](#design-and-creative)
- [Development Tools](#development-tools)
- [Documents and Files](#documents-and-files)
- [Finance and Trading](#finance-and-trading)
- [Productivity](#productivity)
- [Bring Your Own MCP](#bring-your-own-mcp)
- [Skills](#skills)
- [Beyond the Chat](#beyond-the-chat)
- [Related](#related)

---

## Advertising

- [X Ads](https://ads.x.com) **`C`** - Give Grok access to your X ad campaigns: view campaigns, ad groups, and ads — and update creatives or create new ads with Imagine. xAI states it does not train on X Ads data and that Grok only reads or changes ads when you ask. *Use case: Checking campaign performance from chat, adjusting a running ad group, generating fresh creatives without opening Ads Manager.*


## Analytics

- [Google Cloud BigQuery](https://cloud.google.com/bigquery) **`C`** - Query BigQuery from chat through Google's hosted MCP server (`bigquery.googleapis.com/mcp`); connecting requires supplying your own Google Cloud OAuth client credentials. *Use case: Ad-hoc warehouse questions in plain English, sanity-checking a metric without opening the console.*
- [Mixpanel](https://mixpanel.com) **`C`** - Product-analytics data via Mixpanel's hosted MCP server (`mcp.mixpanel.com/mcp`). *Use case: Pulling funnel, retention, and event trends into a conversation.*


## Calendar and Scheduling

- [Calendly](https://calendly.com) **`C`** - Check availability, schedule and cancel meetings, and manage your Calendly event types and invitees (hosted MCP server: `mcp.calendly.com`). *Use case: Booking a meeting from chat, checking the day's calls, rescheduling without opening the app.*
- [Google Calendar](https://calendar.google.com) **`X`** - Search, create, and update events in your Google Calendar. *Use case: Checking free/busy time, scheduling meetings inside a chat, RSVPing to invites, surfacing the day's agenda.*
- [Outlook Calendar](https://outlook.live.com/calendar) **`X`** - Manage Microsoft Outlook calendar events with delegated mailbox permissions. *Use case: Drafting calendar invites, finding meeting conflicts across work calendars, triaging accepted vs declined events.*


## Communication

- [Gmail](https://mail.google.com) **`X`** - Search, summarize, draft, and send messages across your Gmail inbox. *Use case: Triaging the inbox, composing context-aware replies, summarizing long threads, finding specific past conversations.*
- [Microsoft Teams](https://www.microsoft.com/microsoft-teams) **`X`** - Read messages, channels, and chats across your Microsoft Teams workspace. *Use case: Searching channel history, pulling thread context into a Grok answer, surfacing what was said about a topic across team chats.*
- [Outlook Mail](https://outlook.live.com) **`X`** - Search and act on Microsoft Outlook email with delegated mailbox permissions. *Use case: Inbox triage, drafting replies in your voice, finding attachments and threads, summarizing newsletters and notifications.*
- [Slack](https://slack.com) - Search and read Slack channels, DMs, and threads connected to your workspace. *Use case: Pulling decision context from past conversations, summarizing channel activity, finding specific files or links shared in chat.*


## CRM and Sales

- [HubSpot](https://www.hubspot.com) **`C`** - Read-only access to HubSpot CRM data including contacts, companies, deals, and tickets via the [xAI MCP setup guide](https://docs.x.ai/integrations/hubspot-mcp-setup). *Use case: Summarizing open deals over a threshold, surfacing account activity, ranking pipeline by stage, drafting outreach from deal context.*
- [Meltwater](https://www.meltwater.com) **`C`** - Media and social intelligence through Meltwater's hosted MCP server (`api.meltwater.com/v2/mcp`): search billions of news articles and social posts, retrieve live metrics, trends, and sentiment, generate Boolean queries, and manage saved searches. *Use case: Brand-mention monitoring from chat, sentiment pulls on a launch, building media briefs from live coverage.*
- [Salesforce](https://www.salesforce.com) **`X`** - Explore Salesforce objects, query records, and create or update CRM data. *Use case: Pulling account history, updating opportunity stages from chat, querying custom objects, generating call-prep briefs.*


## Design and Creative

- [Canva](https://www.canva.com) **`C`** - Connect your Canva account through Canva's hosted MCP server (`mcp.canva.com/mcp`). *Use case: Referencing and working with Canva designs from a conversation.*
- [Excalidraw](https://excalidraw.com) **`C`** - Virtual whiteboard and diagramming via Excalidraw's hosted MCP server (`mcp.excalidraw.com/mcp`). *Use case: Turning a chat-side idea into a shareable sketch or diagram.*
- [Figma](https://www.figma.com) **`C`** - Access Figma files and design data, letting Grok understand designs and generate flowcharts, code, and UI implementations (hosted MCP server: `mcp.figma.com/mcp`). *Use case: Asking questions of a design file, turning frames into implementation-ready code.*
- [Gamma](https://gamma.app) **`C`** - Connect Gamma's AI presentation and document builder via its hosted MCP server (`mcp.gamma.app/mcp`). *Use case: Drafting deck content in chat and carrying it into Gamma-generated presentations.*
- [HyperFrames by HeyGen](https://hyperframes.heygen.com) **`C`** - HeyGen's open-source HTML-to-video framework — write HTML, render deterministic frame-by-frame video, built for agents — via its hosted MCP server (`mcp.heygen.com/mcp/hyperframes/`). *Use case: Composing and editing programmatic video from a conversation.*


## Development Tools

- [GitHub](https://github.com) **`C`** - Search repositories and code, explore file trees and directory structures, manage repositories (branches, releases, issues, PRs), view notifications, and perform actions like starring or pushing files — served through GitHub's Copilot MCP endpoint (`api.githubcopilot.com/mcp/x/all`). *Use case: Summarizing pull requests, reviewing diffs, searching across code, drafting issue descriptions, triaging backlog.*
- [Linear](https://linear.app) **`C`** - Connect Linear workspace to bring tasks, issues, roadmaps, and projects into Grok. *Use case: Searching the backlog, summarizing sprint progress, drafting status updates, creating new issues from chat.*
- [Vercel](https://vercel.com) **`C`** - Connect your Vercel projects and deployments via Vercel's hosted MCP server (`mcp.vercel.com`). *Use case: Checking deploy status and project state from chat.*


## Documents and Files

- [Box](https://www.box.com) **`C`** - Cloud content storage via Box's hosted MCP server (`mcp.box.com`). *Use case: Searching and referencing Box files in a conversation, pulling document context into an answer.*
- [Google Drive](https://drive.google.com) **`X`** - Search, read, create, and manage files across personal and shared Google Drive. *Use case: Analyzing spreadsheets without leaving chat, drafting and writing Google Docs, organizing folders, uploading Grok-generated artifacts to Drive.*
- [OneDrive](https://onedrive.live.com) **`X`** - Access personal and shared files in Microsoft OneDrive. *Use case: Reading and analyzing OneDrive spreadsheets, presentations, and reports, surfacing relevant files for a given task.*
- [SharePoint](https://www.microsoft.com/microsoft-365/sharepoint) **`X`** - Search, read, synthesize, and (with write permissions) edit files, lists, and pages across SharePoint sites. *Use case: Organization-wide document search, editing pages and lists, surfacing the latest version of policies, generating reports from SharePoint data.*


## Finance and Trading

- [Interactive Brokers](https://www.interactivebrokers.com) **`C`** - Link an existing IBKR account to analyze your portfolio, model exposures, research markets, and generate reviewable order instructions across equities, ETFs, options, and futures in natural language. No new account, no passwords or API keys shared. Hosted MCP server: `api.ibkr.com/v1/api/mcp`. *Use case: Surfacing portfolio exposures and concentration, scenario-modeling sector and region risk, drafting hedges and options strategies as order instructions held in an AI Instructions tab for your approval before execution.*
- [S&P Global](https://www.spglobal.com) **`C`** - Financial data and research served through Kensho, S&P Global's AI arm (hosted MCP server: `kfinance.kensho.com/integrations/mcp`). *Use case: Pulling company fundamentals and market context into an analysis conversation.*
- [Stripe](https://stripe.com) **`C`** - Look up payments, customers, and invoices in your Stripe account (hosted MCP server: `mcp.stripe.com`). *Use case: Checking whether an invoice was paid, summarizing recent payment activity, pulling a customer's history.*
- [Webull](https://www.webull.com) **`C`** - Connect your Webull brokerage account via its hosted MCP server (`api.webull.com/mcp`). *Use case: Reviewing positions and market data in a conversation.*


## Productivity

- [Notion](https://www.notion.so) **`C`** - Search and edit pages, databases, and wikis across personal or team Notion workspaces (hosted MCP server: `mcp.notion.com/mcp`). *Use case: Querying the team wiki, drafting and updating pages, querying structured Notion databases, summarizing project notes.*


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
- [Skill Creator](https://grok.com/skills) **`X`** - Build new custom skills through conversation. *Use case: Capture a perfected workflow once and reuse it across every future chat — describe it, upload a file, or write it from scratch.*


## Beyond the Chat

This list catalogs what Grok can connect *to* inside a conversation. Mid-2026 xAI also shipped adjacent integration surfaces that fall outside that scope but are worth knowing.

**Microsoft Office / Outlook add-ins.** [Grok for PowerPoint](https://x.ai/news/introducing-powerpoint-addin) (June 16), [Grok for Word](https://x.ai/news/introducing-word-addin) (June 18), [Grok for Excel](https://x.ai/news/introducing-excel-addin) (July 20), and [Grok for Outlook](https://x.ai/news/introducing-outlook-addin) (July 21) embed Grok *inside* the Microsoft apps as free Microsoft 365 add-ins. They can themselves leverage connectors — for example, drafting from SharePoint or Google Drive. Distinct from the chat-side document Skills of the same names: Skills generate files chat-side; add-ins put Grok in the app.

**Grok Build, Plugin Marketplace, and open source.** [Grok Build](https://x.ai/news/grok-build-cli) is xAI's terminal coding agent; its [Plugin Marketplace](https://x.ai/news/grok-plugin-marketplace) (June 11, open repo `xai-org/plugin-marketplace`) bundles skills, commands, agents, hooks, MCP servers, and LSPs. On July 15, xAI [open-sourced Grok Build](https://x.ai/news/grok-build-open-source) so the harness (skills, plugins, hooks, MCP, subagents) is readable source. That plugin ecosystem is a separate primitive from chat connectors and would belong in a sibling list.

**Voice Agent Builder.** [Voice Agent Builder](https://x.ai/news/grok-voice-agent-builder) (July 1, beta) is xAI's no-code platform for production voice agents on Grok Voice. It reuses the connector family: Google Calendar, Outlook Calendar, Linear, Notion, Google Drive, OneDrive, custom APIs, and MCP — with SIP telephony, knowledge collections, guardrails, and $0.05/min pricing.

**Automations.** [Automations in Grok](https://x.ai/news/grok-automations) (July 16) let you describe a recurring job once, attach connectors and skills, and `@`-mention tools so they run on a schedule on web and mobile. Not a new connector — a scheduling layer over the ones already listed.

**Grok in X Ads Manager.** Rolling out in early access since ~July 9, 2026 to a limited advertiser group ([trade coverage](https://www.socialmediatoday.com/news/x-adds-grok-powered-insights-to-ads-manager/825497/), July 16): Grok embedded in X Ads Manager itself — campaign Q&A, inline AI tooltips and insights across the manager, and AI-generated ad creatives. The mirror image of the X Ads chat connector listed above: the connector brings ads data into Grok; this puts Grok inside the ads product. No first-party x.ai announcement yet; beta scope may shift by general availability.

**Grok 4.5.** [Introducing Grok 4.5](https://x.ai/news/grok-4-5) (July 16) — model release for coding, agentic tasks, and knowledge work. Not a connector surface, but the runtime those connectors and skills ride on.


## Related

- [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) - Community-maintained directory of MCP servers across all clients.
- [awesome-claude-connectors](https://github.com/rdmgator12/awesome-claude-connectors) - Anthropic Claude connectors directory.
- [awesome-claude-plugins](https://github.com/rdmgator12/awesome-claude-plugins) - Claude Code plugins directory.
- [anthropic-in-public](https://github.com/rdmgator12/anthropic-in-public) - Independent archive of public talks by Anthropic team members.
- [xai-in-public](https://github.com/rdmgator12/xai-in-public) - Independent archive of public talks, demos, and essays by xAI / Grok (sister site to anthropic-in-public).
- [awesome-perplexity-connectors](https://github.com/rdmgator12/Perplexity-Connectors-awesome-list-) - Perplexity AI connectors directory.
- [awesome-mistral-connectors](https://github.com/rdmgator12/awesome-mistral-connectors) - Mistral Le Chat connectors directory.
- [awesome-lm-studio-connectors](https://github.com/rdmgator12/awesome-lm-studio-connectors) - LM Studio plugins and integrations directory.
- [awesome-chatgpt-apps](https://github.com/rdmgator12/awesome-chatgpt-apps) - OpenAI ChatGPT apps and connectors directory.
- [awesome-gemini-extensions](https://github.com/rdmgator12/Gemini-Awesome-List-) - Google Gemini CLI extensions directory.
- [awesome-microsoft-copilot-connectors](https://github.com/rdmgator12/awesome-microsoft-copilot-connectors) - Microsoft Copilot connectors directory.
- [awesome-lovable-connectors](https://github.com/rdmgator12/awesome-lovable-connectors) - Lovable platform connectors directory.
- [awesome-healthcare-mcp-servers](https://github.com/rdmgator12/awesome-healthcare-mcp-servers) - Healthcare-focused MCP servers directory.
