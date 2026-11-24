# Rec Algos conventions

These are the team's working conventions maintained from Chuan's Jira guidance through November 24, 2026. They are not a statement of company-wide Jira policy. Current explicit instructions and verified site settings take precedence.

## Defaults to resolve in the recipient's environment

| Setting | Default |
|---|---|
| Jira site | `https://stitchfix.atlassian.net` |
| Execution project | `RALGOS` — Recommendation Algos |
| Team field | **Recommendation Algorithms** |
| Story Point Estimate on new Stories | **2**, unless the requester explicitly supplies a different valid estimate. This is a starting default, not a reviewed effort commitment. |
| Product planning records | `CX` ideas, linked as native related issues when relevant |
| Access | Connected Atlassian plugin first; authorized browser fallback for unsupported operations |
| Release | Creation timestamp's fiscal quarter in America/Los_Angeles for new Epics/Stories and missing versions on unfinished Epics/Stories in an authorized cleanup; explicit target/unversioned choices override. Use [fiscal quarters](fiscal-quarters.md). |

Verify the site's actual Team and numeric Story point estimate fields, team identity, issue types, release IDs and edit permissions. Preserve existing estimates on edits; backfill missing values only within a requested scope. A supplied valid estimate, including 0, takes precedence over the default. Apply this default to Stories, rather than automatically estimating epics, legacy Tasks or subtasks. This package deliberately contains no account IDs, tokens, private personnel files, current staffing plan or fixed epic keys. It grants no access or permission changes.

## Canonical work-type labels

| Label | Purpose |
|---|---|
| `experimentation-analysis` | Experiment design, setup, measurement, analysis and readout |
| `engineering-pipelines` | Engineering, service/pipeline changes, migrations and infrastructure |
| `modeling-research` | Modeling, scientific evaluation and research |
| `ai-enablement` | AI/agent workflow enablement, evaluated for correctness and useful effort saved |

These are the only four permitted Jira label values for Epics, Stories and subtasks. Choose the appropriate work type from this set; a mixed Epic is not a reason to copy all its labels to every child. Tests or integration steps within a research workstream can retain that workstream's label.

Do not add any other label, even if it already exists in Jira. Pod names, `shared`, `form` and `form-<numeric form ID>` are not allowed. This replaces the earlier Epic pod-label convention; pod context must not be encoded in Labels.

On creation or explicitly authorized cleanup, read the current labels, preserve applicable allowed values, remove values outside this set, and verify the result. Continue using the required intake form, then remove its automatically added provenance labels. If the work type is unclear, report the classification gap rather than inventing a label. A scoped cleanup does not authorize a project-wide label migration or changes to the form configuration.

## Grouping and titles

Use a manageable number of groups with clear boundaries. In the current Outfit grouping, modeling/personalization, quality/coverage and serving/infrastructure are separate purposes. Category relevance and Category operations can share one Category epic. Resolve the actual current epic keys from Jira rather than encoding a dated roadmap in this skill.

Training-source migrations and production migration rollouts fit infrastructure when their deliverable is compatibility, cutover and operational handoff. Scientific model comparison or intent research has a different acceptance boundary. Determine the primary result rather than classifying every mention of a model as research.

Keep planning ranks such as P01 in the planning tool, outside Jira titles. Preserve informative prefixes such as `[LLM as a Judge]` or `[SIOM]`; define them in the epic. Where an existing naming convention matters, apply changes only to the requested scope.

## Ownership and release boundaries

Jira assignee identifies delivery ownership, not everyone who reviews or contributes. Confirm the account and distinguish technical owner, experiment design owner, analyst and Product decision owner when the work needs them. The skill does not allocate staff or turn proposed handoffs into accepted assignments.

Subtasks inherit Team from their parent on the verified Rec Algos site; direct Team edits on subtasks are rejected. Check inheritance through the actual parent, and preserve hierarchy.

Use [fiscal quarters](fiscal-quarters.md) for scheduling and missing-version decisions, including requested cleanup of existing intake items. Preserve explicit release choices and completed history; do not expand a scoped cleanup into a project-wide backfill. Board placement follows the separate [live workflow](jira-workflow.md#board-placement-and-visibility).
