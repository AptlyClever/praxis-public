# Public / Private Praxis Boundary

## Purpose

This boundary protects private implementation work while still giving humans and agents a public-readable Praxis map.

Praxis Public should help readers understand the workflow model, vocabulary, and public-safe examples. It must not expose private operational details.

## Public Praxis may contain

Public Praxis may contain:

- public workflow vocabulary,
- object type definitions,
- public-safe Campaign summaries,
- public-safe Strand summaries,
- public-safe Fiber summaries,
- reusable Doctrines that do not reveal private implementation details,
- Imprints explaining public-safe naming and workflow decisions,
- observation-only Probes with no private host/runtime details,
- agent evaluation prompts that do not require private access,
- scrubbed examples.

## Private Praxis retains

Private Praxis remains the operational ledger for:

- full Directives containing private task details,
- Praxis Records preserving full instructions and execution evidence,
- Reports with private paths, branches, PRs, runtime notes, logs, device state, validation artifacts, and risk details,
- private repo names or implementation specifics when not intentionally public,
- homelab/runtime/device/network/Docker details,
- secrets, tokens, cookies, account identifiers, auth headers, or secret-adjacent configuration,
- unfinished product work,
- private vulnerability or risk details,
- exact deployment or service-operation instructions that are not public-safe.

## Scrub checklist

Before moving any Praxis content into this public surface, remove or generalize:

- secrets, tokens, credentials, cookies, auth headers,
- private service URLs,
- exact LAN IP addresses,
- hostnames and device names when not public-safe,
- internal filesystem paths,
- Docker compose paths, bind mounts, ports, and service topology,
- runtime logs and proof outputs,
- private issue, PR, branch, and commit references when not intentionally public,
- user email addresses or personal identifiers,
- commercially sensitive roadmap details,
- security findings not already intended for public disclosure,
- any operational instruction that would let a reader control private infrastructure.

## Authority boundary

Public Praxis is orientation. It does not grant authority.

Nothing in this repository authorizes:

- private repo access,
- implementation changes,
- PR merges,
- deployments,
- service restarts,
- device operation,
- network or Docker changes,
- destructive actions,
- publication of private material.

Any private operational work requires a separate bounded Directive and the appropriate private context.

## Sync model

Initial sync should be manual and curated.

Recommended phases:

1. Manual seed with small scrubbed object set.
2. Agent read-only comprehension tests.
3. Human review of public/private boundary performance.
4. Manifested export candidates.
5. Automation only after manual and manifest-based export are proven safe.

## Rule of thumb

If an object helps a public reader understand how Praxis thinks, it may belong here.

If an object tells someone how Control Alt private systems actually work, how they are deployed, where they run, or what is currently broken, it belongs in private Praxis.
