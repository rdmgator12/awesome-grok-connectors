# Grok in-app connector catalog — snapshot 2026-07-23

First full enumeration of the logged-in grok.com/connectors catalog (consumer session).
Method: catalog grid expanded via "See more", then each tile's detail modal opened and
captured individually (tiles show no descriptions in the grid; the modal shows the
tile's own category label, its MCP server URL, and — for some tiles — a description).
Captured via Claude-in-Chrome browser automation in a logged-in session; several modals
(Gmail, Google Calendar, Google Drive, GitHub, Notion, IBKR) supplemented from a manual
paste out of the same session, same day.

Baseline for future sweeps: diff the next enumeration against this file so deltas are
attributable. The rail grouping (Featured/Advertising/…) is merchandising; the modal
category label is the tile's own classification and is recorded here.

EVERY modal — including xAI's own built-ins like Gmail — carries the boilerplate
"Third-party connectors are not built or maintained by xAI," so the boilerplate cannot
classify first- vs third-party; the docs.x.ai built-in table remains the authority. The catalog is MCP-based end to end — each tile is a hosted MCP
server whose URL the modal exposes.

## Catalog tiles (26)

| Tile (rail section) | Modal category | MCP server URL | Modal description |
|---|---|---|---|
| Gmail (Featured) | — built-in | — | "Give Grok access to search your emails." Search inbox, summarize unread, find messages from specific people; no training; emails stay in Gmail, searched real-time. |
| Google Calendar (Featured) | — built-in | — | "Give Grok access to search your calendar." Check today's schedule, find upcoming events, get meeting details; no training; events stay in Google Calendar. |
| Google Drive (Featured) | Productivity | — | "Give Grok access to your Google Drive files." Search documents, summarize presentations, ask questions about files; no training; disconnect anytime. |
| GitHub (Featured) | Developer | https://api.githubcopilot.com/mcp/x/all | "Access and interact with GitHub: search repositories and code, explore file trees and directory structures, manage repositories (branches, releases, issues, PRs), view notifications, and perform actions like starring or pushing files." |
| Box (Featured) | Storage | https://mcp.box.com | none shown |
| Canva (Featured) | Productivity | https://mcp.canva.com/mcp | none shown |
| Notion (Featured) | Productivity | https://mcp.notion.com/mcp | none shown |
| Stripe (Featured) | Payments | https://mcp.stripe.com | "Look up payments, customers, and invoices in your Stripe account." |
| Vercel (Featured) | Developer | https://mcp.vercel.com/ | none shown |
| X Ads (Advertising) | Advertising | none shown (About panel instead) | "Give Grok access to your X ad campaigns." About: view campaigns, ad groups, and ads — update creatives or create new ads with Imagine; xAI does not train on X Ads data; Grok only reads or changes ads when you ask. |
| Google Cloud BigQuery (Analytics) | Analytics | https://bigquery.googleapis.com/mcp | requires your own OAuth client credentials (Client ID + secret form in modal) |
| Excalidraw (Developer) | Developer | https://mcp.excalidraw.com/mcp | none shown |
| Mixpanel (Developer) | Developer | https://mcp.mixpanel.com/mcp | none shown |
| Interactive Brokers (IBKR) (Finance) | Finance | https://api.ibkr.com/v1/api/mcp | "Connect your Interactive Brokers account to Grok and manage your portfolio through natural language. Ask about positions, balances, P&L, allocations, and open orders, or request real-time quotes and historical market data." |
| S&P Global (Finance) | Finance | https://kfinance.kensho.com/integrations/mcp | none shown (served via Kensho, S&P's AI arm) |
| Webull (Finance) | Finance | https://api.webull.com/mcp | none shown |
| Outlook (Productivity) | — built-in | — | not captured (xAI built-in) |
| Outlook Calendar (Productivity) | — built-in | — | not captured (xAI built-in) |
| Calendly (Productivity) | Productivity | https://mcp.calendly.com/ | "Check availability, schedule and cancel meetings, and manage your Calendly event types and invitees." |
| Figma (Productivity) | Productivity | https://mcp.figma.com/mcp | "Access Figma files and design data enabling them to understand designs and generate flowcharts code and UI implementations" |
| Gamma (Productivity) | Productivity | https://mcp.gamma.app/mcp | none shown |
| HyperFrames by HeyGen (Productivity) | Productivity | https://mcp.heygen.com/mcp/hyperframes/ | none shown |
| Linear (Productivity) | — | — | not captured this pass |
| Microsoft Teams (Productivity) | — built-in | — | not captured (xAI built-in) |
| HubSpot (Sales) | — | — | not captured this pass |
| Meltwater (Sales) | Sales | https://api.meltwater.com/v2/mcp | "The Meltwater MCP server connects AI tools and workflows to Meltwater's media and social intelligence. Search billions of news articles and social posts, retrieve live metrics, trends, and sentiment, generate Boolean queries, and manage saved searches" |

## Absent from the consumer picker (no removals — see notes)

- OneDrive, SharePoint, Salesforce — in the docs.x.ai built-in table (verified live
  2026-07-23) but not rendered in this consumer-session picker. docs.x.ai:
  Business/Enterprise connectors require admin provisioning in the cloud console, so a
  consumer picker showing a subset is expected. Entries stay.
- Slack — absent from BOTH the picker and the docs built-in table (source was a launch
  callout). Carried as a removal candidate for the next sweep's two-surface test.

## Skills tab (grok.com/skills — verified live, tab routes to that URL)

Personal (5 built-ins): Word Documents ("Create, read, and edit Word documents
(.docx)"), PDFs ("Create, merge, split, and extract from PDFs"), Presentations
("Create, read, and edit PowerPoint presentations (.pptx)"), Skill Creator ("Build new
custom skills through conversation"), Spreadsheets ("Create, read, and edit spreadsheet
files (.xlsx, .csv)").

## Also on the page

- Installed section renders the user's own custom BYO MCP connectors alongside catalog
  tiles (personal servers excluded from the list per curation policy).
