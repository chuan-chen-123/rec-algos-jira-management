# Fiscal quarters and fix versions

For a new Story, default the fix version to the fiscal quarter containing its creation timestamp in America/Los_Angeles. An explicitly requested target quarter/month or instruction to leave the Story unversioned overrides this default. Use the team's month-based planning convention below.

| Fiscal quarter | Planning months | FY27 example | Fix version |
|---|---|---|---|
| Q1 | August–October | August–October 2026 | `FY27Q1` |
| Q2 | November–January | November 2026–January 2027 | `FY27Q2` |
| Q3 | February–April | February–April 2027 | `FY27Q3` |
| Q4 | May–July | May–July 2027 | `FY27Q4` |

A fiscal year runs from August of the preceding calendar year through July of the named year. Continue the same three-month pattern in later fiscal years: August 2027 is `FY28Q1`; November 2027 is `FY28Q2`.

## Apply the version

- When the requester says the story is planned for a named fiscal quarter, use its matching `FYnnQn` fix version. A story created in November for February work belongs to `FY27Q3`, not `FY27Q2`.
- If only a target month is supplied, derive the fiscal quarter from that month and year. January 2027 maps to `FY27Q2`; April 2027 to `FY27Q3`; July 2027 to `FY27Q4`.
- If the request says only “Q2” or “Q3,” resolve the fiscal year from the supplied plan or scheduling context. Ask when the year is genuinely ambiguous. When no target quarter or month is supplied, use the creation timestamp rather than asking for a schedule.
- When no explicit schedule is supplied, derive the default from the creation timestamp in America/Los_Angeles and resolve the matching Jira version. For example, November 6, 2026 maps to `FY27Q2`; January 31, 2027 is still `FY27Q2`; February 1, 2027 maps to `FY27Q3`. Absence of a target date is not a reason to leave a new Story unversioned. Leave it unversioned only when explicitly requested.
- This creation default does not authorize backfilling or changing existing tickets outside the requested scope. Historical priority IDs do not determine version membership.
- If work spans quarters, clarify the intended delivery quarter or use independently accepted Story slices where justified. Avoid automatically assigning multiple versions or copying every epic version to every child.
- Epics spanning quarters can contain stories with different versions. Keep each story's planned quarter explicit; align a Subtask with its parent Story unless a separately agreed schedule requires otherwise.
- Resolve the existing Jira project version by name. If the requested version does not exist, create it as part of an authorized scheduling/create request when permitted; otherwise report that specific gap. Ticket creation and version membership do not imply release, launch or completion.
- Change existing version membership only within the requested scheduling or maintenance scope. Preserve completed historical assignments unless explicitly asked to change them.
