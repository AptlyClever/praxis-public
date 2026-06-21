# Praxis Object Type Translation Map

## Metadata

| Field | Value |
| --- | --- |
| id | `imprint-praxis-object-type-translation-map` |
| type | `praxis.imprint` |
| status | `canonical` |
| revision | `1-public` |
| created | `2026-06-20` |
| updated | `2026-06-20` |
| product_area | `Praxis / Object model / Human and agent readability` |
| source_scope | `public-safe curated export` |
| supersedes | none |
| superseded_by | none |

## Purpose

Provide a human-readable translation map for current Praxis object types.

This imprint explains each object type's intent, current functionality, industry terminology analogs, and plain-language blurb so humans and agents can orient quickly without flattening Praxis into Jira, GitHub Issues, Linear, Azure Boards, or generic Agile terminology.

## Comparison note

The industry terminology column is a conceptual comparison, not an equivalence claim.

Praxis objects are designed for an evidence-first, agent-aware workflow. Comparable systems use different object models and assumptions. For example:

- Jira uses configurable work types and default hierarchies such as Epic, Story, Task, Bug, and Subtask.
- GitHub Issues tracks ideas, feedback, tasks, bugs, and supports sub-issues, labels, milestones, and Projects.
- Linear uses Initiatives to group Projects by company objectives and track progress.
- Azure Boards process templates include work item types such as Epic, Feature, User Story, Product Backlog Item, Task, Bug, Requirement, Change Request, Risk, and Review.

Use these comparisons to orient, not to rename Praxis.

## Current first-class Praxis object types

| Object type | Industry terminology | Intent | Current functionality | Human-readable blurb |
| --- | --- | --- | --- | --- |
| **Campaign** | Similar to Linear Initiative, Jira Initiative / Advanced Roadmaps initiative, GitHub Project, Azure Epic / portfolio backlog | Coordinate a broad effort across multiple lanes, repos, agents, decisions, and outcomes. | Active object type. | The big mission. It explains what we are trying to accomplish, why it matters, what lanes exist, and what final success looks like. |
| **Beacon** | Similar to a project dashboard, Linear Initiative overview/update, GitHub Project view, status report, roadmap health page | Give humans and agents a current-state navigation object for a Campaign or Strand. | Active object type. | Start here. A Beacon tells you where we are, what is active, what is complete, what is deferred, what evidence matters, and the next safe move. |
| **Strand** | Similar to Linear Project, Jira Epic / Feature, Azure Feature / Epic, GitHub milestone or project slice | Define a bounded line or thread of work inside a Campaign. | Active object type; supersedes legacy Scheme for bounded work lines. | A major thread of the mission. A Strand is not the whole Campaign, but it is bigger than one concrete work unit. |
| **Fiber** | Similar to Jira Story / Task / Subtask depending on size, GitHub Issue / sub-issue, Linear Issue, Azure User Story / Task | Define a small identifiable work unit that advances a parent Strand. | Active object type. | The next concrete piece. A Fiber is small enough to work, finish, and verify without pretending it is a whole Strand. |
| **Directive** | Similar to a work order, implementation brief, ticket body, issue form, task spec, change request instruction | Preserve the actual instruction semantics given to an agent or implementer. | Canonized conceptually; template migration may happen separately. | What the agent was told to do. A Directive states scope, boundaries, validation, reporting, stop condition, and authority limits. |
| **Readout** | Similar to a test run result, evaluation report, CI/check result, QA result, experiment result, code review response | Record the result of a bounded evaluation run. | Active object type; should be created only after real evaluation runs. | What happened when we tested the thing. A Readout captures subject, input, allowed actions, behavior, evidence, result, cost if known, and human correction. |
| **Probe** | Similar to a diagnostic check, smoke test, health check, checklist item, GitHub Action check, Azure Test Case in spirit | Provide a reusable observation-first check. | Existing object type for recurring diagnostics and sanity checks. | A reusable check cartridge. A Probe answers one narrow question and should usually be safe/read-only. |
| **Protocol** | Similar to runbook, SOP, procedure, operational playbook, release/deploy procedure | Define a repeatable procedure composed of runnable steps. | Existing object type for repeatable procedures. | A procedure you can run. More step-oriented than a Probe and may include an ordered sequence. |
| **Doctrine** | Similar to policy, standard, working agreement, engineering guideline, architecture principle | Capture reusable guidance that outlives a single task. | Existing object type for durable workflow and behavior guidance. | The rulebook page. A Doctrine tells future humans and agents how to think or behave in a recurring area. |
| **Imprint** | Similar to ADR, decision record, RFC outcome, rationale memo, post-decision note | Preserve rationale, decisions, and conceptual locks. | Existing object type for naming decisions, conceptual locks, and rationale. | Why we decided this. An Imprint is a durable rationale and decision trace so we do not keep re-litigating the same logic. |

## Supporting artifacts and concepts

These are part of the Praxis workflow, but they are not all first-class object types in the same way.

| Artifact / concept | Industry terminology | Intent | Current functionality | Human-readable blurb |
| --- | --- | --- | --- | --- |
| **Praxis Record** | Similar to execution log, audit record, run record, change log entry, implementation journal | Preserve the execution/evidence ledger for work that was actually issued to an agent or implementer. | Private-first operational artifact. Public examples should be scrubbed. | The black box recorder. It preserves what was issued, what was done, and where the evidence lives. |
| **Report** | Similar to completion report, validation report, QA report, implementation summary, release note evidence | Summarize completion, validation, risks, boundaries, and stop/merge/deploy status. | Private-first operational artifact unless scrubbed. | What happened and how we know. Reports support review and decision-making after work. |
| **Implementation PR** | Pull request, merge request, code review change set | Carry actual implementation changes. | External code-hosting object, not Praxis-owned. | The code-change vehicle. It carries diffs, review, and merge mechanics, not the full instruction model. |
| **Relay** | Similar to artifact transport, dispatch/archive layer, workflow file exchange, integration bridge | Transport and archive workflow artifacts. | Canonical product/function name for the transport/archive role. | The courier/archive. Relay moves and preserves Directives, Reports, Records, Readouts, and related artifacts, but it is not workflow authority. |

## Load-order guidance

For a human or agent entering work midstream, use this order:

1. **Beacon** — where are we?
2. **Campaign** — what is the larger effort?
3. **Strand** — which line of work are we in?
4. **Fiber** — what concrete piece are we doing?
5. **Directive** — what exactly was the agent told to do?
6. **Praxis Record / Report / Readout** — what happened, what proved it, and what did we learn?

Beacon is the front door. Directive is the work order. Praxis Record, Report, and Readout are the evidence trail.

## Why Praxis does not use generic industry names directly

Praxis borrows lessons from issue trackers, agile planning systems, project dashboards, test systems, and architecture decision records, but it is not trying to reproduce any of them.

The core Praxis distinction is evidence-first agent/human continuity:

- Campaign frames the broad outcome.
- Beacon orients the reader.
- Strand scopes a meaningful line of work.
- Fiber scopes a concrete work unit.
- Directive preserves instruction semantics.
- Praxis Record preserves execution context.
- Report summarizes implementation evidence.
- Readout records evaluation evidence.
- Doctrine and Imprint prevent repeated conceptual drift.
- Relay transports artifacts but does not grant authority.
