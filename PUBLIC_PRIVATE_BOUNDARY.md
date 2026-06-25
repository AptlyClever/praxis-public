# Public / Private Boundary

Praxis operates as a two-layer model.

| Layer | Visibility | Purpose |
| --- | --- | --- |
| **Private Praxis** | Private | Full operational ledger: handoffs, reports, runtime notes, private repo references, agent traces, deploy context |
| **Public Praxis** | Public | Sanitized durable workflow objects: object model, doctrines, imprints, campaign summaries, agent orientation prompts |

## What is public-safe

- Object kind definitions and lifecycle descriptions
- Sanitized campaign and strand summaries
- Agent orientation prompts for read-only comprehension
- Doctrines and imprints without private runtime detail
- Templates for Praxis objects
- Current work summaries at metadata and purpose level

## What is private-only

- Full handoff artifacts with private task semantics
- Reports containing exact private repo paths, LAN IPs, device names, Docker paths, service URLs, or runtime logs
- Operational protocols for deploy, device, network, or Docker actions
- Agent traces that reveal implementation details or private repo state
- Secrets, tokens, credentials, cookies, auth headers, or account IDs
- Objects referencing private vulnerabilities, unfinished product mechanics, or homelab topology

## Scrub checklist

Before publishing a Praxis object publicly, check for:

- Private repo names where public naming is not intentional
- Exact LAN IP addresses (192.168.x.x, 10.x.x.x, 172.16-31.x.x)
- Hostnames that reveal private infrastructure
- Docker Compose paths and bind mounts
- Service ports and internal service URLs
- API keys, tokens, credentials, cookies, or auth headers
- Device IDs or TV/room names if sensitive
- Runtime proof logs and stack traces
- Private issue/PR URLs when not intentionally public
- User email addresses or personal identifiers
- Commercially sensitive roadmap details

## Authority boundary

Public Praxis is orientation and context only.

- Agents reading Public Praxis may explain workflows and load object model context.
- Agents reading Public Praxis may NOT modify private repos, deploy services, or execute runtime commands.
- Implementation requires a private Directive from private Praxis.
- Public Praxis does not substitute for private Praxis as the operational authority.

## Publisher leak detection

The publisher runs conservative fail-closed checks before inclusion.
Flagged content is excluded, not silently included.
Limitations are recorded in the export report.