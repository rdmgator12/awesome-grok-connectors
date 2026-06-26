# Changelog

All notable changes to this list are documented here.

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). Versioning follows [SemVer](https://semver.org/spec/v2.0.0.html). Pre-1.0.0, minor-level changes can include additions and structural moves; patch-level changes are corrections, polish, and lint fixes.

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
