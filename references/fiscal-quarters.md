# Fiscal quarters and fix versions

The fix version records the intended fiscal quarter for handling/delivering the story, not the quarter in which someone creates the ticket. Use the team's month-based planning convention below.

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
- If the request says only “Q2” or “Q3,” resolve the fiscal year from the supplied plan or scheduling context. Ask when the year is genuinely ambiguous. Creation date alone is not evidence of the intended work quarter.
- Unscheduled backlog work can stay without a fix version. This general quarter rule replaces any historical priority-ID cutoff as the rule for future stories; P01–P20 was one earlier plan's scope, not permanent eligibility.
- If work spans quarters, clarify the intended delivery quarter or use independently accepted Story slices where justified. Avoid automatically assigning multiple versions or copying every epic version to every child.
- Epics spanning quarters can contain stories with different versions. Keep each story's planned quarter explicit; align a Subtask with its parent Story unless a separately agreed schedule requires otherwise.
- Resolve the existing Jira project version by name. If the requested version does not exist, create it as part of an authorized scheduling/create request when permitted; otherwise report that specific gap. Ticket creation and version membership do not imply release, launch or completion.
- Change existing version membership only within the requested scheduling or maintenance scope. Preserve completed historical assignments unless explicitly asked to change them.
