# History, replacement and consolidation

Use this reference when the user requests migration, replacement, cleanup of duplicates, epic consolidation or bulk restructuring. Routine creation does not trigger a backlog-wide migration.

## Preserve the work's identity

Match tickets by actual deliverable, scope and acceptance, not a shared keyword. Keep independent stories independent and retain implementation subtasks beneath the correct standard issue. Preserve owners, status, comments, attachments, useful technical decisions, code/design links and dependencies unless the requested change requires otherwise.

Before replacing a ticket, compare the full original description, relevant complete comments, attachments, children and relationships with the replacement. If important context is missing, prefer refining the original and retiring the redundant replacement within the authorized scope. Carry useful new acceptance requirements back to the original without restarting completed work or losing history.

A many-to-one planning row is not automatically one execution story. Keep separately accepted deliverables as original tickets; a meaningful workstream prefix can identify their common purpose. Maintain the planning row's links to all relevant execution tickets.

## Consolidate epics carefully

Choose coherent surviving groups with explicit scope. Refresh each surviving epic's description to explain all its actual workstreams. Reparent the appropriate standard issues; their subtasks stay under them. Preserve Product links and issue-level metadata.

After verifying the moved children, reconcile the authorized planning source and confirm absorbed epics have no remaining work before closing or archiving them. Mark their disposition and destination clearly. Closure records consolidation rather than delivered business value.

## Archive and completed history

Archive only the explicitly authorized duplicates or obsolete records. Treat archiving as distinct from permanent deletion and verify the product's recovery behavior. A prior broad migration request is not ongoing authorization to delete later discoveries. Follow the host's action-time confirmation rules where applicable.

Keep completed work completed. Adding a relevant parent, Team or Product relationship can be appropriate when requested, but does not justify reopening or rewriting historical acceptance as a new commitment. An active subtask under a completed parent is an explicit hierarchy/workflow exception to resolve with the requester, not a reason to silently reopen the parent or flatten the child.

If approval or a provider restriction blocks retirement, finish the safe restoration/formatting work and state which duplicates remain. Do not describe a Won't Do transition, an archive and a permanent deletion as interchangeable actions.
