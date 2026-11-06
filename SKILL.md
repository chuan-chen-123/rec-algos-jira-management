---
name: rec-algos-jira-management
description: Draft, create, improve and audit Rec Algos Jira epics, stories and subtasks, including acceptance criteria, team, labels, ownership, hierarchy, releases and Product links. Use for requested Jira work design and ticket maintenance.
---

# Rec Algos Jira Management

Make each ticket understandable to the person doing the work: what changes, why it matters, what is in scope, and what proves completion. This skill works independently of Virtual Me. All required guidance is inside this folder; the requester supplies work context and uses their own Jira access.

Read [team conventions](references/team-conventions.md) for Rec Algos defaults. For writing or reviewing descriptions, read [templates and examples](references/issue-writing.md). For live Jira reads or writes, read [provider workflow](references/jira-workflow.md). For scheduling or fix-version decisions, read [fiscal quarters](references/fiscal-quarters.md). For ticket replacement, consolidation or bulk restructuring, also read [history and hierarchy](references/history-and-hierarchy.md).

## Establish the requested work

Distinguish the requested mode:

| Request | Deliverable |
|---|---|
| Explain, brainstorm, draft or review | Usable proposed content or findings; leave Jira unchanged. |
| Create, update, fix, clean up or ensure fields are correct | Apply the bounded changes authorized by the requester and verify them. |
| Audit all stories or an entire epic | Enumerate the complete named scope, including relevant tasks and subtasks; follow every result page. Report coverage and remaining gaps. |

Resolve the issue/project, outcome, existing epic, relevant design or Product request, intended deliverable and any confirmed owner/release. Reuse supplied context and available sources. Ask only for information that materially affects the ticket; continue independent drafting or checks while it is unresolved.

Read current tickets, relevant full comments, attachments and relationships before rewriting. Use history when scope, ownership or completion is disputed. A planning row, volunteered name, proposed calendar allocation or intake idea is context; it does not establish an accepted assignment, start date or release commitment.

## Choose the structure

- **Epic:** a coherent outcome or agreed planning group with several related Stories. Reuse a suitable existing epic and describe all included workstreams and the completion boundary.
- **Story:** an independently accepted deliverable, including feature work, engineering/migration, analysis, research, investigation, documentation, operations or defect correction. Use the work-type label to distinguish the kind of work.
- **Subtask:** an implementation step under a parent Story, not directly under an epic.

Use only **Epic → Story → Subtask** when creating new work. Research and defect correction are Story scopes, not additional Jira issue types. A research Story can finish with a negative or inconclusive finding when its agreed evidence and next decision are complete.

Existing legacy Tasks or other types may be read and audited. Preserve their history and hierarchy; changing this skill does not itself authorize bulk conversion. When a specific conversion is requested, use the site's supported conversion workflow and verify the result.

Keep independently accepted deliverables separate. Group related work into a manageable set of epics; a new work item or lifecycle phase does not automatically require a new epic. Shared capabilities have one delivery home with consuming links. Distinguish feature implementation, experiment design, launch, readout and business impact where their acceptance differs.

## Write the ticket

Lead with a clear purpose and scope paragraph, then observable **Acceptance criteria**. Add technical context, dependencies and evidence links only when they help execution or review. Prefer a short paragraph and distinct bullets over a block of mixed sentences.

Write the desired result, comparison, artifact or decision precisely enough to distinguish pass, fail and unknown. Preserve important technical constraints, experimental populations, sources and later decisions. Unknown targets stay unconfirmed; avoid manufactured thresholds or promises of positive lift.

Keep structured metadata in Jira fields. Descriptions do not repeat work-type labels, assignee, Team, parent or fix version, and do not reproduce planning spreadsheets or migration logs. Explain meaningful acronyms. Keep long designs in linked documents. Templates are starting shapes, not mandatory sections or an invitation to add filler.

## Check the fields for every target

| Field | Completion check |
|---|---|
| Summary | Clear verb/outcome; no planning priority prefix such as `[P01]`. Meaningful workstream prefixes can remain. |
| Assignee | Confirmed delivery owner, resolved to the correct assignable account. Unknown stays unassigned; preserve existing assignments unless a change is requested or supported. An instruction to leave unassigned tickets unassigned takes precedence over proposed staffing. |
| Work type / labels | Apply the team's canonical work-type label and preserve unrelated useful labels. Classify by the deliverable/planning workstream, not an implementation verb. |
| Parent | Match the actual outcome and scope to the right epic. Retain subtasks under their standard-issue parent; check the containing epic as well. |
| Team | Set Recommendation Algorithms for Rec Algos epics and standard issues. Verify subtasks inherit the correct team. |
| Story Point Estimate | Set the numeric field on every new Story using the [team default](references/team-conventions.md#defaults-to-resolve-in-the-recipients-environment), unless the requester supplies another estimate. Verify the saved value; preserve existing estimates during edits. |
| Fix version | Set the fix version from the intended fiscal work quarter using the fiscal-quarter reference: Q2 is November–January; Q3 is February–April. Resolve the fiscal year, and leave genuinely unscheduled backlog work unversioned. |
| Product priority | Add the appropriate native linked issue where a verified Product mapping exists. Preserve the relation's meaning; a dependency, supporting contribution and direct deliverable are different. Missing matches stay explicit. |
| Description | Purpose, scope and verifiable acceptance criteria; essential context and sources retained; no duplicated field metadata. |

A consolidated epic can contain different work types. Within one agreed workstream, maintain consistent classification: for example, tests and data preparation supporting the LLM-as-a-Judge research workstream retain its modeling/research label.

## Apply and finish

Prepare a concrete field/content patch, preserving unrelated values and user edits. For creation, check for existing matching work, resolve required fields and parent, include Story Point Estimate for every Story, create once, and retain the returned key. For audits, distinguish missing, incorrect, inherited, intentionally blank and unverified fields.

For board visibility or placement requests, follow the board-placement checks in [provider workflow](references/jira-workflow.md); verify fix-version membership and actual board placement separately.

Verify the saved state and complete coverage. Check the requested changes and preservation of assignees, statuses, labels, release membership, relationships and rich content where relevant. Preserve concurrent edits; reconcile an affected planning source only within the authorized scope. Do not reopen completed work to make an old ticket resemble a new template.

Finish with links to the created/updated issues, a concise change summary and specific unresolved decisions. State actual counts only after complete enumeration and verification. A draft, attempted call or successful-looking outer response is not proof of a saved Jira update.
