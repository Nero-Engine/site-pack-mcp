# Site Pack

Free tools a UK builder's AI assistant uses on the job: permitted development and Building Regulations checks, Party Wall Act notice dates, CDM 2015 duties and F10, brick, block, concrete and plasterboard quantities, and structural emergency triage.

**Endpoint:** `https://site-pack.nerolabs.workers.dev/mcp` (MCP, Streamable HTTP)
**Sign-in:** None. No account, no key and no sign-in: add the address and use it.
**How to connect:** https://site-pack.nerolabs.workers.dev/docs
**Privacy:** https://site-pack.nerolabs.workers.dev/privacy
**Support:** founder@neroengine.com

## Tools

| Tool | What it does |
|---|---|
| `list_capabilities` | What Site Pack can do. Lists Site Pack's tools, the date its rules were last checked, what it covers (nations, project types, work types) and what it deliberately does not do. |
| `check_permitted_development` | Planning: permitted development or not? (England). Checks a householder project in England against the permitted development limits in the GPDO 2015, Schedule 2, Part 1: single and multi storey rear extensions, side and wraparound extensions (Class A), loft dormers and hip to gable (Class... |
| `check_building_regs` | Building Regulations: notifiable, which route, which Parts? (England and Wales). For one or more kinds of building work in England or Wales: is it notifiable building work, exempt (small outbuildings, ground level conservatories and porches up to 30 m2), self-certifiable by a competent person scheme (FENSA, Certass,... |
| `party_wall_notices` | Party Wall Act notices and dates (England and Wales). Works out which notice the Party Wall etc. |
| `cdm_duties` | CDM 2015 duties and HSE F10 notification. For a construction project in Great Britain (domestic by default): who holds the client's duties (on a domestic job they pass to the contractor, the principal contractor, or the principal designer under a written agreement), which roles... |
| `estimate_materials` | Bricks, blocks, mortar, concrete and plasterboard quantities. Works out quantities from dimensions, with the working: bricks (60 a m2 per half brick leaf), blocks (about 10 a m2), cavity walls with ties, mortar from wall volume minus unit volume, cement bags and sand tonnes for a chosen mix, concrete... |
| `structural_triage` | Structural worry: how urgent, and safe first steps. First-response triage when a customer reports a crack, a bulging or leaning wall, a sagging or fallen ceiling, a collapse, storm damage to a roof or chimney, a fallen tree or vehicle impact, a sagging floor, problems after a wall was... |
| `trade_profile` | Check the builder's business details. Checks the builder's own business details (Nero Trade Profile v1: trading name, Companies House number, trade body or scheme and membership number such as FMB or TrustMark, postcode, contact) and returns them cleaned, with a stable... |

Every tool carries a plain title and the read-only, destructive and open-world hints, so your AI app can ask before anything that changes data.

## Connect

- **Claude (web or desktop):** Settings, Connectors, Add custom connector, paste the endpoint.
- **ChatGPT:** Settings, Apps and connectors, Advanced settings, switch on Developer mode, then Create, paste the endpoint, No authentication.
- **Claude Code:** `claude mcp add --transport http site-pack https://site-pack.nerolabs.workers.dev/mcp`
- **Cursor, VS Code, Windsurf and others:**

```json
{ "mcpServers": { "site-pack": { "type": "http", "url": "https://site-pack.nerolabs.workers.dev/mcp" } } }
```

## Try asking

- "Can I build a 4 metre deep single storey rear extension on a semi-detached house in England without planning permission?"
- "I want to start digging foundations next to the neighbour's wall on 1 March. When must the party wall notice go out?"
- "How many bricks, blocks and bags of mortar for a 6 by 2.4 metre cavity wall?"

## Good to know

- Built for UK builders. Every answer shows its working and sources and lists what the trade must check. The trade doing the work stays responsible for it.
- Free forever: no sign-up, no key, no daily cap, no paid plan.

## Privacy

What is kept, what is never kept, and how to get data deleted: https://site-pack.nerolabs.workers.dev/privacy. Usage counts log the tool name, time, AI app name, country and a one-way scrambled caller code; never your questions, the answers or IP addresses.

This repository holds the listing only (README and server.json). The server runs at the endpoint above.

Built by Nero Labs (Nero Engine Group Ltd, UK).
