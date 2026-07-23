# Changelog

All notable changes to this list are documented here.

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). Versioning follows [SemVer](https://semver.org/spec/v2.0.0.html). Pre-1.0.0, minor-level changes can include additions and structural moves; patch-level changes are corrections, polish, and lint fixes.

## [0.2.0] - 2026-07-23

### Added
- **Full in-app catalog enumerated for the first time** — 15 new connectors (15 → 30): **X Ads**, **Stripe**, **Box**, **Canva**, **Vercel**, **Google Cloud BigQuery**, **Excalidraw**, **Mixpanel**, **S&P Global**, **Webull**, **Calendly**, **Figma**, **Gamma**, **HyperFrames by HeyGen**, **Meltwater**. Method: tile-by-tile modal capture from a logged-in grok.com/connectors consumer session (browser automation + same-session manual paste); raw snapshot at `data/grok-catalog-2026-07-23.md`. This resolves the "20+ connectors" scope gap carried since May — the catalog has 26 tiles.
- New **`C`** marker: third-party in-app-catalog tiles — hosted MCP servers xAI surfaces but does not build or maintain. Applied to the 15 new entries plus GitHub, Linear, Notion, HubSpot, and Interactive Brokers.
- **MCP server endpoints** recorded per catalog entry (the in-app detail view exposes them — e.g. `mcp.stripe.com`, `api.githubcopilot.com/mcp/x/all`, `api.ibkr.com/v1/api/mcp`, `kfinance.kensho.com/integrations/mcp`). The catalog is MCP-based end to end; this list now documents the endpoints.
- Three new categories: **Advertising**, **Analytics**, **Design and Creative** (7 → 10). House placement follows function; the catalog's own rail/modal labels are preserved in the data snapshot.
- GitHub entry description upgraded to the catalog's real capability text (repos, code search, file trees, branches/releases/issues/PRs, notifications, starring/pushing).

### Changed
- Connector of the Week rotated from `Automations in Grok` (7/21) to **X Ads** (7/23) — the headliner of the catalog enumeration, pairing with the same-week Grok-in-Ads-Manager beta (Beyond the Chat).
- Scope note rewritten: catalog now enumerated, not estimated; documents the MCP substrate and the Business/Enterprise provisioning nuance (OneDrive/SharePoint/Salesforce absent from a consumer picker but current in the docs built-in table — entries stay).
- Skill Creator link upgraded `grok.com` → `grok.com/skills` (verified live: the in-app Skills tab routes there; 5 built-ins confirmed with live descriptions).
- Beyond the Chat: Grok-in-Ads-Manager paragraph now cross-references the X Ads connector as its chat-side mirror.
- README header: v0.2.0, totals 30 connectors / 10 categories.

### Notes
- **Slack** is absent from BOTH the in-app catalog and the docs built-in table (its source was a launch callout) — carried as a removal candidate for next sweep's two-surface test. Not removed this pass per the two-surface rule.
- Linear and HubSpot modal endpoints not captured this pass (no server URL recorded for them) — enrich next sweep.
- The in-app modals show the third-party boilerplate on every tile including xAI built-ins, so it cannot classify first- vs third-party; the docs.x.ai built-in table remains the `X`-marker authority.
- Personal/custom BYO MCP connectors visible in a logged-in session (Installed section) are out of scope for the list.

## [0.1.9] - 2026-07-23

### Added
- `Beyond the Chat` gained **Grok in X Ads Manager** — early-access rollout since ~July 9, 2026 to a limited advertiser beta (campaign Q&A, inline AI insights, AI-generated ad creatives). Trade-press sourced (Social Media Today, July 16; first sighted by TestingCatalog July 9); no first-party x.ai post yet — upgrade the link when one lands.
- Auto-updating last-commit badge in the README header (freshness visible without a hand-typed date), matching the sibling Claude lists.

### Changed
- Related: `awesome-claude-connectors` entry is now count-free — the hand-typed count went stale twice (398+ → 500+ → actual 841); the sibling repo now carries its own live badge.
- README header bumped: version v0.1.9, `Last updated` July 23, 2026. Connector totals unchanged (15).

### Fixed
- Pre-existing awesome-lint double-link shipped in v0.1.8: the Connector of the Week block AND Beyond the Chat both hyperlinked x.ai/news/grok-automations. De-linked the COTW mention per the of-the-week convention (pick's name never hyperlinked); the link lives in Beyond the Chat. v0.1.8 went out red because admin pushes bypass the required lint check.

### Notes
- Connector of the Week stays **Automations in Grok** (July 21) — same calendar week, and a limited ads beta is a weaker pick than the shipped scheduling surface.
- Verified live against x.ai/news and the docs.x.ai sitemap (fetched 2026-07-23): no post newer than Grok for Outlook (July 21); built-in connector table unchanged (Gmail & Google Calendar through Salesforce); still no new catalog connector with a dedicated setup guide beyond HubSpot. Full catalog still requires a logged-in Grok session. Side note: x.ai/news now brands as "SpaceXAI" post-acquisition — existing disclaimer already covers SpaceX.

## [0.1.8] - 2026-07-21

### Added
- `Beyond the Chat` expanded: **Grok for Excel** (July 20) and **Grok for Outlook** (July 21) add-ins with dated links; **Automations in Grok** (July 16) as a scheduling layer over existing connectors; **Grok Build open source** (July 15); **Grok 4.5** (July 16) as the current model runtime note.
- Related: [anthropic-in-public](https://github.com/rdmgator12/anthropic-in-public) and [xai-in-public](https://github.com/rdmgator12/xai-in-public) — independent public-talks archives (sister projects).

### Changed
- Connector of the Week rotated from `X hosted MCP server` (7/2) to **Automations in Grok** (7/21) — no new named connector this window; Automations is the surface that makes the existing connector set recurring.
- README header bumped: version v0.1.8, `Last updated` July 21, 2026. Connector totals unchanged (15).

### Notes
- Verified live against docs.x.ai/grok/connectors (fetched 2026-07-21): built-in table still Gmail & Google Calendar, Google Drive, OneDrive, Outlook Mail & Calendar, Microsoft Teams, SharePoint, Salesforce. No new publicly named catalog connector with a dedicated setup guide beyond HubSpot + Interactive Brokers (announcement path). Full catalog still requires a logged-in Grok session.

## [0.1.7] - 2026-07-02

### Added
- `Beyond the Chat` gained a third adjacent surface: **Voice Agent Builder** (July 1, 2026, beta) — xAI's no-code platform for production voice agents on Grok Voice, reusing the connector family (Google Calendar, Outlook Calendar, Linear, Notion, Google Drive, OneDrive) plus custom APIs and MCP servers, with SIP telephony and knowledge collections.
- `Bring Your Own MCP` note: X launched an official hosted MCP server June 30, 2026 (docs.x.com/mcp) exposing 200+ X API endpoints to MCP clients — the highest-profile public server a Grok user can add as a custom connector.

### Changed
- Connector of the Week rotated from `Interactive Brokers` (6/26) to the `X hosted MCP server` (7/2) — the week's one genuinely connectable launch, arriving through the BYO MCP door.
- Related: corrected the stale `awesome-claude-connectors` entry count (398+ → 500+).
- README header bumped: version v0.1.7, `Last updated` July 2, 2026. Connector totals unchanged (15).

### Fixed
- Replaced the dead Connector Catalog link (`docs.x.ai/grok/connectors/catalog` now 404s and is gone from the docs sitemap) with the in-product catalog entry point at grok.com/connectors.

### Notes
- Verified live against docs.x.ai/grok/connectors (fetched 2026-07-02): built-in connector set unchanged, HubSpot still the only catalog entry with a dedicated setup guide. No connector additions or removals this window; total stays 15.

## [0.1.6] - 2026-06-26

### Added
- New `Finance and Trading` category with the **Interactive Brokers** connector — xAI's first finance integration, announced June 25, 2026. OAuth account link (no API keys shared), portfolio analysis, exposure modeling, and reviewable order instructions across equities, ETFs, options, and futures, with a human-in-the-loop AI Instructions approval tab. Total connectors 14 → 15; categories 6 → 7.
- New `Beyond the Chat` section noting two adjacent June 2026 xAI integration surfaces that fall outside this list's connector/skill scope: the Microsoft Office add-ins (Grok for Word June 18, PowerPoint June 16, Excel) and Grok Build + its Plugin Marketplace (June 11, `xai-org/plugin-marketplace`).

### Changed
- Connector of the Week rotated from `Grok Skills` (5/21) to `Interactive Brokers` (6/26), reflecting the June 25 finance-connector launch.
- README header bumped: version v0.1.6, `Last updated` June 26, 2026, total connectors 15, categories 7.

### Notes
- Verified against the official Connectors docs (crawled 2026-06-14) and Connector Catalog page: the built-in connector set and the only catalog entry with a dedicated setup guide (HubSpot) are unchanged since the June 5 sweep. Interactive Brokers is the one newly name-documented catalog connector via its dedicated x.ai/news announcement. The full catalog beyond named entries still requires a logged-in Grok session to enumerate.

## [0.1.5] - 2026-05-21

### Added
- New `Skills` top-level section covering xAI's May 18, 2026 Grok Skills launch — 5 built-in skills on Grok 4.3: Word Documents, Presentations, Spreadsheets, PDFs, and Skill Creator.
- Intro paragraph framing Skills as a second primitive alongside Connectors (I/O layer vs procedural layer).
- `Built-in skills: 5` field in the README header summary line.
- `awesome-claude-plugins` and `awesome-microsoft-copilot-connectors` added to Related list (5/16 vintage repos previously missing).

### Changed
- Connector of the Week rotated from `Bring Your Own MCP` (5/16) to `Grok Skills` (5/21), reflecting the May 18 launch and reframing connectors + skills as paired primitives.
- Scope note strengthened to explicitly reference xAI's May 11, 2026 follow-up announcement of "20+ connectors" — surfacing the public-vs-logged-in catalog enumeration gap rather than burying it.
- README header reframed from "connectors only" to "connectors and skills + BYO MCP."
- `Last updated` stamp bumped to May 21, 2026.

## [0.1.4] - 2026-05-16

### Fixed
- Reverted em-dash (`—`) separators to ASCII hyphens (`-`) between connector links and descriptions — `awesome-lint` enforces dash, not en/em-dash. Em-dashes remain in prose where lint is silent.
- Added the ASCII-dash rule explicitly to `CONTRIBUTING.md` so future contributors don't repeat the mistake.

## [0.1.3] - 2026-05-16

### Changed
- Strengthened the non-affiliation disclaimer with explicit Grok / xAI Corp / SpaceX / Musk-entity language.
- Added free / public / no-paid-placement framing.
- Mirrored disclaimer language into `CONTRIBUTING.md`.

## [0.1.2] - 2026-05-16

### Changed
- Softened "every connector" framing in the intro.
- Moved scope note up in the README for earlier reader visibility.
- Trimmed Connector of the Week editorial.
- Reordered the Related links list.
- Switched separators to em-dashes (later reverted in v0.1.4 — see above).

### Fixed
- Corrected the CONTRIBUTING marker guideline.

## [0.1.1] - 2026-05-16

### Fixed
- Corrected built-in vs. catalog connector framing in the Connector of the Week section.
- Updated HubSpot canonical URL.
- Updated `awesome-chatgpt-apps` repo URL to reflect the rename.

## [0.1.0] - 2026-05-16

### Added
- Initial scaffold of the list — 14 connectors across 6 categories, plus a Bring Your Own MCP section.
- Contents table, scope note, Connector of the Week feature, non-affiliation disclaimer, Related links to sibling awesome-lists.
- `CONTRIBUTING.md` and `code-of-conduct.md` baseline.
