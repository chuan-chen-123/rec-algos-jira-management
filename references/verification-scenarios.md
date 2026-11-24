# Verification scenarios

Use these cases when reviewing changes to this skill. Supply mock Jira fields and proposed actions; do not mutate live issues to evaluate the instructions. These are review scenarios, not evidence that an agent evaluation has been executed.

| Case | Given | Expected decision |
|---|---|---|
| New Story | Created November 24, 2026 in America/Los_Angeles; no version or explicit target. | Resolve FY27Q2, create the project version if absent and permitted, set it and read back the saved field. Do not infer board placement from the version. |
| Existing intake cleanup | An unfinished form-created Story or Epic is a named cleanup target; its version is blank and no intentional unversioned choice is recorded. | Apply the original creation timestamp's fiscal-quarter default even though the issue already existed before cleanup began. |
| Conversion across a quarter boundary | A Story created January 31, 2027 is cleaned or converted on February 1, 2027; no target/version is set. | Use FY27Q2 from creation, not FY27Q3 from the cleanup/conversion date. Align subtasks with their parent unless separately agreed. |
| Explicit release choice | A November-created Story already has FY27Q3, or the requester explicitly targets February. | Preserve/use FY27Q3. Preserve an explicit unversioned choice and completed historical version assignments as well. |
| Labels outside the allowlist | A scoped cleanup target has `experimentation-analysis`, `shared`, a pod label and `form-1234`. | Keep the applicable `experimentation-analysis` value and remove the other values. The only allowed labels are `experimentation-analysis`, `ai-enablement`, `engineering-pipelines` and `modeling-research`. Do not change issues outside the authorized scope. |
| Backlog batch without a move instruction | Content and fields for two scoped Stories are saved and verified; both remain in backlog. | Ask one closing question naming/linking both Stories. Do not move them before the answer, even when both have the current-quarter version. |
| Move already authorized | The requester explicitly says to move those Stories onto the board. | Move and verify them without asking again. Verify subtasks under their parent and preserve statuses, owners and hierarchy. |
| No placement question needed | No scoped Story remains in backlog, or the requester explicitly says to retain the Stories there. | Do not ask a redundant placement question or move the work. Read-only reviews and passive form submissions do not trigger a move. |

For each case, check the proposed field changes, any required closing question, preserved values and the evidence needed before reporting completion. Metadata/link validation alone does not demonstrate that these behavioral decisions are correct.
