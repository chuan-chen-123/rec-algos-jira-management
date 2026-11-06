# Rec Algos conventions

These are the team's working conventions distilled from Chuan's Jira guidance on November 5, 2026. They are not a statement of company-wide Jira policy. Current explicit instructions and verified site settings take precedence.

## Defaults to resolve in the recipient's environment

| Setting | Default |
|---|---|
| Jira site | `https://stitchfix.atlassian.net` |
| Execution project | `RALGOS` — Recommendation Algos |
| Team field | **Recommendation Algorithms** |
| Product planning records | `CX` ideas, linked as native related issues when relevant |
| Access | Connected Atlassian plugin first; authorized browser fallback for unsupported operations |
| Release | Intended fiscal work quarter; use [fiscal quarters](fiscal-quarters.md) for `FYnnQn` naming and month mapping |

Verify the site's actual Team custom field, team identity, issue types, release IDs and edit permissions. This package deliberately contains no account IDs, tokens, private personnel files, current staffing plan or fixed epic keys. It grants no access or permission changes.

## Canonical work-type labels

| Label | Purpose |
|---|---|
| `experimentation-analysis` | Experiment design, setup, measurement, analysis and readout |
| `engineering-pipelines` | Engineering, service/pipeline changes, migrations and infrastructure |
| `modeling-research` | Modeling, scientific evaluation and research |
| `ai-enablement` | AI/agent workflow enablement, evaluated for correctness and useful effort saved |

Use the agreed primary work type for the planning workstream. Preserve existing non-work-type labels that remain useful. A mixed epic is not a reason to give every child the epic's label. A test or integration step within a research workstream is not automatically a separate engineering workstream.

## Grouping and titles

Use a manageable number of groups with clear boundaries. In the current Outfit grouping, modeling/personalization, quality/coverage and serving/infrastructure are separate purposes. Category relevance and Category operations can share one Category epic. Resolve the actual current epic keys from Jira rather than encoding a dated roadmap in this skill.

Training-source migrations and production migration rollouts fit infrastructure when their deliverable is compatibility, cutover and operational handoff. Scientific model comparison or intent research has a different acceptance boundary. Determine the primary result rather than classifying every mention of a model as research.

Keep planning ranks such as P01 in the planning tool, outside Jira titles. Preserve informative prefixes such as `[LLM as a Judge]` or `[SIOM]`; define them in the epic. Where an existing naming convention matters, apply changes only to the requested scope.

## Ownership and release boundaries

Jira assignee identifies delivery ownership, not everyone who reviews or contributes. Confirm the account and distinguish technical owner, experiment design owner, analyst and Product decision owner when the work needs them. The skill does not allocate staff or turn proposed handoffs into accepted assignments.

Subtasks inherit Team from their parent on the verified Rec Algos site; direct Team edits on subtasks are rejected. Check inheritance through the actual parent, and preserve hierarchy.

Use [fiscal quarters](fiscal-quarters.md) for all scheduling and fix-version decisions. Planned quarter, not ticket creation date or priority ID, determines version membership. Preserve completed history and independently queued backlog work.
