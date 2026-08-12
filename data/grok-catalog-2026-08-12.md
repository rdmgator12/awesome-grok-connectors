# Grok in-app connector catalog — snapshot 2026-08-12

Consumer-session rail capture from a logged-in grok.com/connectors session.
Method: rail headings and tile names as shown in the app (no modal pass this sweep).
Diff against `grok-catalog-2026-07-23.md`.

The rail grouping (Featured / Advertising / …) is merchandising. This sweep
follows the rails in the README so the public list matches what the app shows.

## Catalog tiles (28)

### Featured (10)
Gmail, Google Calendar, Google Drive, GitHub, Box, Canva, Notion, Stripe, Vercel, **Wix** *(new)*

### Advertising (1)
X Ads

### Analytics (1)
Google Cloud BigQuery

### Developer (2)
Excalidraw, Mixpanel

### Finance (4)
Interactive Brokers (IBKR), S&P Global, Webull, **etoro** *(new)*

### Productivity (8)
Outlook, Outlook Calendar, Calendly, Figma, Gamma, HyperFrames by HeyGen, Linear, Microsoft Teams

### Sales (2)
HubSpot, Meltwater

## Delta vs 2026-07-23 (26 tiles)

- Added: Wix (Featured), etoro (Finance)
- Removed from picker: none of the prior 26
- Mixpanel remains under Developer in the rail (README had parked it in Analytics)

## Absent from this consumer picker (not removals)

- OneDrive, SharePoint, Salesforce — still in the docs.x.ai built-in table
  (fetched 2026-08-12). Business/Enterprise connectors require admin
  provisioning. Entries stay.
- Slack — still absent from both the picker and the docs built-in table.
  Failed the two-surface test carried since 2026-07-23. Removed from the
  listed set this sweep.

## Skills tab

Not re-verified this pass. Five built-ins from 2026-07-23 still listed:
Word Documents, PDFs, Presentations, Skill Creator, Spreadsheets.
