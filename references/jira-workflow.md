# Live Jira workflow

## Access and discovery

Use the recipient's connected Atlassian plugin for supported operations. Discover the currently exposed tools and their schemas; do not rely on a previous session's tool names, account IDs or field IDs. If an operation is unavailable, state the limitation and use an authorized browser fallback when available. Drafting can proceed without live access; label unverified fields accordingly.

Confirm the site/project and read the target before editing. Resolve the actual team and editable Team field. Prefer assignable-user lookup when selecting a named assignee. Inspect actual issue types, parents, releases, link types and transitions as needed. Use existing IDs already verified in this task rather than repeatedly rediscovering them.

## Reliable reads

- Enumerate every result page when auditing a named complete scope. A filtered board is not a complete project or backlog.
- Retrieve full comments with the comments operation and its pagination; an issue's comment count or embedded preview is not a full comment history.
- For rich-text edits, request lossless HTML and inspect the response's reported body format. Some integrations expose a converted preview alongside the actual tool body; use the actual body with its `appliedContentFormat` for round trips.
- Preserve native media, mentions, tables and local IDs. Consult the provider's current content-format guide before HTML writes. Plain Markdown is sufficient for new simple text when the provider supports it.

## Minimal writes

Create or reuse the epic before attaching children. Check for matching work using actual outcome, surface/cohort, artifact and acceptance scope. Read candidate matches before deciding they are duplicates.

Send only the intended fields. Multi-value fields are often replaced rather than appended: preserve the full intended label/link/component set. Set Team on standard issues and epics; verify subtask inheritance rather than forcing an unsupported edit.

Link verified Product ideas using native Jira relationships, not only a URL in the description. Preserve existing relationships and avoid duplicate links. A template or this skill never grants permission to send messages, create access, change workflows or expand a release.

An explicit create/update request authorizes the corresponding bounded work. A draft/review request does not. Explain concrete missing values, permission failures or host-required confirmations when they block the next step; continue unaffected authorized work.

## Errors and concurrency

Inspect both the outer tool result and its application payload. An outer success flag can wrap an `EDIT_FAILED` payload or a field-level rejection. Use the returned repair hint and verified field shape. For example, a Team field may need the resolved team UUID rather than its display name.

After a timeout or ambiguous response, read the actual target before retrying. Check for partial creation or edits; do not create the same issue again. If the same failure repeats without a supported repair, stop that mutation and report the exact gap rather than trying unverified fields or broadening access.

Preserve concurrent user changes. If a parent or scope changes during an audit, inspect the current record/history, avoid overwriting it from an old snapshot, and reconcile affected planning/epic text when authorized. Do not attribute a change to a particular actor without evidence.

## Verification and handoff

Read the requested fields after saving; edit responses may omit custom fields. For Team, verify the actual stored team identity, including inherited values. Confirm parent, labels, release membership and Product links as applicable. Check rich-content preservation after description edits.

For a large operation, keep a private execution record of scoped keys, before/after values, applied patches, partial failures and verification. Save it in the recipient's chosen task/workspace location, outside the distributed skill; no personal agent directory is required.

Return a concise result: changed keys/links, verified coverage, intentionally blank fields and unresolved decisions. A rollout, experiment start, analysis completion and measured business effect are separate claims.
